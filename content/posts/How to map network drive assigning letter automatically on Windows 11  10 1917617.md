---
title: "Unlock the Secret Trick to Automatically Map Network Drives on Windows 11 and 10!"
ShowToc: true 
date: "2023-04-03"
author: "Phillip Carrion"
---
*****
# Unlock the Secret Trick to Automatically Map Network Drives on Windows 11 and 10!

Many Windows users have difficulty in mapping network drives when booting up their system. This is because the network drives are not connected automatically, and they have to map them manually again and again. However, there is a secret trick to automatically map network drives on Windows 11 and 10.

# What is a network drive?

A network drive is a location on a remote computer that you can access from your computer. You can map the network drives to your computer for easier access. Network drives are helpful when you need to access files, folders, or resources shared on another computer or server.

# The Problem with Manually Mapping Network Drives

When you boot up your computer, Windows may not have the necessary network information to access the drives. This causes the mapped network drives to fail, and you have to manually map them every time you start your computer.

# The Solution

You can configure your Windows operating system to map the network drives automatically. The steps to do this are as follows:

1. Press "Windows Key + R" and type "gpedit.msc" in the Run box and hit "Enter". This will open the Local Group Policy Editor.

2. Navigate to "Computer Configuration > Administrative Templates > System > Logon".

3. Double-click on "Always wait for the network at computer startup and logon" and select "Enabled".

4. Click "OK" to save the changes.

5. Next, navigate to "User Configuration > Preferences > Windows Settings > Drive Maps".

6. Right-click in the empty space and select "New > Mapped Drive".

7. In the "General" tab, select the drive letter you want to use for the drive and enter the path to the folder you want to map.

8. In the "Common" tab, select "Run in logged-on user's security context" and "Reconnect" options.

9. Click "OK" to save the changes.

10. Finally, close the Group Policy Editor and restart your computer.

After following these steps, your network drives will automatically map when you boot up your computer. This will save you time and hassle, and you will be able to access your files and folders quickly and easily.

# Conclusion

Mapping network drives is a useful feature for Windows users who need to access shared files and resources on another computer or server. However, the manual process can be tiresome and time-consuming, especially when you need to map the same network drives every time you start your computer.

By following the steps outlined in this article, you can automate the process of mapping network drives on Windows 11 and 10. With this trick, you can save time and hassle, and access your files and folders quickly and easily.

{{< youtube Vw6uXMGsxZc >}} 



On Windows 11 (or Windows 10), you can use the “net use” command to quickly map a network drive to access files on a shared folder located on a server or another computer in the network. The only caveat is that you usually have to specify a driver letter to make the drive available in File Explorer. However, if the letter is already in use, the drive will not connect. 
 
If you want to avoid mapping problems, you can use a specific command option that will automatically assign a drive letter.
 
This guide will teach you the steps to use Command Prompt to map a network drive without specifying a drive letter.
 
## Map network drive assigning letter automatically on Windows 11, 10
 
To map a network drive on Windows 11 or 10 by assigning a drive letter automatically, use these steps:
 
- Open Start on Windows 11.
 - Search for Command Prompt and click the top result to open the app.
 - Quick note: If you run the command as an administrator, the drive may not mount correctly, and it won’t appear in File Explorer. As a result, run the command as a standard user.
 - Type the following command to map the network drive using the next available drive letter and press Enter:
 - net use * \\DEVICE-NAME-OR-IP\SHARED-FOLDER
 - In the command, the (*) is the option that allows the system to assign any drive letter that is not already in use. Remember to replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the name of the computer name or IP address of the device hosting the shared folder and the name of the shared.
 - For example, this command maps the ShareOne folder to the computer:
 - net use * \\vm-beta\ShareOne
 - (Optional) Type the following command to map the network drive using the next available drive letter providing sign-in credentials and press Enter:
 - net use * \\DEVICE-NAME-OR-IP\SHARED-FOLDER PASSWORD /user:USERNAME /persistent:yes
 - In the command, the (*) is the option that allows the system to assign any drive letter that is not already in use. Remember to replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the name of the computer name or IP address of the device hosting the shared folder and the name of the shared. The PASSWORD and USERNAME have to be replaced with the credentials to authenticate with the remote device. The “persistent” option allows the folder to stay mapped after reboot. For example, this command maps the ShareOne folder providing the user credentials and making the mapping persistent:
 - net use * \\vm-beta\ShareOne password /user:admin /persistent:yes
 - 

 
Once you complete the steps, the network drive will automatically map with the next available drive letter, and the command will let you know the letter the new map is using.
 
Open Start on Windows 11.
 
Search for Command Prompt and click the top result to open the app.
 
Type the following command to map the network drive using the next available drive letter and press Enter:
 
net use * \\DEVICE-NAME-OR-IP\SHARED-FOLDER
 
In the command, the (*) is the option that allows the system to assign any drive letter that is not already in use. Remember to replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the name of the computer name or IP address of the device hosting the shared folder and the name of the shared.
 
For example, this command maps the ShareOne folder to the computer:
 
net use * \\vm-beta\ShareOne
 

 
(Optional) Type the following command to map the network drive using the next available drive letter providing sign-in credentials and press Enter:
 
net use * \\DEVICE-NAME-OR-IP\SHARED-FOLDER PASSWORD /user:USERNAME /persistent:yes
 
In the command, the (*) is the option that allows the system to assign any drive letter that is not already in use. Remember to replace DEVICE-NAME-OR-IP and SHARED-FOLDER for the name of the computer name or IP address of the device hosting the shared folder and the name of the shared. The PASSWORD and USERNAME have to be replaced with the credentials to authenticate with the remote device. The “persistent” option allows the folder to stay mapped after reboot. For example, this command maps the ShareOne folder providing the user credentials and making the mapping persistent:
 
net use * \\vm-beta\ShareOne password /user:admin /persistent:yes
 
 
 
Using the net use command, you can disconnect, make mapped network drives persistent, connect using different credentials, and more. Here you can learn more about how to use the map command on Windows 10.
 
This guide focuses on Windows 10 and 11, but you can use the same command on Windows 8.1, Windows 7, and previous versions. 




