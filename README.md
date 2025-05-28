# VIRTUAL-MACHINES-
### NAME : Thaanesh.V
### REGISTER NUMBER : 212223230228
## EX 6: MOVING FILES BETWEEN VIRTUAL MACHINES

### Aim: 

To move the files between virtual machine. 

You can move files between virtual machines in several ways: 

• You can copy files using network utilities as you would between physical computers on your network.

To do this between two virtual machine: • Both virtual machines must be configured to allow access to your network. 


• Any of the networking methods (host-only, bridged and NAT) are appropriate.

• With host-only networking, you copy files from the virtual machines to the host and vice-versa, since host-only networking only allows the virtual machines see your host computer.

• With bridged networking or NAT enabled, you can copy files across your network between the virtual machines.

• You can create a shared drive, either a virtual disk or a raw partition, and mount the drive in each of the virtual machines.

### Procedure: 
How to Enable File Sharing in VirtualBox. 

Step 1. Install Guest Additions on the Guest machine. 

Step 2. Configure File Sharing on VirtualBox.

<br>

Step 1. Install Guest Additions on the Guest machine.

1. Start the Virtuabox Guest Machine (OS).
2. From Oracle's VM VirtualBox main menu, select Devices > Install Guest Additions *

a. Open Windows Explorer


b. Double click at the "CD Drive (X:) VirtualBox Guest additions" to explore its contents.

![image](https://github.com/user-attachments/assets/4aef06f8-bf3e-43c8-aa8a-fd29a836e427)


C.Right click at "VBoxWindowsAdditions" application and from the pop-up menu, choose "Run as administrator".

![image](https://github.com/user-attachments/assets/2e310381-979b-485e-b1b1-1b606418cdcc)

3.Press Next and then follow the on screen instructions to complete the Guest Additions installation.

![image](https://github.com/user-attachments/assets/a5939d0b-2473-4a85-869b-7875461fc89b)


4.When the setup is completed, choose Finish and restart the Virtuabox guest machine.

Step 2. Setup File Sharing on VirtualBox Guest Machine.

5. From VirtualBox menu click Devices and choose Shared Folders -> Shared Folder Settings.

![image](https://github.com/user-attachments/assets/cdf7cbbc-28d2-4ad6-93a2-29a291ffd74d)

Click the Add new shared folder icon.

![image](https://github.com/user-attachments/assets/a875dbc2-3c7d-46ba-8de3-e8bae26e5756)

Click the drop-down arrow and select Other.

![image](https://github.com/user-attachments/assets/d57c14b7-ed7e-4634-ae01-f0701d8eac25)

Locate and highlight (from the Host OS) the folder that you want to share between the VirtualBox Guest machine and the Host and click Select Folder. 

Note: To make your life easier, create a new folder for the file sharing, on the Host OS and give it with a recognizable name. (e.g. "Public")

![image](https://github.com/user-attachments/assets/e9488467-9c16-46da-83d6-76b399ed92ec)

Now, in the 'Add Share' options, type a name (if you want) at the 'Folder Name box, click the Auto Mount and the Make Permanent checkboxes and click OK twice to close the Shared Folder Settings.

![image](https://github.com/user-attachments/assets/01cf9664-60ef-4e38-b059-17ba6761759c)

You 're done! To access the shared folder from the Guest OS, open Windows Explorer and under the 'Network locations' you should see a new network drive that corresponds to the shared folder on the Host OS.

### Result:

Thus the virtual machine files are moved to another VM

