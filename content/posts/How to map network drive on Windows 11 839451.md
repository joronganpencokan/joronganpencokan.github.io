---
title: "Windows 11 Users Rejoice! Learn the Ultimate Hack to Streamline Your Work with a Simple Network Drive Mapping Trick"
ShowToc: true 
date: "2023-01-12"
author: "Dennise Donley"
---
*****
# Windows 11 Users Rejoice: The Ultimate Hack to Streamline Your Work with a Simple Network Drive Mapping Trick

If you're a Windows 11 user, you know how crucial it is to have all of your files and applications accessible at a moment's notice. Whether you're managing a team of coworkers or working solo, having quick access to your work can make or break your productivity. But did you know there's a simple trick to streamline your work and save yourself time and effort? With network drive mapping, you can access your files and applications with ease, so you can focus on what really matters: getting your work done.

What is Network Drive Mapping?

In simple terms, network drive mapping is the process of assigning a drive letter to a remote network location. Essentially, you're creating a shortcut on your computer that leads to a folder or application stored elsewhere on the network. By mapping a network drive, you're making it easier to access important files and resources that might otherwise be buried deep in your company's file system.

Why Should You Use Network Drive Mapping?

There are several reasons why network drive mapping is useful for Windows 11 users. Here are just a few benefits to consider:

1. Easy access to important files: By mapping a network drive, you can quickly access important files without having to navigate through multiple folders. This can save you time and help you stay organized.

2. Collaboration made easy: If you're working on a project with others, mapping a network drive can streamline collaboration. Everyone can access the same files easily, ensuring that everyone is working from the same page.

3. Better security: By mapping a network drive, you can ensure that your data is secure. If you're sharing files with others, you can set permissions and control access to sensitive information.

How to Map a Network Drive on Windows 11

Now that you know why network drive mapping is useful, you're probably wondering how to do it. Fortunately, the process is straightforward and easy to follow. Here's a step-by-step guide:

Step 1: Open File Explorer

Begin by opening File Explorer. You can do this by clicking on the folder icon in your taskbar.

Step 2: Select "This PC"

In File Explorer, select "This PC" from the left-hand menu.

Step 3: Click "Map network drive"

At the top of the screen, click on "Map network drive."

Step 4: Choose a drive letter

In the "Map network drive" window, choose a drive letter. This will be the letter assigned to your network drive.

Step 5: Choose a folder

Next, click "Browse" and select the folder you want to map.

Step 6: Check "Reconnect at sign-in"

If you want the network drive to be mapped every time you sign in to your computer, check the box next to "Reconnect at sign-in."

Step 7: Click "Finish"

Finally, click "Finish" to complete the process. The network drive will now appear in File Explorer under "This PC."

Final Thoughts

Mapping a network drive might seem like a small step, but the benefits it provides can make a significant impact on your productivity. With network drive mapping, you can access important files quickly and collaborate more effectively. So if you're a Windows 11 user looking to streamline your work, give network drive mapping a try. Your workflow will thank you!

{{< youtube ORdWE_ffirg >}} 



Windows 11 has several ways to map a network drive to your computer, including using File Explorer or commands with PowerShell or Command Prompt. This guide will show you how, including the steps to disconnect.
 
When mapping a network drive, the system technically only creates a “shortcut” or “pointer” that allows Windows 11 to locate the shared folder and access its contents as if it was a drive physically attached to the computer. After the mapping process is complete, the storage will appear on “This PC” under the “Network locations” section in File Explorer.
 
If you no longer need access to the network resources, Windows 11 also provides quick ways to disconnect the network drive using the same tools.
 
In this guide, you will learn the steps to use File Explorer, Command Prompt, and PowerShell to map a network drive on Windows 11.
 
- Map network drive on Windows 11 using File Explorer
 - Disconnect mapped network drive on Windows 11 using File Explorer
 - Map network drive on Windows 11 using PowerShell
 - Disconnect mapped network drive on Windows 11 using PowerShell
 - Map network drive on Windows 11 with Command Prompt
 - Disconnect mapped network drive on Windows 11 with Command Prompt

 
