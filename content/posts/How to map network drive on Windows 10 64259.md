---
title: "Unlock the Power of Windows 10: Learn How to Map Your Network Drive in Seconds!"
ShowToc: true 
date: "2023-03-05"
author: "Cary Huber"
---
*****
# Unlock the Power of Windows 10: Learn How to Map Your Network Drive in Seconds!

Windows 10 is the most popular operating system in the world, and its users are constantly discovering new ways to make the most of its powerful features. One such feature is the ability to map a network drive, which allows you to access files and folders stored on other computers or servers on your network. Mapping a network drive is an essential skill for anyone working in a business or home setting, where files and data need to be shared across devices. In this article, we will show you how to map your network drive in seconds!

## What is a network drive?

First, let us understand what a network drive is. A network drive is a storage device that is connected to your network, and which can be accessed by multiple computers or devices. By mapping your network drive, you are essentially connecting your computer to the network drive, so that you can access the files and folders stored on it.

## How to map your network drive

Mapping a network drive in Windows 10 is a quick and easy process. Here are the steps to follow:

### Step 1: Open File Explorer

To open File Explorer, press the Windows key and E on your keyboard, or click on the File Explorer icon in your taskbar.

### Step 2: Click on "This PC"

In the left pane of File Explorer, you will see a list of folders and devices. Click on "This PC" to see an overview of your computer's storage devices.

### Step 3: Click on "Map network drive"

In this window, you will see a "Map network drive" button in the toolbar at the top of the window. Click on it.

### Step 4: Choose a drive letter

Choose a drive letter from the drop-down menu. This drive letter will be used to access your network drive in Windows. You can choose any available letter.

### Step 5: Type in the network path

In the "Folder" field, type in the network path to your network drive. This path will start with either "\\" or "smb://", depending on the type of network drive you are connecting to. You will need to check with your network administrator to get the correct path.

### Step 6: Connect using different credentials

If you need to connect to the network drive using different credentials, click on the "Connect using different credentials" checkbox. You will be prompted to enter your network username and password.

### Step 7: Click "Finish"

Once you have entered all the required information, click on the "Finish" button. Windows will now connect to your network drive and create a shortcut to it on your computer.

## Conclusion

Mapping a network drive in Windows 10 is a simple and powerful tool that can help you access files and folders stored on other computers or servers on your network. By following the simple steps outlined in this article, you can quickly and easily map your network drive, unlock the full power of Windows 10, and take your productivity to the next level.

{{< youtube q8KVJdgewNk >}} 



- To map network drive on Windows 10, open File Explorer > This PC and click “Map network drive.”
 - Then select the drive letter for the mapping, confirm the network path for the drive, and click Finish to complete the mapping on Windows 10.
 - Alternatively, on Command Prompt (non-admin), use the “net use \\SERVER\FOLDERPATH” command to map a network drive.
 - Or, on PowerShell, use the “New-PSDrive -Name “LETTER” -PSProvider “FileSystem” -Root “\\SERVER\FOLDERPATH” -Persist” command to map a drive on Windows 10.

 
On Windows 10, you can map a network drive to quickly access files stored in a shared folder on another computer (or server) connected to the network.
 
When you connect to a drive using the “Map Network Drive” option on Windows 10, the system essentially creates a “shortcut” that points to the network shared folder with a drive letter and access credentials. The mapped drive then appears on “This PC” under the “Network locations” section to give you quick access to those files stored on the remote computer.
 
This guide will teach you how to map a network drive on Windows 10. In addition, you’ll learn how to disconnect it using the options available in File Explorer, Command Prompt, and PowerShell.
 
- Map network drive on Windows 10
 - Disconnect mapped drive on Windows 10

 
## Map network drive on Windows 10
 
On Windows 11, you can map a network drive in at least three ways using the File Explorer wizard and commands with Command Prompt and PowerShell.
 
### Network drive map from File Explorer
 
To map a network drive on Windows 10 from File Explorer, use these steps:
 
- Open File Explorer on Windows 10.
 - Click on This PC from the left pane.
 - Click the “Map network drive” option from the “Computer” tab.
 - Use the “Drive” drop-down menu and select an unused letter to assign the drive. (Or you can use the default selection.)
 - In the “Folder” field, enter the network path to the shared folder. (Or click the Browse button to browse to the folder to map as a network drive, and click the OK button.)
 - Check the “Reconnect at sign-in” option to connect to the network location permanently.
 - Check the “Connect using different credentials” option if the credentials are different from the account you are already using to sign in to Windows 10.
 - Click the Finish button.
 - Confirm the network account credentials (if applicable).
 - Click the OK button.

 
