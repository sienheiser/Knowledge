## What do you need?
You need a VM where you can install the gitlab-runner software see 
https://docs.gitlab.com/runner/install/linux-repository.html. 
In the same VM create an ssh key. 
Suppose you have repos test1 and test2. Let test1 have a .gitlab-ci.yml and be a submodule of test2. Suppose you want the runner to do the following actions every time a commit is made to test1
1. git clone test2 through ssh
2. navigate into the repo and initialize the submodule test1

The rest of this document will describe how to do this.

## Setting up runner
If you have not registered the VM as a runner then go to test1/Settings/CI CD/Runners. Click the new project runner button 

In the Tags field you can add different tags. These tags can be used in the .gitlab-ci.yml to specify which runner to use. If you tick Run untagged jobs this allows .gitlab-ci.yml without any tags to use the Runner. Then click create runner.

In the next page you will be given instructions to follow. This page is self contained. Ensure that you have installed the gitlab-runner software see https://docs.gitlab.com/runner/install/linux-repository.html. 

That is it you have registered a new runner that can be used for any project.
## Giving permissions
You want the runner to clone and initialize repos without using your own gitlab user name and password. Start by generating a ssh key
```
ssh-keygen -t rsa -b 2048 -C "<comment>"
```
### Adding permissions to test1
#### Private Key
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
I think you need to add the private key to test1 because this is where we trigger the automated process.
#### Public Key
In gitlab go to test1>Settings>Repository>Deploy Key> Add key
copy and paste the public key.

### Adding permissions to test2
By now you have registered the public key in test1. You should also register it in test2. Do this by going to  test2>Settings>Repository>Deploy Key> Add key>Privately accessible deploy keys;
you should see the public key that you just registered for test1.
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