## Map network drive on Windows 11 using File Explorer
 
To map a network drive with File Explorer on Windows 11, use these steps:
 
- Open File Explorer on Windows 11.
 - Click on This PC from the left pane.
 - Click the See more (three-dotted) button in the command bar and select the “Map network drive” option.
 - Use the “Drive” drop-down menu and choose a letter to assign the drive.
 - In the “Folder” field, enter the network path to the shared folder. (Or click the Browse button to browse the folder to map as a network drive, and click the OK button.)
 - Check the “Reconnect at sign-in” option to make the connection permanent.
 - Check the Connect using different credentials option if the credentials are different from the account you are already using.
 - Click the Finish button.
 - Confirm the network account credentials (if applicable) to map the network drive to Windows 11.
 - Click the OK button.

 
Once you complete the steps, the network drive will become available in File Explorer.
 
Open File Explorer on Windows 11.
 
Click on This PC from the left pane.
 
Click the See more (three-dotted) button in the command bar and select the “Map network drive” option.
 

 
Use the “Drive” drop-down menu and choose a letter to assign the drive.
 
In the “Folder” field, enter the network path to the shared folder. (Or click the Browse button to browse the folder to map as a network drive, and click the OK button.)
 
Check the “Reconnect at sign-in” option to make the connection permanent.
 
Check the Connect using different credentials option if the credentials are different from the account you are already using.
 
Click the Finish button.
 
Confirm the network account credentials (if applicable) to map the network drive to Windows 11.
 
Click the OK button.
 
If you cannot connect to the shared folder, use the IP address instead of the computer name. However, if the remote device uses a dynamic IP address configuration, it may change in the future, and you may need to reconnect again.
 
Also, if the device providing the resources is using a Microsoft account with the passwordless option, you will need to create a local account you can use to connect. Otherwise, the mapping won’t work.
 
## Disconnect mapped network drive on Windows 11 using File Explorer
 
To disconnect a network drive on Windows 11, use these steps:
 
- Open File Explorer.
 - Click on This PC from the left pane.
 - Under the “Network Locations” section, right-click the network drive (select See more options) and choose the Disconnect option.

 
After you complete the steps, the network drive will no longer be available on the computer.
 
Open File Explorer.
 
Under the “Network Locations” section, right-click the network drive (select See more options) and choose the Disconnect option.
 
## Map network drive on Windows 11 using PowerShell
 
To map a network drive with PowerShell commands, use these steps:
 
- Open Start.
 - Search for PowerShell and click the top result to open the console.
 - Quick tip: Do not run the terminal as an administrator to allow the mount to appear in File Explorer.
 - Type the following command to map network drive assigning letter manually and press Enter:
 - New-PSDrive -Name "DRIVER-LETTER" -PSProvider "FileSystem" -Root "\\DEVICE-NAME-OR-IP\SHARED-FOLDER" -Persist
 - In the command, replace DRIVER-LETTER with a drive letter not already in use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the computer hosting the shared folder and the name of the share.
 - For example, this command maps the ShareFiles folder to the computer with the “Z” drive letter:
 - New-PSDrive -Name "Z" -PSProvider "FileSystem" -Root "\\vm-10v21h2\ShareFiles" -Persist

 
Once you complete the steps, the shared folder will mount as a network drive on the computer, and it will appear in File Explorer.
 
Open Start.
 
Search for PowerShell and click the top result to open the console.
 
Type the following command to map network drive assigning letter manually and press Enter:
 
New-PSDrive -Name "DRIVER-LETTER" -PSProvider "FileSystem" -Root "\\DEVICE-NAME-OR-IP\SHARED-FOLDER" -Persist
 
In the command, replace DRIVER-LETTER with a drive letter not already in use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the computer hosting the shared folder and the name of the share.
 
For example, this command maps the ShareFiles folder to the computer with the “Z” drive letter:
 
New-PSDrive -Name "Z" -PSProvider "FileSystem" -Root "\\vm-10v21h2\ShareFiles" -Persist
 
### Map network drive with password on PowerShell
 
To map a network drive providing the account name and password, use these steps:
 
