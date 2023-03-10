---
title: "Unlock the secret to refreshing your Nexus 6 with the ultimate guide to installing 5.1.0 Lollipop factory image!"
ShowToc: true 
date: "2023-03-17"
author: "Yvonne Trudnowski"
---
*****
Unlock the Secret to Refreshing Your Nexus 6 with the Ultimate Guide to Installing 5.1.0 Lollipop Factory Image!

If you're a Nexus 6 owner and your device is running slow, stuttering or simply not working the way it should, you may need to consider installing a new operating system. The Android 5.1.0 Lollipop OS may be just what you need to bring your Nexus 6 back to life. In this ultimate guide, we walk you through the steps needed to install the factory image for Android 5.1.0 Lollipop on your Nexus 6.

Why You Should Install Android 5.1.0 Lollipop

Android 5.1.0 Lollipop is not just your average operating system. This upgrade comes with several features that improve your device's performance and usability. Here are some reasons why you should consider installing it on your Nexus 6:

1. Improved Battery Life: One of the most notable improvements in Android 5.1.0 Lollipop is its battery life enhancements. Doze, a new feature in this update, enables your device to conserve battery life by entering sleep mode whenever it's not in use.

2. Enhanced Security: Android 5.1.0 Lollipop comes with improved device security features. One such feature is the ability to set a device lock screen message that displays your contact information when the phone is locked. This means that if someone finds your phone, they will know who to contact to return it.

3. Faster Performance: With Android 5.1.0 Lollipop, your Nexus 6 will run faster and smoother than before. This improved performance can be attributed to several factors such as the ART runtime, which replaces the old Dalvik runtime and is much faster.

Step-by-Step Guide to Installing Android 5.1.0 Lollipop Factory Image

Before you proceed with the installation process, please note that installing the factory image will wipe all of the data on your Nexus 6. Therefore, it is important to backup all of your data before proceeding with the installation process. Follow these steps to install the factory image for Android 5.1.0 Lollipop on your device:

Step 1: Download the Android SDK

Before you can install the factory image, you need to download and install the Android SDK on your computer. You can download the SDK from the Android developer website.

Step 2: Download the Factory Image

Once you have downloaded and installed the SDK, you need to download the factory image for your device from the Google Nexus Factory Images page.

Step 3: Prepare Your Nexus 6

Now that you have the factory image, you need to prepare your Nexus 6. To do this, follow these steps:

• Enable USB Debugging: Go to Settings > Developer Options > USB Debugging and check the box.

• Unlock the Bootloader: Put your Nexus 6 into bootloader mode by powering off your device and then holding down the power button and the volume down button until the bootloader screen appears. Use the volume buttons to navigate to the "Unlock Bootloader" option and press the power button to confirm your decision.

• Install ADB and Fastboot: Extract the files from the Android SDK to your preferred location on your computer. Then, search for and open the "SDK Manager." Check the boxes next to "Android SDK Platform-tools" and "Google USB Driver" and click on "Install Packages."

Step 4: Flash the Factory Image

Now it's time to flash the factory image. Connect your Nexus 6 to your computer and use ADB to boot into fastboot mode by typing "adb reboot bootloader" in the command prompt. Once your device is in fastboot mode, navigate to the folder where you extracted the factory image files and type "flash-all" in the command prompt. This will begin the installation process, and your Nexus 6 will reboot once the process is complete.

In conclusion, installing the factory image for Android 5.1.0 Lollipop on your Nexus 6 can refresh your device and give it a new lease of life. With the improved battery life, enhanced security features, and faster performance, the benefits of this upgrade are too good to pass up. By following the steps in this ultimate guide, you can install the factory image with ease and enjoy all the benefits of Android 5.1.0 Lollipop on your Nexus 6.

{{< youtube c5yBAbv43Jo >}} 



Google had recently released the Android Lollipop 5.1 version along with its changelog, and it has already started to become obsolete, let alone the 5.0 or 5.0.2 versions (they are too old to discuss about now). Recently, Google had released the factory image of 5.10 Lollipop for the Nexus 6. The new build LMY47E, which is different from the previous build, LMY47D.
 

 
For the newbies, here is a guide on how to install the factory image of 5.1.0 Lollipop in your Nexus 6:
 
- First of all, Download the factory image for the new build from here.

 
To flash a device using one of the system images below (or one of your own), you need the fastboot tool. You can get the fastboot tool either:
 
