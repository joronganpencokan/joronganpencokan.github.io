---
title: "You'll Never Believe How Easy it is to Manage Windows Device Drivers with this Command Prompt Trick!"
ShowToc: true 
date: "2023-07-06"
author: "Kevin Kaspar"
---
*****
# You'll Never Believe How Easy it is to Manage Windows Device Drivers with this Command Prompt Trick!

Windows operating systems have a built-in feature for managing device drivers. However, accessing this feature is not always user-friendly, and the process can be time-consuming. Luckily, there is a simple command prompt trick that makes managing device drivers in Windows a breeze. In this article, I will show you how to use this trick and how it can streamline your device management process.

## The Challenge of Managing Device Drivers in Windows

Device drivers are essential software components that enable communication between hardware devices and the operating system. Windows typically installs drivers for hardware devices automatically. However, sometimes, the installed drivers might not work correctly or might be outdated, requiring an update or replacement.

To manage device drivers in Windows, you need to access the Device Manager, a built-in tool that displays all installed hardware devices and their relevant drivers. Opening the Device Manager requires several clicks, which can be time-consuming, especially when you want to update drivers regularly.

## The Command Prompt Trick to Manage Device Drivers in Windows

Fortunately, there is an easy command prompt trick that allows you to access the Device Manager quickly. Here's how to do it:

1. Press the Windows key + X to open the Quick Link menu.
2. Choose Command Prompt (Admin) or Windows PowerShell (Admin).
3. Type devmgmt.msc and press Enter.

This command opens the Device Manager directly, without having to navigate through several menu options. You can now view all installed hardware devices and their corresponding drivers.

## The Benefits of Using this Command Prompt Trick

The command prompt trick for accessing the Device Manager has several benefits, including:

- Saving time: With this trick, you can open the Device Manager in just a few clicks, without having to navigate through several menus.

- Easy access: The command prompt trick is user-friendly, and you don't need any technical expertise to use it.

- Advanced management: The Device Manager allows you to perform several functions, including updating, disabling, or uninstalling drivers.

This command prompt trick also allows you to manage device drivers remotely, making it particularly useful for IT professionals who manage several Windows devices.

## Conclusion

In conclusion, managing device drivers in Windows can be time-consuming and cumbersome, particularly when dealing with several devices. However, the command prompt trick outlined in this article makes it incredibly easy to access the Device Manager in just a few clicks. This trick can save you time and simplify your device management tasks, particularly if you work in IT or manage several Windows devices regularly. Why not give it a try and see how it can streamline your device management process!

{{< youtube Fg03d5A-0gY >}} 



In Windows, managing your hardware devices can be easily done via the Device Manager section. However, if you are in a server environment or if you want to control device drivers using the command line, then DevCon is a good alternative for the regular Device Manager.
 
DevCon is a part of Windows Driver Kit and is a command line utility which can be used to quickly disable, enable, install, remove, scan and list all the hardware devices in a local or network computer. 
 
## Using DevCon
 
DevCon is available for free and can be downloaded from the Microsoft website. Once downloaded, extract the executable and place it somewhere in the C drive so that you can reach it easily in the command prompt. For instance, I’ve placed the extracted files in a folder named “devcon” in my C drive.
 

 
Now open up the Command Prompt as the administrator. To do that, search for the command prompt in the Start menu, right click on it and select the option “Run as administrator.” If you are using Windows 8, simply select the option “Command Prompt (Admin)” from the power user menu (Win + X).
 
Once you are in the command prompt, navigate to either the 32-bit (i386) or the 64-bit (ia64) folder in the “devcon” folder using the command below. If you have placed the DevCon executable somewhere else then change the command accordingly.
 
Now, if you want to know the syntax, different commands and arguments used by the Devcon utility, use the command below to get some help.
 
To get a list of the devices, you can use the find command with the wild card entries. Since DevCon is also used over the network, you need to specify the computer name to get a list of the devices. You can easily find your Windows computer name in the “System Properties” window. For instance, I used the following command to get the details about my CD-ROM. Don’t forget to replace the computer name and the device name. Moreover, you can always replace the “deviceName” with the hardware IDs.
 
Alternatively, you can also use the Hardware IDs command to get a list of all the devices. To get a list of all the hardware devices, use the following command.
 
If want to trim down the list, use the command with the wild card entries.
 
Now to get the status of a device, use the below command. To make your life much easier, you can either use the hardware IDs or the names with wildcard entries like I did. This command outputs the device name and status of the device.
 
To disable a device using the DevCon utility, you can use the below command. Again, use the wild card entries if necessary, but be careful as you might disable other devices that you don’t intend to.
 
To re-enable the device, use the command below. The command does nothing more than replacing “disable” with the word “enable.”
 
If you want to scan for any new devices on your computer, then you can use the command below. It is just like the “Scan for new hardware” button in your Device Manager.
 
To install a certain driver using the DevCon utility, you need the INF file which comes bundled with the driver files. Now, to install a device driver, use the following command. Don’t forget to replace “Path to INF file” with the actual path and the “hardwareID” with the actual hardware ID. In case you are wondering, the switch /r is an argument to restart the computer once the process is finished.
 
To update a device driver, use the following command. While entering the hardware ID’s, you can use the wildcards, but be careful while using them.
 
Now to remove a hardware device completely, use the below command. Just like in any other command, you can use the wildcards but it is not at all recommended for this command.
 
That’s all for now, and it is that simple to use the DevCon command-line utility to manage your hardware drivers. The commands shared above are helpful in almost all the basic situations. But if you want to know more, Microsoft Library has an excellent documentation detailing each and every command regarding the DevCon utility. So don’t forget to give it a try.
 
Hopefully that helps, and do comment below sharing your thoughts and experiences about using DevCon to manage your hardware drivers.
 
Vamsi is a tech and WordPress geek who enjoys writing how-to guides and messing with his computer and software in general. When not writing for MTE, he writes for he shares tips, tricks, and lifehacks on his own blog Stugon.
 
Our latest tutorials delivered straight to your inbox