- Open Start.
 - Search for PowerShell and click the top result to open the console.
 - Type the following command to create a variable to store the account information and press Enter:
 - $cred = Get-Credential -Credential USERNAME
 - Quick tip: If you are mapping a drive in Active Directory, specify the user name like this: network\admin.
 - Confirm the account password.
 - Click the OK button.
 - Type the following command to map a drive assigning drive letter manually and press Enter:
 - New-PSDrive -Name "E" -Root "\\DEVICE-NAME-OR-IP\SHARED-FOLDER" -Persist -PSProvider "FileSystem" -Credential $cred
 - In the command, replace DRIVER-LETTER with the drive letter not already in use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the share.
 - For example, this command maps the ShareFiles folder to the computer with the “X” drive letter:
 - New-PSDrive -Name "X" -Root "\\vm-10v21h2\ShareFiles" -Persist -PSProvider "FileSystem" -Credential $cred

 
After you complete the steps, the command will map the shared folder with your specified credentials.
 
Type the following command to create a variable to store the account information and press Enter:
 
$cred = Get-Credential -Credential USERNAME
 
Confirm the account password.
 
Type the following command to map a drive assigning drive letter manually and press Enter:
 
New-PSDrive -Name "E" -Root "\\DEVICE-NAME-OR-IP\SHARED-FOLDER" -Persist -PSProvider "FileSystem" -Credential $cred
 
In the command, replace DRIVER-LETTER with the drive letter not already in use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the share.
 
For example, this command maps the ShareFiles folder to the computer with the “X” drive letter:
 
New-PSDrive -Name "X" -Root "\\vm-10v21h2\ShareFiles" -Persist -PSProvider "FileSystem" -Credential $cred
 
When you try to connect using credentials, you will always get prompted to provide a password manually. If you want to avoid this step, you could store the password in an encrypted file on the computer and query that file using PowerShell. Or you can speed up the process by holding the remote host account name and password in Credential Manager and then using the same command without the -Crendtial option like this: New-PSDrive -Name "E" -Root "\\vm-beta\ShareOne" -Persist -PSProvider "FileSystem"
 
You can create a new entry in Credential Manager using this command: cmdkey /add:pcname /user:network\username /pass:password
 
## Disconnect mapped network drive on Windows 11 using PowerShell
 
To disconnect and remove a mapped network drive with PowerShell on Windows 11, use these steps:
 
- Open Start.
 - Search for PowerShell and click the top result to open the console.
 - Type the following command to view all the mapped drives and press Enter:
 - Get-PSDrive -PSProvider "FileSystem"
 - Type the following command to disconnect the mapped network drive and press Enter:
 - Remove-PSDrive -Name DRIVE-LETTER
 - In the command, replace DRIVE-LETTER for the drive letter of the mapping.
 - For example, this command disconnects the “X” drive:
 - Remove-PSDrive -Name X
 - (Optional) Type the following command to disconnect multiple mappings and press Enter:
 - Get-PSDrive DRIVER-LETTER-1, DRIVE-LETTER-2 | Remove-PSDrive
 - In the command, replace DRIVER-LETTER-1 and DRIVE-LETTER-2 with the drive letters you want to disconnect.
 - For example, this command disconnects the “E” and “F” drives:
 - Get-PSDrive E, F | Remove-PSDrive

 
Once you complete the steps, the network mapping will no longer be available on the computer.
 
Type the following command to view all the mapped drives and press Enter:
 
Get-PSDrive -PSProvider "FileSystem"
 
Type the following command to disconnect the mapped network drive and press Enter:
 
Remove-PSDrive -Name DRIVE-LETTER
 
In the command, replace DRIVE-LETTER for the drive letter of the mapping.
 
For example, this command disconnects the “X” drive:
 
Remove-PSDrive -Name X
 
(Optional) Type the following command to disconnect multiple mappings and press Enter:
 
Get-PSDrive DRIVER-LETTER-1, DRIVE-LETTER-2 | Remove-PSDrive
 
In the command, replace DRIVER-LETTER-1 and DRIVE-LETTER-2 with the drive letters you want to disconnect.
 