Once you complete the steps, the drive will map and become available in File Explorer.
 
Open File Explorer on Windows 10.
 
Click on This PC from the left pane.
 
Click the “Map network drive” option from the “Computer” tab.
 

 
Use the “Drive” drop-down menu and select an unused letter to assign the drive. (Or you can use the default selection.)
 
In the “Folder” field, enter the network path to the shared folder. (Or click the Browse button to browse to the folder to map as a network drive, and click the OK button.)
 
Check the “Reconnect at sign-in” option to connect to the network location permanently.
 
Check the “Connect using different credentials” option if the credentials are different from the account you are already using to sign in to Windows 10.
 
Click the Finish button.
 
Confirm the network account credentials (if applicable).
 
Click the OK button.
 
If you cannot connect to the shared folder, use the IP address instead of the computer name. However, if the remote computer uses a dynamic IP address configuration, it may change in the future, and you may need to reconnect again.
 
### Network drive map from Command Prompt
 
To map a network drive from Command Prompt on Windows 10, use these steps:
 
- Open Start.
 - Search for Command Prompt and click the top result to open the console.
 - Quick note: If you run the command as an administrator, the drive may not mount correctly and won’t appear in File Explorer. As a result, run the command as a standard user.
 - Type the following command to map a drive assigning drive letter manually and press Enter:
 - net use Z: \\DEVICE-NAME-OR-IP\SHARED-FOLDER
 - In the command, replace “Z” with the drive letter not already in use you want to use. Then replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the shared. For example, this command maps the ShareOne folder to the computer with the “Z” drive letter:
 - net use Z: \\vm-beta\ShareOne
 - Type the following command to map a drive assigning drive letter automatically and press Enter:
 - net use * \\DEVICE-NAME-OR-IP\SHARED-FOLDER
 - In the command, the (*) is the option that allows the system to assign any drive letter that is not already in use. Then replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the shared. For example, this command maps the ShareOne folder to the computer:
 - net use * \\vm-beta\ShareOne
 - Type the following command to map a drive providing authentication details and press Enter:
 - net use Z: \\DEVICE-NAME-OR-IP\SHARED-FOLDER PASSWORD /user:USERNAME /persistent:yes
 - In the command, replace “Z” with the drive letter not already in use you want to use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the shared. The PASSWORD and USERNAME have to be replaced with the credentials to authenticate with the remote machine. The “persistent” option allows the folder to stay mapped after reboot. For example, this command maps the ShareOne folder providing the user credentials and making the mapping persistent:
 - net use Z: \\vm-beta\ShareOne password /user:admin /persistent:yes

 
Once you complete the steps, the network-shared folder will map on the device and appear in File Explorer.
 
Open Start.
 
Search for Command Prompt and click the top result to open the console.
 
Type the following command to map a drive assigning drive letter manually and press Enter:
 
net use Z: \\DEVICE-NAME-OR-IP\SHARED-FOLDER
 
In the command, replace “Z” with the drive letter not already in use you want to use. Then replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the shared. For example, this command maps the ShareOne folder to the computer with the “Z” drive letter:
 
net use Z: \\vm-beta\ShareOne
 
Type the following command to map a drive assigning drive letter automatically and press Enter:
 
net use * \\DEVICE-NAME-OR-IP\SHARED-FOLDER
 
In the command, the (*) is the option that allows the system to assign any drive letter that is not already in use. Then replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the shared. For example, this command maps the ShareOne folder to the computer:
 
net use * \\vm-beta\ShareOne
 
Type the following command to map a drive providing authentication details and press Enter:
 
net use Z: \\DEVICE-NAME-OR-IP\SHARED-FOLDER PASSWORD /user:USERNAME /persistent:yes
 
In the command, replace “Z” with the drive letter not already in use you want to use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the shared. The PASSWORD and USERNAME have to be replaced with the credentials to authenticate with the remote machine. The “persistent” option allows the folder to stay mapped after reboot. For example, this command maps the ShareOne folder providing the user credentials and making the mapping persistent:
 
net use Z: \\vm-beta\ShareOne password /user:admin /persistent:yes
 
### Network drive map from PowerShell
 
To map a network drive from PowerShell on Windows 10, use these steps:
 
