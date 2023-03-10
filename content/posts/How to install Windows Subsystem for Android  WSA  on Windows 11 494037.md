---
title: "You won't believe how easy it is to install Android apps on Windows 11 with WSA - see how in just minutes!"
ShowToc: true 
date: "2023-06-28"
author: "Heather Gracia"
---
*****
# You won't believe how easy it is to install Android apps on Windows 11 with WSA - see how in just minutes!

If you're a Windows 11 user, you may have heard about the new Windows Subsystem for Android (WSA) feature that allows you to run Android apps on your PC. This exciting new feature has garnered a lot of attention and excitement among tech enthusiasts, and for good reason—the process of installing and running Android apps on Windows 11 using WSA is incredibly easy and straightforward.

In this article, we'll take a closer look at how you can use WSA to install Android apps on your Windows 11 PC in just a few minutes.

## Step 1: Install Windows 11 Insider Preview Build

Before you can install WSA on your Windows 11 PC, you'll need to make sure that you have the Insider Preview Build of Windows 11 installed. To do this, follow these steps:

1. Open the Settings app on your Windows 11 PC.
2. Click on "Update & Security."
3. Click on "Windows Insider Program" in the left sidebar.
4. Click on "Get Started."
5. Follow the prompts to sign in to your Microsoft account and enroll in the Insider program.
6. Once you've enrolled, go to "Windows Update" and check for updates. You should see the Insider Preview Build available for download.

## Step 2: Install WSA on Your Windows 11 PC

Now that you have the Insider Preview Build of Windows 11 installed, you're ready to install WSA. To do this, follow these steps:

1. Open the Microsoft Store on your Windows 11 PC.
2. Search for "Windows Subsystem for Android" and select it from the search results.
3. Click on "Get" to begin the download and installation process.

## Step 3: Install Android Apps on Your Windows 11 PC

Now that you have WSA installed on your Windows 11 PC, you're ready to start installing Android apps. Here's how:

1. Open the Microsoft Store on your Windows 11 PC.
2. Search for the Android app you want to install and select it from the search results.
3. Click on "Get" to begin the download and installation process.
4. Once the app is installed, you can find it in your Start menu and launch it like any other Windows app.

## Final Thoughts

As you can see, installing Android apps on your Windows 11 PC using WSA is a breeze. With just a few simple steps, you can have your favorite Android apps up and running on your PC in no time.

So why wait? Give WSA a try today and experience the best of both worlds—the power and convenience of a Windows 11 PC and the vast library of apps available on Android.

{{< youtube WaM7AyXFuMQ >}} 



This guide will teach you the steps to install WSA on Windows 11.
 
## Install WSA on Windows 11
 
Although installing the Windows Subsystem for Android requires only one click from the Microsoft Store, you still need to complete various steps before adding the support.
 
### 1. Prerequisites
 
You can use these instructions to check your computer specifications on Windows 11.
 
### 2. Enable Virtual Machine Platform
 
Before enabling the Virtual Machine Platform feature, the computer must have virtualization enabled on the UEFI firmware. If you don’t have this feature enabled, check with your computer manufacturer to find the specific details to complete this task.
 
To enable Virtual Machine Platform on Windows 11, use these steps:
 
- Open Start on Windows 11.
 - Search for Turn Windows features on or off, and click the top result to open the app.
 - Check the “Virtual Machine Platform” option.
 - Click the OK button.
 - Restart the computer.

 
Once you complete the steps, you can continue with the steps to install WSA. 
 
Open Start on Windows 11.
 
Search for Turn Windows features on or off, and click the top result to open the app.
 
Check the “Virtual Machine Platform” option.
 

 
Click the OK button.
 
Restart the computer.
 
### 3. Install Windows Subsystem for Android
 
Once you complete the steps, you can install Android apps on Windows 11. If you have problems installing this app, you can install WSA directly with the steps below.
 
Click the Install button.
 
After you complete the steps, you can start running Android apps on Windows 11.
 
#### Force installation from PowerShell
 
Alternatively, you can force the installation using PowerShell commands if you have a capable machine.
 
To install WSA manually with PowerShell, use these steps:
 
- Open the rg-adguard.net website.
 - Select the Productid option, paste this ID: 9p3395vx91nr, select the Slow option, and click the Check button.
 - Click the MicrosoftCorporationII.WindowsSubsystemForAndroid_2210.40000.7.0_neutral_~_8wekyb3d8bbwe.msixbundle link to save the app package (1.35GB).
 - Open Start.
 - Search for PowerShell, right-click the top result, and select the Run as administrator option.
 - Type the following command to change the directory to the folder with the Msixbundle file and press Enter:
 - cd C:\PATH\TO\Msixbundle
 - In the command, update the path with the location where you saved the package file.
 - Type the following command to install Windows Subsystem for Android on Windows 11 and press Enter:
 - Add-AppxPackage MicrosoftCorporationII.WindowsSubsystemForAndroid_2210.40000.7.0_neutral_~_8wekyb3d8bbwe.msixbundle.msixbundle
 - In the command, update the app package name with the name of the file you have downloaded.

 
Open the rg-adguard.net website.
 
Select the Productid option, paste this ID: 9p3395vx91nr, select the Slow option, and click the Check button.
 
Click the MicrosoftCorporationII.WindowsSubsystemForAndroid_2210.40000.7.0_neutral_~_8wekyb3d8bbwe.msixbundle link to save the app package (1.35GB).
 
Open Start.
 
Search for PowerShell, right-click the top result, and select the Run as administrator option.
 
Type the following command to change the directory to the folder with the Msixbundle file and press Enter:
 
cd C:\PATH\TO\Msixbundle
 
In the command, update the path with the location where you saved the package file.
 
Type the following command to install Windows Subsystem for Android on Windows 11 and press Enter:
 
Add-AppxPackage MicrosoftCorporationII.WindowsSubsystemForAndroid_2210.40000.7.0_neutral_~_8wekyb3d8bbwe.msixbundle.msixbundle
 
In the command, update the app package name with the name of the file you have downloaded.