For example, this command disconnects the “E” and “F” drives:
 
Get-PSDrive E, F | Remove-PSDrive
 
## Map network drive on Windows 11 with Command Prompt
 
To map a shared folder with Command Prompt on Windows 11, use these steps:
 
- Open Start.
 - Search for Command Prompt and click the top result to open the console.
 - Quick tip: Do not run the terminal as an administrator to allow the mount to appear in File Explorer.
 - Type the following command to map a drive assigning drive letter manually and press Enter:
 - net use Z: \\DEVICE-NAME-OR-IP\SHARED-FOLDER
 - In the command, replace “Z” with the drive letter not already in use. Then replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the share.
 - For example, this command maps the ShareFiles folder to the computer with the “Z” drive letter:
 - net use Z: \\vm-10v21h2\ShareFiles
 - Type the following command to map a drive assigning drive letter automatically and press Enter:
 - net use * \\DEVICE-NAME-OR-IP\SHARED-FOLDER
 - In the command, the (*) is the option that automatically assigns a random available drive letter. Then replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the share.
 - For example, this command maps the ShareOne folder to the computer:
 - net use * \\vm-10v21h2\ShareFiles
 - Type the following command to map a drive providing authentication details and press Enter:
 - net use Z: \\DEVICE-NAME-OR-IP\SHARED-FOLDER PASSWORD /user:USERNAME /persistent:yes
 - In the command, replace “Z” with the drive letter not already in use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the share. The PASSWORD and USERNAME have to be replaced with the credentials to authenticate with the remote machine. The “persistent” option allows the folder to stay mapped after reboot.
 - For example, this command maps the ShareFiles folder providing the user credentials and making the mapping persistent:
 - net use Z: \\vm-10v21h2\ShareFiles password /user:admin /persistent:yes

 
Once you complete the steps, the network shared folder will map on the device, appearing in File Explorer.
 
Search for Command Prompt and click the top result to open the console. 
 
net use Z: \\DEVICE-NAME-OR-IP\SHARED-FOLDER
 
In the command, replace “Z” with the drive letter not already in use. Then replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the share.
 
net use Z: \\vm-10v21h2\ShareFiles
 
Type the following command to map a drive assigning drive letter automatically and press Enter:
 
net use * \\DEVICE-NAME-OR-IP\SHARED-FOLDER
 
In the command, the (*) is the option that automatically assigns a random available drive letter. Then replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the share.
 
For example, this command maps the ShareOne folder to the computer:
 
net use * \\vm-10v21h2\ShareFiles
 
Type the following command to map a drive providing authentication details and press Enter:
 
net use Z: \\DEVICE-NAME-OR-IP\SHARED-FOLDER PASSWORD /user:USERNAME /persistent:yes
 
In the command, replace “Z” with the drive letter not already in use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the share. The PASSWORD and USERNAME have to be replaced with the credentials to authenticate with the remote machine. The “persistent” option allows the folder to stay mapped after reboot.
 
For example, this command maps the ShareFiles folder providing the user credentials and making the mapping persistent:
 
net use Z: \\vm-10v21h2\ShareFiles password /user:admin /persistent:yes
 
## Disconnect mapped network drive on Windows 11 with Command Prompt
 
To disconnect a network drive on Windows 11 with commands, use these steps:
 
- Open Start.
 - Search for Command Prompt and click the top result to open the console.
 - Type the following command to disconnect a mapped network drive and press Enter:
 - net use z: /Delete
 - In the command, replace “Z” for the drive letter of the map you want to remove.
 - (Optional) Type the following command to disconnect all the mapped network drives and press Enter:
 - net use * /Delete

 
After you complete the steps, the mapped drives will be disconnected and no longer accessible from File Explorer.
 
Search for Command Prompt and click the top result to open the console.
 
Type the following command to disconnect a mapped network drive and press Enter:
 
net use z: /Delete


 
In the command, replace “Z” for the drive letter of the map you want to remove.
 
(Optional) Type the following command to disconnect all the mapped network drives and press Enter:
 
net use * /Delete






