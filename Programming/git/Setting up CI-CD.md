## Setting up runner
Suppose you want to try using CI/CD techniques. Let's say you have some virtual machine that you want to set up as a runner. Go to the repository you want to automate then go to Settings>CI/CD>Runners. You will see an option to register a new runner, just follow the instruction they are self contained. 
The instructions below work for docker container with python3.9 as version.
**Note you will need to install the gitlab runner software on the VM that you want to become a runner. This is also found the instructions ** 

## Configuring the runner and gitlab
### Generating keys
In the VM generate a ssh key by typing the following
```
ssh-keygen -t rsa -b 2048 -C "<comment>"
```
### Adding private key
In gitlab go to test1>Settings>Repository>CI/CD>Variables>Add variable

A prompt will open up and in there you should copy and paste the private key that was generated in **value**; include the starting and ending e.g.
```
-----BEGIN RSA PRIVATE KEY-----
<private key>
-----END RSA PRIVATE KEY-----
```
In **key** field name the variable as
```
SSH_PRIVATE_KEY
```
### Adding public key
In gitlab go to test2>Settings>Repository>Deploy Key> Add key
Copy and paste the public key. Give it a name of your choice.

## yml file
In test1 create file .gitlab-ci.yml
The code below successfully clones repo test2 into runner at the moment it does not successfully initializes the submodule.
``` yml
stages:
  - clone_and_setup_test2

clone_and_setup_test2:
  stage: clone_and_setup_test2
  before_script:
    - 'which ssh-agent || (apt-get update -y && apt-get install openssh-client -y)'  # Ensure SSH client is installed
    - eval $(ssh-agent -s)  # Start the SSH agent
    - echo "$SSH_PRIVATE_KEY" | tr -d '\r' | ssh-add -  # Add the SSH private key stored in CI variables
    - mkdir -p ~/.ssh  # Create SSH directory if it does not exist
    - chmod 700 ~/.ssh  # Set correct permissions for SSH directory
    - ssh-keyscan gitlab.esss.lu.se >> ~/.ssh/known_hosts  # Add GitLab to known hosts to prevent manual prompt
  script:
    - echo "Cloning test2 repository..."
    - git clone git@gitlab.esss.lu.se:emmanueldcosta/test2.git # Use SSH to clone test2 (no username required)
    - cd test2
    - echo "Initializing submodules..."
    - git submodule update --init --recursive  # Initialize and update submodules
  tags:
    - emmanuel-test-runner  # Add your specific runner tag here
  only:
    - branches  # Runs for all branches, adjust if you want specific branches like 'main'
```
