---
title: "You won't believe the time-saving trick to map network drive on Windows 10 using Command Prompt!"
ShowToc: true 
date: "2023-04-11"
author: "Lyle Sullivan"
---
*****
- Introduction -

As technology evolves, our daily tasks become more effortless and less time consuming. Mapping network drives is one of those tasks that often take up a considerable amount of time. Fortunately, there is a trick that can save you time if you use Windows 10!

In this article, we will show you how to easily map a network drive using Command Prompt on Windows 10, saving you valuable time and effort.

- The old way of mapping a network drive -

The traditional method of mapping a network drive involves using File Explorer, a process that can be time-consuming and complex. To do this, you would have to open Windows Explorer, and navigate to This PC or My Computer. From there, you would search for the map network drive option, which can often be hidden, and then continue with the process.

If you need to map the same drive to multiple computers, doing it manually can take up a significant amount of time. Thankfully, there is an easier, quicker, and more efficient way!

- The shortcut method: Mapping a network drive using Command Prompt -

Command Prompt is a powerful tool in Windows 10 that can save you time and effort. It’s an old-school command-line interface that’s virtually identical to the original MS-DOS, but it’s still in use today.

To map a network drive using Command Prompt, follow these simple steps:

Step 1: Open Command Prompt. Press the Windows key + R, type cmd into the Run box, and click OK.

Step 2: Type the following command into Command Prompt: net use * "\\[computer name]\[shared folder name]" /user:[username]

Make sure to replace [computer name] with the name of the computer that you want to connect, [shared folder name] with the name of the shared folder that you want to access, and [username] with your username.

Step 3: Press Enter. You will be prompted to enter the password for the shared folder you are connecting to. After you input the correct password, the network drive will be successfully mapped.

- Conclusion -

Mapping a network drive can be time-consuming, but with Command Prompt, it's much easier and quicker. In just a few simple steps, your network drive will be mapped, saving you valuable time and effort.

So next time don’t waste your time clicking through different folder hierarchy, try this shortcut using Command Prompt and see the difference for yourself.

{{< youtube Jfvg3CS1X3A >}} 



On Windows 10, you can quickly map a network drive in several ways, including from Command Prompt when you prefer to use command lines or create a script to access files stored on another computer.
 
When connecting to a network drive, Windows 10 essentially creates a “shortcut” that points to the shared folder with a drive letter and the username and password to access its content. Once a drive is mapped, it will appear on “This PC” under “Network locations” to quickly access files stored on another computer from File Explorer.
 
This guide will teach you the steps to use Command Prompt to map a network drive on Windows 10 and how to disconnect when you no longer need access to the shared folder.
 
- Map network drive on Windows 10 with Command Prompt
 - Disconnect mapped network drive on Windows 10 with Command Prompt

 
## Map network drive on Windows 10 from Command Prompt
 
To use the net command to map a shared folder as a drive, use these steps:
 
- Open Start on Windows 10.
 - Search for Command Prompt and click the top result to open the console.
 - Quick note: If you run the command as an administrator, the drive may not mount correctly and won’t appear in File Explorer. As a result, run the command as a standard user.
 - Type the following command to map a drive assigning drive letter manually and press Enter:
 - net use Z: \\DEVICE-NAME-OR-IP\SHARED-FOLDER
 - In the command, replace “Z” with the drive letter not already in use you want to use. Then replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the shared. For example, this command maps the ShareOne folder to the computer with the “Z” drive letter:
 - net use Z: \\vm-beta\ShareOne
 - Type the following command to map a drive assigning drive letter automatically and press Enter:
 - net use * \\DEVICE-NAME-OR-IP\SHARED-FOLDER
 - In the command, the (*) is the option that allows the system to assign any drive letter that is not already in use. Then replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the shared. For example, this command maps the ShareOne folder to the computer:
 - net use * \\vm-beta\ShareOne
 - Type the following command to map a drive providing authentication details and press Enter:
 - net use Z: \\DEVICE-NAME-OR-IP\SHARED-FOLDER PASSWORD /user:USERNAME /persistent:yes
 - In the command, replace “Z” with the drive letter not already in use you want to use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the shared. The PASSWORD and USERNAME have to be replaced with the credentials to authenticate with the remote machine. The “persistent” option allows the folder to stay mapped after reboot. For example, this command maps the ShareOne folder providing the user credentials and making the mapping persistent:
 - net use Z: \\vm-beta\ShareOne password /user:admin /persistent:yes

 
Once you complete the steps, the network folder will map on the device and appear in File Explorer.
 
Open Start on Windows 10.
 
Search for Command Prompt and click the top result to open the console.
 
Type the following command to map a drive assigning drive letter manually and press Enter:
 
net use Z: \\DEVICE-NAME-OR-IP\SHARED-FOLDER
 
In the command, replace “Z” with the drive letter not already in use you want to use. Then replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the shared. For example, this command maps the ShareOne folder to the computer with the “Z” drive letter:
 
net use Z: \\vm-beta\ShareOne
 

 
Type the following command to map a drive assigning drive letter automatically and press Enter:
 
net use * \\DEVICE-NAME-OR-IP\SHARED-FOLDER
 
In the command, the (*) is the option that allows the system to assign any drive letter that is not already in use. Then replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the shared. For example, this command maps the ShareOne folder to the computer:
 
net use * \\vm-beta\ShareOne
 
Type the following command to map a drive providing authentication details and press Enter:
 
net use Z: \\DEVICE-NAME-OR-IP\SHARED-FOLDER PASSWORD /user:USERNAME /persistent:yes
 
In the command, replace “Z” with the drive letter not already in use you want to use. Then change DEVICE-NAME-OR-IP and SHARED-FOLDER for the computer name or IP address of the device hosting the shared folder and the name of the shared. The PASSWORD and USERNAME have to be replaced with the credentials to authenticate with the remote machine. The “persistent” option allows the folder to stay mapped after reboot. For example, this command maps the ShareOne folder providing the user credentials and making the mapping persistent:
 
net use Z: \\vm-beta\ShareOne password /user:admin /persistent:yes
 
## Disconnect mapped network drive on Windows 10 from Command Prompt
 
To disconnect a network drive on Windows 10, use these steps:
 
- Open Start.
 - Search for Command Prompt and click the top result to open the console.
 - Type the following command to disconnect a mapped network drive and press Enter:
 - net use z: /Delete
 - In the command, replace “Z” with the drive letter of the map you want to remove.
 - Type the following command to disconnect all the mapped network drives and press Enter:
 - net use * /Delete

 
After you complete the steps, the mapped drives will be disconnected and no longer accessible from File Explorer.
 
Open Start.
 
Type the following command to disconnect a mapped network drive and press Enter:
 
net use z: /Delete


 
In the command, replace “Z” with the drive letter of the map you want to remove.
 
Type the following command to disconnect all the mapped network drives and press Enter:
 
net use * /Delete


 
While we focus this guide on Windows 10, you can use these steps on Windows 8.1, 7, and earlier versions. Use these instructions if you want to use File Explorer to complete this task.