- Open Start.
 - Search for PowerShell and click the top result to open the console.
 - Type the following command to map a drive assigning drive letter manually and press Enter:
 - New-PSDrive -Name "DRIVE-LETTER" -PSProvider "FileSystem" -Root "\\DEVICE-NAME-OR-IP\SHARED-FOLDER" -Persist
 - In the command, replace DRIVE-LETTER with the drive letter not already in use you want to use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the shared. For example, this command maps the ShareOne folder to the computer with the “E” drive letter:
 - New-PSDrive -Name "E" -PSProvider "FileSystem" -Root "\\vm-beta\ShareOne" -Persist

 
Once you complete the steps, the network shared folder will map on the computer and appear in File Explorer.
 
Search for PowerShell and click the top result to open the console.
 
New-PSDrive -Name "DRIVE-LETTER" -PSProvider "FileSystem" -Root "\\DEVICE-NAME-OR-IP\SHARED-FOLDER" -Persist
 
In the command, replace DRIVE-LETTER with the drive letter not already in use you want to use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the shared. For example, this command maps the ShareOne folder to the computer with the “E” drive letter:
 
New-PSDrive -Name "E" -PSProvider "FileSystem" -Root "\\vm-beta\ShareOne" -Persist
 
If you need to map a drive using credentials, follow these instructions.
 
## Disconnect mapped drive on Windows 10
 
When you no longer need access to the network drive, you can disconnect using the same methods, including File Explorer, Command Prompt, or PowerShell.
 
### Disconnect network drive from File Explorer
 
To disconnect a network drive on Windows 10, use these steps:
 
- Open File Explorer.
 - Click on This PC from the left pane.
 - Under the “Network Locations” section, right-click the network drive, and select the Disconnect option.
 - Quick tip: Alternatively, you can select the network drive, and on the “Computer” tab, click the Map network driver sub-button and select the Disconnect network drive option.

 
After you complete the steps, the network drive will no longer be available on Windows 10.
 
Open File Explorer.
 
Under the “Network Locations” section, right-click the network drive, and select the Disconnect option.
 
### Disconnect network drive from Command Prompt
 
To disconnect a network drive from Command Prompt on Windows 10, use these steps:
 
- Open Start.
 - Search for Command Prompt and click the top result to open the console.
 - Type the following command to disconnect a mapped network drive and press Enter:
 - net use z: /Delete
 - In the command, replace “Z” with the drive letter of the map you want to remove.
 - Type the following command to disconnect all the mapped network drives and press Enter:
 - net use * /Delete

 
After you complete the steps, the mapped drives will be disconnected and no longer accessible from File Explorer.
 
Type the following command to disconnect a mapped network drive and press Enter:
 
net use z: /Delete


 
In the command, replace “Z” with the drive letter of the map you want to remove.
 
Type the following command to disconnect all the mapped network drives and press Enter:
 
net use * /Delete


 
### Disconnect network drive from PowerShell
 
To disconnect and remove a mapped network drive with PowerShell, use these steps:
 
- Open Start.
 - Search for PowerShell and click the top result to open the console.
 - Type the following command to view all the mapped drives and press Enter:
 - Get-PSDrive -PSProvider "FileSystem"
 - Type the following command to disconnect the mapped network drive and press Enter:
 - Remove-PSDrive -Name DRIVE-LETTER
 - In the command, replace DRIVE-LETTER with the drive letter of the mapping. For example, this command disconnects the “E” drive:
 - Remove-PSDrive -Name E
 - (Optional) Type the following command to disconnect multiple mappings and press Enter:
 - Get-PSDrive DRIVER-LETTER-1, DRIVE-LETTER-2 | Remove-PSDrive
 - In the command, replace DRIVER-LETTER-1 and DRIVE-LETTER-2 with the drive letters you want to disconnect. For example, this command disconnects the “E” and “F” drives:
 - Get-PSDrive E, F | Remove-PSDrive

 
Once you complete the steps, the drive mapping will be removed from Windows 10.
 
Type the following command to view all the mapped drives and press Enter:
 
Get-PSDrive -PSProvider "FileSystem"
 
Type the following command to disconnect the mapped network drive and press Enter:
 
Remove-PSDrive -Name DRIVE-LETTER
 
In the command, replace DRIVE-LETTER with the drive letter of the mapping. For example, this command disconnects the “E” drive:
 
Remove-PSDrive -Name E
 
(Optional) Type the following command to disconnect multiple mappings and press Enter:
 
Get-PSDrive DRIVER-LETTER-1, DRIVE-LETTER-2 | Remove-PSDrive
 
In the command, replace DRIVER-LETTER-1 and DRIVE-LETTER-2 with the drive letters you want to disconnect. For example, this command disconnects the “E” and “F” drives:
 
Get-PSDrive E, F | Remove-PSDrive




