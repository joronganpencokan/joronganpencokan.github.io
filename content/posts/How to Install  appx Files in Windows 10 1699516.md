---
title: "Discover the Secret Hack to Install Any Appx Files in Windows 10 – Only a Few Clicks Needed!"
ShowToc: true 
date: "2022-12-25"
author: "Annette Bullard"
---
*****
Title: Discover the Secret Hack to Install Any Appx Files in Windows 10 – Only a Few Clicks Needed!

Introduction: 

Have you ever found yourself struggling to install an appx file in a Windows 10 device? It can be frustrating and time-consuming, especially when you’re not well-versed in technical know-how. But what if we told you there’s a simple solution to this problem? In this article, we’ll share a secret hack to install any appx files in Windows 10 with only a few clicks – saving you precious time and effort.

Body: 

The Appx format is a relatively new addition to the Windows ecosystem. Appx files are the standard packaging format for Windows Store applications and provide a seamless installation experience. However, installing appx files outside of the Windows Store can be a bit tricky.

First, you need to activate the Windows Developer Mode. This feature allows you to sideload or install third-party apps on your Windows 10 device. To activate it, open the Settings app and navigate to “Update & Security” > “For developers”, and select the “Developer mode” option.

Once you’ve enabled Windows Developer Mode, you need to install the appx file. The easiest way to do this is by using the PowerShell command. PowerShell is a command-line tool that allows you to automate various tasks in Windows.

To install an appx file using PowerShell, follow the steps below:

Step 1: Open PowerShell as an administrator from the Start menu or by pressing “Windows key + X” and selecting “Windows PowerShell (Admin)”.

Step 2: Type the following command, replacing <file path> with the path to your appx file:

Add-AppxPackage -Path <file path>

Step 3: Hit the “Enter” key to run the command. 

And that’s it! The appx file will be installed on your Windows 10 device. You can now access the installed app from the Start menu or the Apps section in Settings.

This hack not only saves you time and effort but also opens up a world of possibilities in terms of app installation options. You’re no longer limited to the Windows Store, so feel free to explore and install any appx files you come across.

Conclusion: 

Installing appx files in Windows 10 is no longer a challenge. All you need is a few clicks and the secret hack we’ve shared in this article. By enabling the Windows Developer Mode and using PowerShell commands, you can easily sideload any third-party apps onto your Windows 10 device. So go ahead and explore your app installation options without limitations!

{{< youtube DV3jdOOBEcM >}} 



With Windows 10, Microsoft introduced a new architecture called Universal Windows Platform (UWP) that aims to unify the app experience across devices like desktops and mobiles. As such, all the new Universal Windows Platform apps use “.appx” or “.appxbundle” as their file formats. One of the good things about UWP apps is that Windows manages all the installation and uninstallation process so that you don’t have to worry about any leftover files or registry entries.
 
Generally, you can download UWP apps directly from the Windows Store. However, if you want to you can directly download .appx files from a developer site and sideload them in your system. Here is how to manually install .appx files in Windows 10.
 
## Enable Sideloading Windows 10
 
Before you can install or sideload Universal Windows Platform apps, sideloading should be enabled in Windows 10. Thankfully, sideloading is enabled by default. However, it is better to verify and enable the “Sideloading” setting, as it might be disabled by your administrator or organization.
 
To enable sideloading, click on the Notification icon in the taskbar and then select the option “All Settings.”
 

 
Once the Settings app has been opened, click on the option “Update and Security.”
 
Here, navigate to “For Developers” appearing on the left panel.
 
Now, select the “Sideload apps” radio button on the right panel and close the window.
 
You’ve now successfully enabled sideloading in Windows 10.
 
## Install .appx Files With Double-Click
 
To sideload a UWP app, simply double-click on the .appx file. For instance, I downloaded the .appx file of CrystalDiskMark UWP app and double-clicked on it.
 
Since Windows uses its own installer, just click on the “Install” button to start the installation procedure. As you can see from the image below, Windows will show you which capabilities the app will run with. In my case the CrystalDiskMark app will run with “Full Trust Mode” capabilities.
 
Once the installation has been completed, just click on the “Launch” button to launch the installed UWP application.
 
If everything goes well, you should be able to use the app like any other UWP app installed from the Windows Store.
 
If you want to, you can uninstall the sideloaded app like any other app from the Windows Store. Simply find the app in the Start menu, right-click on it and then select the option “Uninstall” and you are good to go.
 
## Install .appx Files via PowerShell
 
Alternatively, you can also use the PowerShell to install an .appx file. To start, search for PowerShell in the Start menu, right-click on it and then select the option “Run as Administrator.”
 
The above action will launch PowerShell with administrator rights. Here, navigate to the file location using the below command. Don’t forget the replace c:\path\to\appx\file\directory with the actual directory path of the .appx file.
 
After navigating to the required directory, use the below command to install the .appx file. Again, don’t forget to replace “file.appx” with the actual UWP file name.
 
Alternatively, you can also use the below command:
 
As soon as you execute the command, the app will be installed. You will not receive any confirmation message whatsoever in the PowerShell window. However, you can search for the installed app in the Start menu and open it.
 
Do comment below sharing your thoughts and experiences about using the above methods to install .appx UWP files in Windows 10.
 
Vamsi is a tech and WordPress geek who enjoys writing how-to guides and messing with his computer and software in general. When not writing for MTE, he writes for he shares tips, tricks, and lifehacks on his own blog Stugon.
 
Our latest tutorials delivered straight to your inbox




