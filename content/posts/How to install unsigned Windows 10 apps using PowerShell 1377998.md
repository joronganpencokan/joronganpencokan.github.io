---
title: "Secret Hack: Install Any Windows 10 App Without Hesitation Using This Simple Powershell Trick!"
ShowToc: true 
date: "2023-04-28"
author: "Carl Thorpe"
---
*****
Title: Secret Hack: Install Any Windows 10 App Without Hesitation Using This Simple Powershell Trick!

Are you tired of being hesitant when downloading apps on your Windows 10 device due to the fear of malicious software? Well, fear no more! There's a simple yet effective solution to install any Windows 10 app without hesitation using a Powershell trick!

Powershell is a command line tool that allows Windows users to automate tasks and manage configurations. This tool is available on all Windows devices and can be used to quickly install apps from the Microsoft Store with ease.

Here's how it works:

Step 1: Open Powershell

To open Powershell, simply press the Windows key + X and select "Windows PowerShell" from the menu.

Step 2: Enable Execution Policy

By default, the execution policy is set to "Restricted" which prevents the installation of certain apps. To change this policy, type the following command in Powershell:

Set-ExecutionPolicy RemoteSigned -Scope CurrentUser

Step 3: Install

Once the execution policy is set, you can install any Windows 10 app using the following command:

PowerShell -Command Add-AppxPackage -Path "C:\Path\To\The\AppxFile.appx"

Replace "C:\Path\To\The\AppxFile.appx" with the path to the app you're looking to install. You can find the path by right-clicking the app file and selecting "Properties."

And that's it! With these simple steps, you can now install any app without hesitation using Powershell. This trick is particularly useful for those who wish to install apps that are not readily available on the Microsoft Store.

However, it's important to note that this method should only be used for trusted apps. Be sure to do your research and only install apps from reputable sources to avoid any potential security risks.

In conclusion, Powershell is a fantastic tool for Windows users looking to automate tasks and manage configurations on their devices. With this simple trick, you can install any Windows 10 app without hesitation and unleash the full potential of your device. Give it a try today!

{{< youtube Jfvg3CS1X3A >}} 



Windows 10 apps are built and installed differently than traditional desktop applications. While with desktop applications, you need to go through various installation steps, with an appx package, you only need to click one button.
 
These types of apps (part of the Universal Windows Platform (UWP)) are usually available through the Microsoft Store, but there will be times when you’ll have to install them outside of the store.
 
Depending on how you acquired the app, you’ll come across apps with a digital signature, which is a requirement before they’re submitted to the Microsoft Store, and those that might still be under development and are unsigned.
 
While you can install digitally signed Windows 10 apps with a single click from the store and different sources, you cannot easily install unsigned apps. If you try to install an unsigned appx package, you’ll get the “Ask the app developer for a new app package. This one isn’t signed with a trusted certificate (0x800B0100)” error message. However, the installation isn’t impossible, you need to change the installation settings and use the PowerShell command-line tool.
 
This guide will teach you the steps to install unsigned Windows 10 apps on your computer.
 
## Install unsigned appx packages on Windows 10
 
It’s important to note that in most cases, you shouldn’t install unsigned apps on Windows 10, as they may cause harm to your computer. However, if you are a developer or trying to install a new Windows 10 app outside of the store, you can use the following steps to install the unsigned “.appx” package.
 
### Enable Developers mode
 
If the app doesn’t have a digital signature, you must enable the “Developer mode” on your computer.
 
- Open Settings.
 - Click on Update & security.
 - Click on For developers.
 - Under the “Developer Mode” section, turn on the “Install apps from any source, including loose files” toggle switch.
 - Click the Yes button.
 - Restart your computer.

 
Once you have enabled the developer mode, you can install the unsigned packages.
 
Open Settings.
 
Click on Update & security.
 
Click on For developers.
 
Under the “Developer Mode” section, turn on the “Install apps from any source, including loose files” toggle switch.
 

 
Click the Yes button.
 
Restart your computer.
 
### Install unsigned apps using PowerShell
 
If you are trying to install an app that wasn’t packaged, meaning that you have a folder with all content instead of a single *.appx file, you will need to use the following instructions:
 
- Open Start, search for PowerShell, right-click the result, and select the Run as administrator option.
 - Type the following command to register the app and press Enter:
 - Add-AppxPackage -Path PATH-TO-APPXFILEFOLDER\AppxManifest.xml -Register

 
If you have a “*.appx” file, double-click it, and click the Install button. Or to avoid running into any issues, you can use the following PowerShell command:
 
Open Start, search for PowerShell, right-click the result, and select the Run as administrator option.
 
Type the following command to register the app and press Enter:
 
Add-AppxPackage -Path PATH-TO-APPXFILEFOLDER\AppxManifest.xml -Register
 
- Open Start.
 - Search for PowerShell, right-click the result, and select the Run as administrator option.
 - Type the following command to install the unsigned app and press Enter:
 - Add-AppxPackage -Path PATH-TO-APPXFILE\APP.appx

 
After you complete the steps, you can launch the app from the Start menu like any other Windows application.
 
Open Start.
 
Search for PowerShell, right-click the result, and select the Run as administrator option.
 
Type the following command to install the unsigned app and press Enter:
 
Add-AppxPackage -Path PATH-TO-APPXFILE\APP.appx




