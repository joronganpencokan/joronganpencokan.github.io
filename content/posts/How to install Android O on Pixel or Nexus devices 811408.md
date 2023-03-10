---
title: "Unlock the Secret to the Latest Android O Update: A Step-by-Step Guide to Installing on Your Pixel or Nexus Device!"
ShowToc: true 
date: "2023-01-22"
author: "Frank Young"
---
*****
# Unlock the Secret to the Latest Android O Update: A Step-by-Step Guide to Installing on Your Pixel or Nexus Device!

Are you still using the outdated Android Nougat OS on your Pixel or Nexus device? If yes, then it's time to upgrade to the latest Android O. With its impressive features and benefits, Android O has caught the attention of many tech enthusiasts. So, if you want to explore its innovative traits, then follow our step-by-step guide to install Android O on your Pixel or Nexus device.

## Step 1: Back Up Your Device

Before you start the installation process, it's essential to back up your data to avoid any data loss. Therefore, connect your device with a charger and connect it to a Wi-Fi network. Then navigate to settings, select the backup option, and click on the backup my data button. This step will ensure that all your data is safely stored in the cloud.

## Step 2: Enroll in the Android Beta Program

To access the latest Android O update, you must enroll in the Android Beta program. This program allows you to receive the latest OS updates before they are released to the general public.  To enroll in the Android Beta program, visit https://www.google.com/android/beta and sign in with your Google account. Once you have access, select your device and click on the enroll device button. This will allow you to receive updates of the latest OS versions.

## Step 3: Update Your Device

After enrolling in the beta program, go to your device's settings, click on the system update option, and check for an available update. If there is an available update, then click on the download and install option to start downloading the Android O update.

## Step 4: Wait for the Installation to Complete

After downloading the update, let the installation process begin. Wait for the installation to complete, and restart your device. During the installation process, your device will reboot several times. Therefore, it's essential to be patient and let the process take its course.

## Step 5: Start Exploring Android O

Finally, your device has been successfully upgraded to the latest Android O. After the installation process is complete, start exploring the new features and exciting improvements of Android O. You will undoubtedly appreciate the better battery life, the picture-in-picture feature, and the new notification features, among others.

Conclusion

In conclusion, upgrading to the latest Android O is essential to experience the latest features and performance improvements that come with this particular OS. You can quickly and easily install the Android O update on your Pixel or Nexus device by following our step-by-step guide. So, enroll in the Android Beta program, back up your data, check for the update, and start exploring the new features of Android O. With Android O, you can be assured of a fast, reliable, and enjoyable user experience. Hurry and upgrade to Android O today!

{{< youtube uXc5mES8LA4 >}} 



Android O is the next version of Google’s mobile OS that the company will be releasing in 2017. The new version of Android doesn’t include major changes, but it’ll improve your device battery life and notifications. There will be an official API for autofill, adaptive icons, and O will introduce a new picture-in-picture mode for tablets as well as phones.
 
Alongside the announcement, Google also made available the factory image preview for developers. Although, you’ll have to wait until May to get Android O through the beta program, you can install the early preview on your Pixel or Nexus device. It’s just going to take a little more of work.
 
In this guide, you’ll learn the steps to manually flash your phone or tablet to install Android O and test all the new features.
 
- Android O supported devices
 - Backup your Android device
 - Download ’15 seconds ADB Installer’
 - Download Android O
 - Configure your Android device
 - How to flash your device using Android O

 
## Android O supported devices
 
If you want to try Android O, you’ll need one of these compatible devices:
 
- Google Pixel
 - Google Pixel XL
 - Google Pixel C
 - Nexus 5X
 - Nexus 6P
 - Nexus Player

 
You shouldn’t try to install this version of the mobile OS on any other device other than the ones in the list.
 
Also, remember that Android O is an unfinished product, and you’ll find bugs, you’ll come across errors, and features may not work as expected.
 
## Backup your Android device
 
Since you’ll be unlocking the bootloader and doing a clean install of the OS, you want to make sure to make a backup of your data before proceeding.
 
You can quickly do this by going to Settings > Backup & reset and make sure your device and app date are backed up.
 