- From a compiled version of the the Android Open Source Project.
 - Or, from the platform-tools/ directory in the Android SDK. Be sure that you have the latest version of the Android SDK Platform-tools from the SDK Manager.

 
Once you have the fastboot tool, add it to your PATH environment variable (the flash-all script below must be able to find it). Also be certain that you’ve set up USB access for your device, as described in the Using Hardware Devices guide.
 
From a compiled version of the the Android Open Source Project.
 
Or, from the platform-tools/ directory in the Android SDK. Be sure that you have the latest version of the Android SDK Platform-tools from the SDK Manager.
 
Caution: Flashing a new system image deletes all user data. Be certain to first backup any personal data such as photos.
 
To flash a system image:
 
- Download the appropriate system image for your device below, then unzip it to a safe directory.
 - Connect your device to your computer over USB.
 - Start the device in fastboot mode with one of the following methods:
 - Using the adb tool: With the device powered on, execute:
 - adb reboot bootloader
 - Using a key combo: Turn the device off, then turn it on and immediately hold down the relevant key combination for your device. For example, to put a Nexus 5 (“hammerhead”) into fastboot mode, press and hold Volume Up + Volume Down + Power as the device begins booting up.
 - If necessary, unlock the device’s bootloader by running:
 - fastboot oem unlock
 - The target device will show you a confirmation screen. (This erases all data on the target device.)
 - Open a terminal and navigate to the unzipped system image directory.
 - Execute the flash-all script. This script installs the necessary bootloader, baseband firmware(s), and operating system.

 
Once the script finishes, your device reboots. You should now lock the bootloader for security:
 
Download the appropriate system image for your device below, then unzip it to a safe directory.
 
Connect your device to your computer over USB.
 
Start the device in fastboot mode with one of the following methods:
 
- Using the adb tool: With the device powered on, execute:
 - adb reboot bootloader
 - Using a key combo: Turn the device off, then turn it on and immediately hold down the relevant key combination for your device. For example, to put a Nexus 5 (“hammerhead”) into fastboot mode, press and hold Volume Up + Volume Down + Power as the device begins booting up.

 
Using the adb tool: With the device powered on, execute:
 
adb reboot bootloader
 
Using a key combo: Turn the device off, then turn it on and immediately hold down the relevant key combination for your device. For example, to put a Nexus 5 (“hammerhead”) into fastboot mode, press and hold Volume Up + Volume Down + Power as the device begins booting up.
 
If necessary, unlock the device’s bootloader by running:
 
fastboot oem unlock
 
The target device will show you a confirmation screen. (This erases all data on the target device.)
 
Open a terminal and navigate to the unzipped system image directory.
 
Execute the flash-all script. This script installs the necessary bootloader, baseband firmware(s), and operating system.
 
- Start the device in fastboot mode again, as described above.
 - Execute:
 - fastboot oem lock

 
Locking bootloader will wipe the data on some devices. After locking the bootloader, if you want to flash the device again, you must run fastboot oem unlock again, which will wipe the data.
 
Start the device in fastboot mode again, as described above.
 
Execute:
 
fastboot oem lock
 
This update for the Nexus 6 is obviously to fix the memory leak issues, which was experienced in the 5.1 Lollipop for LMY47D build. For rest of the devices running on 5.1 (the Nexus 5, Nexus 10 and Android One devices, which recently got the update) Google has secretly fixed the issue without rolling out any major update, so there is nothing to worry about.
 
Did you update your Nexus 6 to latest build installing the factory images provided by Google? Feel free to share your experience or opinions in the comment section below.
 
- TAGSNexus 6System Update

 
### How To: Stop Bootloop in Samsung Galaxy S8
 
### Samsung rolls out first OTA update for T-Mobile’s Galaxy S6 and S6 Edge
 
### Buyer’s Guide: Top Stock Android Smartphones
 
### Nexus 6 vs iPhone 6 Plus vs OnePlus One: specs comparison
 
### Motorola Nexus 6 goes official: specs and details
 
### Leave a Reply Cancel reply

 
### How to Fix Samsung Galaxy S22 Overheating?
 
### How to Fix Mobile Data Not Working on Samsung Galaxy S22?
 
### Instagram Tips and Tricks
 
### How to See Liked Posts on Instagram?
 
### How to Make Android Faster?




