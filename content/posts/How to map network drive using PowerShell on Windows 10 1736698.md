---
title: "You Won't Believe How Easy it is to Map a Network Drive with Powershell on Windows 10!"
ShowToc: true 
date: "2023-04-05"
author: "Nickie Murders"
---
*****
+++

title = "You Won't Believe How Easy it is to Map a Network Drive with Powershell on Windows 10!"

date = "2021-07-02"

author = "OpenAI GPT-3"

tags = ["Windows 10", "Powershell", "Network Drive"]

+++

As Windows 10 is becoming increasingly prevalent in the workplace, it's more important than ever to know how to map a network drive. Mapping a network drive allows you to access shared folders and files on other machines connected to the same network. Fortunately, mapping a network drive on Windows 10 is incredibly easy - especially if you use Powershell. In this article, we'll take you through the process of using Powershell to map a network drive step by step.

First, it's important to note that you'll need to be connected to the network in question in order to map a network drive. Once you're connected, open up Powershell. You can do this by typing "powershell" into the search bar beside the Windows icon at the bottom left of your desktop.

Next, type the following command into Powershell:

```
New-PSDrive -Name X -PSProvider FileSystem -Root \\server\share -Persist
```

In this example, we're assuming that the name of the network drive you'd like to map is X. You can change this to whatever you'd like, as long as it's not already in use on your computer.

The -PSProvider parameter tells Powershell what type of drive you're creating. In this case, we're creating a drive that's connected to a file system. The -Root parameter tells Powershell where on the network the files you'd like to access are located. In this example, we're assuming that the files are located on a server with the name "server", and that they're in a folder called "share".

Finally, the -Persist parameter tells Powershell to make the mapped network drive permanent. This means that the drive will still be mapped even if you restart your computer.

Once you've typed in the command, press enter. If all goes well, Powershell should respond with a prompt confirming that the network drive has been created. You should now see the network drive in your Windows Explorer, and you can access it just like you would any other drive on your computer.

And that's it! As you can see, mapping a network drive using Powershell is incredibly easy. Whether you're accessing files from other computers on your work network, or you just want to make sure you always have access to your family's shared files, mapping a network drive can be incredibly useful. And with Powershell, you can do it in just a few simple steps.

{{< youtube dOHbDtSUuhk >}} 



Windows 10 provides multiple ways to map a network drive on your computer, including using PowerShell, which can come in handy when creating a script or when you prefer using a command-line interface.
 
When you use PowerShell (or any other methods, such as Command Prompt or File Explorer) to map a network-shared folder, the process will create a pointer to the destination folder that will appear in File Explorer as a drive with the letter you assigned it.
 
This guide will teach you how to use PowerShell to map a network drive on Windows 10. In addition, we will outline the steps to disconnect the mapping when it is no longer needed.
 
- Map network drive on PowerShell
 - Map network drive with credentials on PowerShell
 - Disconnect mapped network drive on PowerShell

 
## Map network drive on PowerShell
 
To map a network drive with PowerShell, use these steps:
 
- Open Start on Windows 10.
 - Search for PowerShell and click the top result to open the console.
 - Type the following command to map a drive assigning letter manually and press Enter:
 - New-PSDrive -Name "DRIVER-LETTER" -PSProvider "FileSystem" -Root "\\DEVICE-NAME-OR-IP\SHARED-FOLDER" -Persist
 - In the command, replace DRIVER-LETTER with the drive letter not already in use you want to use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the name of the computer name or IP address of the device hosting the shared folder and the name of the shared. For example, this command maps the ShareOne folder to the computer with the “E” drive letter:
 - New-PSDrive -Name "E" -PSProvider "FileSystem" -Root "\\vm-beta\ShareOne" -Persist

 
Once you complete the steps, the network shared folder will map on the computer and appear in File Explorer.
 
Open Start on Windows 10.
 
Search for PowerShell and click the top result to open the console.
 
Type the following command to map a drive assigning letter manually and press Enter:
 
New-PSDrive -Name "DRIVER-LETTER" -PSProvider "FileSystem" -Root "\\DEVICE-NAME-OR-IP\SHARED-FOLDER" -Persist
 
In the command, replace DRIVER-LETTER with the drive letter not already in use you want to use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the name of the computer name or IP address of the device hosting the shared folder and the name of the shared. For example, this command maps the ShareOne folder to the computer with the “E” drive letter:
 
