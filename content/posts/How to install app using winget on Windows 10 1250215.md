---
title: "You won't believe how easy it is to install apps on Windows 10 using Winget!"
ShowToc: true 
date: "2023-06-07"
author: "Stephen Rodriguez"
---
*****
Title: You Won't Believe How Easy It Is to Install Apps on Windows 10 Using Winget!

Are you tired of downloading apps manually on your Windows 10 computer? Then it's time to use the latest command-line tool called Winget. This revolutionary tool allows you to install apps on your PC with just a few simple commands.

In this article, we'll explore how to use Winget to install apps on your Windows 10 computer. But before that, let's explore what Winget is and how it works.

What is Winget?

Winget is a package manager for Windows 10 that allows users to install, update, and uninstall applications from the command line. It aims to make it easier and faster to install software on Windows 10, without the need to open a browser and search for a download.

How does Winget work?

Winget uses a repository of application packages that contain information about the app's installation files, dependencies, and requirements. When you run a Winget command, it connects to this repository, downloads the necessary files, and installs the software on your computer.

So, how do you use Winget to install apps? Let's find out.

Step 1: Install Winget

The first step to using Winget is to install it on your Windows 10 computer. Microsoft has included Winget in the latest updates, so you don't need to download it separately. To check if it's installed on your computer, open the Command Prompt or PowerShell and type the following command:

winget --version

If Winget is installed, you'll see the version number. If not, you'll need to install it manually. Go to the Winget Github page, download the installer, and follow the on-screen instructions.

Step 2: Search the Repository

Now that you have Winget installed, you need to search for the app you want to install. To do this, type the following command in the Command Prompt or PowerShell:

winget search [app name]

Replace [app name] with the name of the application you want to install. For example, if you want to install Google Chrome, you'll type:

winget search Google Chrome

Step 3: Install the App

Once you've found the app you want to install, type the following command:

winget install [app name]

Replace [app name] with the name of the application you want to install. For example:

winget install GoogleChrome

Winget will now download and install the app on your computer.

Step 4: Update Apps

Winget also allows you to update your installed apps with ease. To do this, type the following command:

winget upgrade [app name]

Replace [app name] with the name of the app you want to update. For example:

winget upgrade GoogleChrome

Winget will check for updates and download and install them if available.

Step 5: Uninstall Apps

If you want to uninstall an app, type the following command:

winget uninstall [app name]

Replace [app name] with the name of the application you want to uninstall. For example:

winget uninstall GoogleChrome

Winget will now remove the app from your computer.

Conclusion

You won't believe how easy it is to install, update, and uninstall apps on Windows 10 using Winget. With just a few simple commands, you can have the latest apps installed on your computer, without the need to search for downloads manually. So, if you're looking for a faster and more efficient way to manage your apps, give Winget a try.

{{< youtube c5w_uHQAGbM >}} 



Windows 10 now includes the Windows Package Manager (winget), which is a tool that allows you to discover, install, upgrade, remove and configure apps on your device using the tool. Technically, the tool is simply an interface to connect and use the Windows Package Manager service.
 
The service is still in preview, which means that you’ll need to be part of the Windows Insider Program with a machine enrolled in the Fast ring to access the tool.
 
In this guide, you will learn the steps to install an app using the winget command on Windows 10. You can also use these instructions to uninstall apps.
 
## How to install app using Windows Package Manager
 
To install an app using the winget command, use these steps:
 
- Open Start on Windows 10.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to search the app and press Enter:
 - winget search APP-NAME
 - In the command, make sure to replace the APP-NAME for the name of the app that you’re trying to install. If you don’t know the exact name, you can search part of the name.
 - For example, the following command winget search micro will return apps available from Microsoft and other apps that may contain the query in the name or ID:
 - winget search micro
 - Windows 10 winget search command
 - Type the following command to install an app and press Enter:
 - winget install APP-NAME
 - In the command, make sure to change “APP-NAME” for the name of the app you want to install.
 - For example, the following command installs the PowerToys app:
 - winget install powertoys
 - Windows 10 winget install command
 - Continue with the on-screen directions (if applicable).

 
Once you complete the steps, the app will download and install on your device. If it is a desktop application, after the package downloads, you may need to go through the installation experience like with other desktop apps.
 
Open Start on Windows 10.
 
Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 
Type the following command to search the app and press Enter:
 
winget search APP-NAME
 
In the command, make sure to replace the APP-NAME for the name of the app that you’re trying to install. If you don’t know the exact name, you can search part of the name.
 
For example, the following command winget search micro will return apps available from Microsoft and other apps that may contain the query in the name or ID:
 
winget search micro


 
Windows 10 winget search command

 
Type the following command to install an app and press Enter:
 
winget install APP-NAME
 
In the command, make sure to change “APP-NAME” for the name of the app you want to install.
 
For example, the following command installs the PowerToys app:
 
winget install powertoys
 
Windows 10 winget install command

 
Continue with the on-screen directions (if applicable).
 
You can use the Windows Package Manager without administrator privileges, but you will be prompted to elevate, and if you choose not to elevate, the installation will fail.
 
The winget command should be available in the latest preview of Windows 10 in the Fast ring, if it’s not, you may need to install the preview version of the App Installer from the Microsoft Store.
 
Alternatively, you can also winstall to create a script to install apps in bulk on Windows 10 using winget.