Create a backup of your photos and videos, you can use Google Photos, or you can connect your phone or tablet to your computer and just copy over the DCIM folder. Also, don’t forget to copy other files and folders you may have created.
 
## Download ’15 seconds ADB Installer’
 
The “15 seconds ADB Installer” is not from Google, but it’s a tool that helps you to install the official Android tools on Windows without needing to download the entire SDK to install only a few items. You can download this tool from XDA forums using the link below.
 
- 15 seconds ADB Installer | Download

 
When you launch the setup, type Y to agree to install ADB and Fastboot. Type Y again when asked to Install ADB system-wide and device drivers. Finally, restart your computer to complete the installation.
 
The installation files will be located inside the adb folder in the C:\ drive.
 
## Download Android O
 
It’s now the time to download the image that contains the files to install Android O. Google is listing the images to supported devices at the Android developers support site. Under the “Downloads” section, click the download link that correspond to your device.
 
Once the image downloaded on your computer, use a third-party tool like 7zip to extract all its content to C:\adb.
 
## Configure your Android device
 
Before you can install Android O on Pixel or Nexus devices, you need to enable the developer mode on your device by doing the following:
 
- Open Settings.
 - Select on About phone.
 - Tab on Build number about 7 times until you see the “become a developer” message.
 - On the main Settings page, select Developer options.
 - Turn on the OEM unlocking and USB debugging toggle switches. These options will allow you to quickly unlock your device with a single command, and you’ll be able to send files from your computer to your Android device.
 - OEM Unlocking and USB Debugging options

 
## How to flash your device using Android O
 
To flash your device with the new Android O preview, power off your phone or tablet, connect it to your computer using a USB data cable, and do the following:
 
Open Settings.
 
Select on About phone.
 
Tab on Build number about 7 times until you see the “become a developer” message.
 
On the main Settings page, select Developer options.
 
Turn on the OEM unlocking and USB debugging toggle switches. These options will allow you to quickly unlock your device with a single command, and you’ll be able to send files from your computer to your Android device.
 
OEM Unlocking and USB Debugging options
 
- Power on your device using fastboot using press and hold down the Volume button down and Power button on your Nexus 6P, Nexus 5X, Google Pixel, Google Pixel XL and Google Pixel C.
 - On your PC, browse the following path and locate the flash-all.bat file:
 - C:\adb
 - Right-click the flash-all.bat file and select Run as administrator.
 - Inside the adb folder, hold down the shift key, right-click on an empty space, and select “Open command window here”. Alternatively, you can always open Command Prompt and navigate to C:\adb.
 - Type the following command to verify that your device has connectivity with your computer and press Enter:
 - fastboot devices
 - If the command returns your phone’s serial number, then everything is working OK so far.
 - Type the following command unlock the bootloader and wipe everything on your phone and press Enter:
 - fastboot flashing unlock
 - Type the following command to re-lock of the bootloader after Android O is installed on your device and press Enter:
 - fastboot flashing lock

 
Once you completed the steps, you can start using Android O on your device. It should be noted that to uninstall a Developer Preview to roll back to Android Nougat, you’ll need to do a full device reset, which will remove all data, apps, and settings.
 
Power on your device using fastboot using press and hold down the Volume button down and Power button on your Nexus 6P, Nexus 5X, Google Pixel, Google Pixel XL and Google Pixel C.
 
On your PC, browse the following path and locate the flash-all.bat file:
 
C:\adb
 
Right-click the flash-all.bat file and select Run as administrator.
 
Inside the adb folder, hold down the shift key, right-click on an empty space, and select “Open command window here”. Alternatively, you can always open Command Prompt and navigate to C:\adb.
 
Type the following command to verify that your device has connectivity with your computer and press Enter:
 
fastboot devices
 
If the command returns your phone’s serial number, then everything is working OK so far.
 
Type the following command unlock the bootloader and wipe everything on your phone and press Enter:
 
fastboot flashing unlock
 
Type the following command to re-lock of the bootloader after Android O is installed on your device and press Enter:
 
fastboot flashing lock




