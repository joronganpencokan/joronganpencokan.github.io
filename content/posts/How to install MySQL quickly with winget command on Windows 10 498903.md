---
title: "Unlock Lightning-Fast Mysql Installations on Windows 10 with This Game-Changing Winget Command!"
ShowToc: true 
date: "2023-04-15"
author: "Dustin Smith"
---
*****
# Unlock Lightning-Fast Mysql Installations on Windows 10 with This Game-Changing Winget Command!

Have you been struggling with slow and cumbersome MySQL installations on your Windows 10 machine? Well, it's time to put an end to that with the help of a powerful new tool called Winget.

Winget is a package manager for Windows that allows you to easily download and install all kinds of software from the command line. And with the help of a few simple commands, you can now get MySQL up and running on your Windows 10 machine in a matter of minutes, with lightning-fast speeds that will blow your mind.

Here's how it works:

First, you need to make sure that Winget is installed on your system. If you're running Windows 10 version 1809 or later, you should already have it installed. Otherwise, you can download it from Microsoft's official Winget repository.

Once you have Winget up and running, simply open up a command prompt and type:

```
winget install --id=Oracle.MySQL
```

This will initiate the installation of MySQL, and within minutes, you'll have a fully functional MySQL server running on your machine.

The best part? Because Winget is optimized for speed and efficiency, you'll notice a significant improvement in the speed and performance of your MySQL installations. No more waiting around for hours for your database to be up and running – with Winget, everything is lightning-fast and hassle-free.

But that's not all. Winget also makes it incredibly easy to manage and update your MySQL installations. You can simply run the following command to update MySQL to the latest version:

```
winget upgrade --id=Oracle.MySQL
```

And just like that, your MySQL installation will be up-to-date and running at peak performance once again.

In conclusion, if you're tired of slow and cumbersome MySQL installations on your Windows 10 machine, it's time to switch to Winget. With its lightning-fast speeds and easy installation and management process, it's a game-changer for any database administrator or developer. So why wait? Give it a try today, and unlock the full potential of your MySQL installations on Windows 10.

{{< youtube c9oxk9W7FkU >}} 



- To install MySQL with on Windows 10 use the winget install Oracle.MySQL command.
 - To uninstall MySQL, then use the winget uninstall Oracle.MySQL command.

 
If you need to work MySQL to create and manage databases for web or application projects, it is no longer necessary to go through all the steps to find the installer and run the setup manually. You can now install it quickly with the Windows Package Manager (winget).
 
On Windows 10, winget a command-line tool from Microsoft designed to save time and frustration searching, downloading, installing, updating, and configuring applications. The tool is available for developers, but anyone can use it to install applications quickly with one command through Command Prompt or Windows Terminal.
 
The command-line tool should already be available on your device, running version 1809 or higher. If it is not, you may need to install the App Installer app from the Microsoft Store.
 
In this guide, you will learn the steps to install and uninstall the Oracle MySQL database application on Windows 10.
 
- Install MySQL using Windows Package Manager
 - Uninstall MySQL using Windows Package Manager

 
## Install MySQL using Windows Package Manager
 
To install MySQL with the winget command, use these steps:
 
- Open Start.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - (Optional) Type the following command to search for the name of the application and press Enter:
 - winget search mysql
 - Quick note: While the search command is not required, the install query must match the ID, name, or moniker of the package, which can change at any time. So, it’s a good practice to search the application to execute the correct install command.
 - Type the following command to install MySQL on Windows 10 with winget and press Enter:
 - winget install Oracle.MySQL
 - winget install command

 
Once you complete the steps, the Windows Package Manager will download and install the Oracle MySQL database application on your computer. After the installation, you can launch the community version of MySQL from the Start menu to complete the setup.
 
Open Start.
 
Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 
(Optional) Type the following command to search for the name of the application and press Enter:
 
winget search mysql
 
Type the following command to install MySQL on Windows 10 with winget and press Enter:
 
winget install Oracle.MySQL
 
winget install command

 
## Uninstall MySQL using Windows Package Manager
 
If you no longer need the application, it’s also possible to remove it using the winget command. However, at the time of this writing, the option is available in the beta, and you may need to enable it manually before you can uninstall the app. Of course, you can always get rid of the database application from the “Apps & features” settings.
 
To uninstall an app with the Windows Package Manager tool, use these steps:
 
- Open Start on Windows 10.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to confirm whether the uninstall option is enabled and press Enter:
 - winget features
 - winget uninstall enabled
 - Quick note: If the feature is disabled, use these instructions to enable it and continue with the steps below.
 - Type the following command to determine the name of the application with the Windows Package Manager and press Enter:
 - winget uninstall
 - winget install apps list
 - Type the following command to uninstall an app with winget and press Enter:
 - winget uninstall Oracle.MySQL
 - winget uninstall command

 
After you complete the steps, the app will be removed from the computer.
 
Open Start on Windows 10.
 
Type the following command to confirm whether the uninstall option is enabled and press Enter:
 
winget features
 
Type the following command to determine the name of the application with the Windows Package Manager and press Enter:
 
winget uninstall
 
winget install apps list

 
Type the following command to uninstall an app with winget and press Enter:
 
winget uninstall Oracle.MySQL
 
winget uninstall command





