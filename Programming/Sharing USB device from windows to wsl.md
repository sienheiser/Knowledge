1. Go to the [latest release page for the usbipd-win project](https://github.com/dorssel/usbipd-win/releases).
2. Select the .msi file, which will download the installer. (You may get a warning asking you to confirm that you trust this download).
3. Run the downloaded usbipd-win_x.msi installer file.

This will install:
- A service called `usbipd` (display name: USBIP Device Host). You can check the status of this service using the Services app from Windows.
- A command line tool `usbipd`. The location of this tool will be added to the PATH environment variable.
- A firewall rule called `usbipd` to allow all local subnets to connect to the service. You can modify this firewall rule to fine tune access control.

Before attaching your USB device, ensure that a WSL command line is open. This will keep the WSL 2 lightweight VM active.

1. List all of the USB devices connected to Windows by opening PowerShell in _administrator_ mode and entering the following command. Once the devices are listed, select and copy the bus ID of the device you’d like to attach to WSL.
    
    PowerShellCopy
    
    ```
    usbipd list
    ```
    
2. Before attaching the USB device, the command `usbipd bind` must be used to share the device, allowing it to be attached to WSL. This requires administrator privileges. Select the bus ID of the device you would like to use in WSL and run the following command. After running the command, verify that the device is shared using the command `usbipd list` again.
    
    PowerShellCopy
    
    ```
    usbipd bind --busid 4-4
    ```
    
3. To attach the USB device, run the following command. (You no longer need to use an elevated administrator prompt.) Ensure that a WSL command prompt is open in order to keep the WSL 2 lightweight VM active. Note that as long as the USB device is attached to WSL, it cannot be used by Windows. Once attached to WSL, the USB device can be used by any distribution running as WSL 2. Verify that the device is attached using `usbipd list`. From the WSL prompt, run `lsusb` to verify that the USB device is listed and can be interacted with using Linux tools.
    
    PowerShellCopy
    
    ```
    usbipd attach --wsl --busid <busid>
    ```
    
4. Open Ubuntu (or your preferred WSL command line) and list the attached USB devices using the command:
    
    BashCopy
    
    ```
    lsusb
    ```
    
    You should see the device you just attached and be able to interact with it using normal Linux tools. Depending on your application, you may need to configure udev rules to allow non-root users to access the device.
    
5. Once you are done using the device in WSL, you can either physically disconnect the USB device or run this command from PowerShell:
    
    PowerShellCopy
    
    ```
    usbipd detach --busid <busid>
    ```