New-PSDrive -Name "E" -PSProvider "FileSystem" -Root "\\vm-beta\ShareOne" -Persist
 

 
## Map network drive with credentials on PowerShell
 
To map a network drive providing the account name and password, use these steps:
 
- Open Start.
 - Search for PowerShell and click the top result to open the console.
 - Type the following command to create a variable with the proper credentials, and press Enter:
 - $cred = Get-Credential -Credential USERNAME
 - Quick tip: If you are mapping a drive in Active Directory, remember to use the network name like this: network\admin to specify the account information.
 - Confirm your account password.
 - Click the OK button.
 - Type the following command to map a drive assigning drive letter manually and press Enter:
 - New-PSDrive -Name "E" -Root "\\DEVICE-NAME-OR-IP\SHARED-FOLDER" -Persist -PSProvider "FileSystem" -Credential $cred
 - In the command, replace DRIVER-LETTER with the drive letter not already in use you want to use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the name of the computer name or IP address of the device hosting the shared folder and the name of the shared. For example, this command maps the ShareOne folder to the computer with the “E” drive letter:
 - New-PSDrive -Name "E" -Root "\\vm-beta\ShareOne" -Persist -PSProvider "FileSystem" -Credential $cred

 
After you complete the steps, the command will authenticate and map the shared folder as a drive on Windows 10.
 
Open Start.
 
Type the following command to create a variable with the proper credentials, and press Enter:
 
$cred = Get-Credential -Credential USERNAME
 
Confirm your account password.
 
Click the OK button.
 
Type the following command to map a drive assigning drive letter manually and press Enter:
 
New-PSDrive -Name "E" -Root "\\DEVICE-NAME-OR-IP\SHARED-FOLDER" -Persist -PSProvider "FileSystem" -Credential $cred
 
New-PSDrive -Name "E" -Root "\\vm-beta\ShareOne" -Persist -PSProvider "FileSystem" -Credential $cred
 
When connecting using credentials, you will always get prompted to provide a password manually. If you want to avoid this step, you could store the password in an encrypted file on the computer and query that file using PowerShell. Or you can speed up the process by storing the remote host account name and password in Credential Manager and then use the same command without the -Crendtial option like this: New-PSDrive -Name "E" -Root "\\vm-beta\ShareOne" -Persist -PSProvider "FileSystem"
 
You can create a new entry in Credential Manager using this command: cmdkey /add:pcname /user:network\username /pass:password
 
## Disconnect mapped network drive on PowerShell
 
To disconnect and remove a mapped network drive with PowerShell, use these steps:
 
- Open Start.
 - Search for PowerShell and click the top result to open the console.
 - Type the following command to view all the mapped drives and press Enter:
 - Get-PSDrive -PSProvider "FileSystem"
 - Type the following command to disconnect the mapped network drive and press Enter:
 - Remove-PSDrive -Name DRIVE-LETTER
 - In the command, replace DRIVE-LETTER with the drive letter of the mapping. For example, this command disconnects the “E” drive:
 - Remove-PSDrive -Name E
 - (Optional) Type the following command to disconnect multiple mappings and press Enter:
 - Get-PSDrive DRIVER-LETTER-1, DRIVE-LETTER-2 | Remove-PSDrive
 - In the command, replace DRIVER-LETTER-1 and DRIVE-LETTER-2 with the drive letters you want to disconnect. For example, this command disconnects the “E” and “F” drives:
 - Get-PSDrive E, F | Remove-PSDrive

 
Once you complete the steps, the drive mapping will be removed from the computer.
 
Type the following command to view all the mapped drives and press Enter:
 
Get-PSDrive -PSProvider "FileSystem"
 
Type the following command to disconnect the mapped network drive and press Enter:
 
Remove-PSDrive -Name DRIVE-LETTER
 
In the command, replace DRIVE-LETTER with the drive letter of the mapping. For example, this command disconnects the “E” drive:
 
Remove-PSDrive -Name E
 
(Optional) Type the following command to disconnect multiple mappings and press Enter:
 
Get-PSDrive DRIVER-LETTER-1, DRIVE-LETTER-2 | Remove-PSDrive
 
In the command, replace DRIVER-LETTER-1 and DRIVE-LETTER-2 with the drive letters you want to disconnect. For example, this command disconnects the “E” and “F” drives:
 
Get-PSDrive E, F | Remove-PSDrive




