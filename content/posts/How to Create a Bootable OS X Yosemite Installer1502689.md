---
title: "You won't believe how easy it is to make a bootable OS X Yosemite installer! Click now to learn the secret!"
ShowToc: true 
date: "2023-03-29"
author: "David Morgan"
---
*****
Title: You won't believe how easy it is to make a bootable OS X Yosemite installer! Click now to learn the secret!

Description: Installing OS X Yosemite on your Mac is a simple task. But, did you know that creating a bootable OS X Yosemite installer is even more effortless? In this article, we will reveal the secret to making a bootable OS X Yosemite installer in just a few steps.

Introduction:

OS X Yosemite is the eleventh release of the Mac operating system, and its key features are its dynamic and streamlined look and feel, its advanced Spotlight search function, and its ability to work seamlessly with the Apple ecosystem. Installing it on a Mac requires an internet connection, an existing Mac OS X version of 10.6.8 or later, and at least 2 GB of RAM.

But, installing it via a bootable installer is an even more straightforward process. It ensures that you have a backup of the installation on an external drive, allowing you to install the OS with no need to download it again or worry about internet connection issues. Here is how to create one.

Steps to creating a bootable OS X Yosemite installer:

Step 1: Download OS X Yosemite from the Apple App Store ($20.00).

Step 2: Insert a USB drive with at least 8GB of storage (16GB recommended) into your Mac.

Step 3: Rename your USB drive. Open Finder and go to your USB drive, right-click and select Get Info. In the Info window, you can change the name under the Name & Extension section.

Step 4: Open Terminal from the Utilities folder within Applications.

Step 5: In Terminal, type 'diskutil list' (without quotes) to get a list of active disks on your Mac.

Step 6: Identify the USB drive by its size and type 'sudo /Applications/Install\ OS\ X\ Yosemite.app/Contents/Resources/createinstallmedia --volume /Volumes/USB --applicationpath /Applications/Install\ OS\ X\ Yosemite.app --nointeraction' (without quotes).

Step 7: Hit return, and Terminal will prompt you to enter your administrator password.

Step 8: Follow the prompts and select Y to confirm erasing the USB drive. The process usually takes about 20-30 minutes.

Conclusion:

Creating a bootable OS X Yosemite installer is a simple process that allows you to install the macOS on your Mac anytime you need it without having to download it again. The above-outlined steps are all you need to follow to have your bootable USB ready in just a few minutes. Next time you want to install OS X Yosemite, use your bootable installer, and you can do it in no time!

{{< youtube zBLnjT3lEd4 >}} 




You can download OS X Yosemite (10.10) for free from the Mac App Store if you have purchased it in the past and it shows in your purchase history with the option to re-download the operating system. Once you download it, the installer will start up automatically. If you follow the onscreen instructions, you'll end up with an upgrade install of OS X (or macOS) Yosemite on your startup drive.

 

What if you want to perform a clean install, completely erasing your startup drive? Or perhaps you'd like to have the installer on a bootable USB drive, so you don’t have to keep downloading it every time you wish to upgrade one of your Macs?

 

The problem is you cannot upgrade another Mac without downloading the installer all over again. The workaround is to create a bootable USB flash drive containing the OS X Yosemite installer.

 
##   Use Disk Utility to Create a Bootable OS X Yosemite Installer  
 

You can create a bootable installer in two ways.

 
While it's easiest to use a USB flash drive as the destination for the installer, you can use any bootable media, including hard drives, SSDs, and USB flash drives.
 

The first is to use a hidden Terminal command that can handle all of the heavy lifting for you.

 

The second is more manual and time-intensive. It uses the Finder and Disk Utility apps. This article will take you through the steps to manually create a bootable copy of the OS X Yosemite installer.

 
##   What You Need  
 
- OS X Yosemite installer. You can download the installer from the Mac App Store. Once complete, you'll find the download in the /Applications/ folder, with the file name Install OS X Yosemite.
 - A USB flash drive or another suitable bootable device. As mentioned, you can use a hard drive or an SSD for the bootable device, although these instructions will refer to a USB flash drive.
 - A Mac that meets the minimum requirements for OS X Yosemite.

 

The process for creating a bootable copy of the OS X Yosemite installer follows these basic steps:

 
- Mount the installer on your desktop.
 - Use Disk Utility to make a clone of the installer.
 - Modify the clone to allow it to boot successfully.

 
##   How to Mount the OS X Yosemite Installer  
 

Deep within the Install,OS X Yosemite file that you downloaded is a disk image that contains all of the files you need to create your own bootable installer. The first step is to gain access to this file.

 
- Open a Finder window and navigate to /Applications/.
 - Locate the file named Install OS X Yosemite, and then right-click the file and select Show Package Contents.
 - Open the Contents folder, then open the Shared Support folder.
 - Here you will find the disk image that contains the files you need to create a bootable installer. Double-click the InstallESD.dmg file.
 - Doing so will mount the InstallESD image on your Mac desktop and open a Finder window displaying the contents of the mounted file.
 - You may notice that the mounted image seems to contain only a single folder, named Packages. In actuality, the image file contains an entire bootable system that is hidden. You'll need to use Terminal to make the system files visible.
 - With the files now visible, you can see that the OS X Install ESD image contains three additional files: .DS_Store, BaseSystem.chunklist, and BaseSystem.dmg.

 
##   How to Use Disk Utility to Clone the OS X Install ESD Image  
 

The next step is to use Disk Utility's Restore feature to create a clone of the OS X Install ESD image you mounted on your desktop.

 

Open a Finder window and navigate to /Applications/.

 

Locate the file named Install OS X Yosemite, and then right-click the file and select Show Package Contents.

 

Open the Contents folder, then open the Shared Support folder.

 

Here you will find the disk image that contains the files you need to create a bootable installer. Double-click the InstallESD.dmg file.

 

Doing so will mount the InstallESD image on your Mac desktop and open a Finder window displaying the contents of the mounted file.

 

You may notice that the mounted image seems to contain only a single folder, named Packages. In actuality, the image file contains an entire bootable system that is hidden. You'll need to use Terminal to make the system files visible.

 

With the files now visible, you can see that the OS X Install ESD image contains three additional files: .DS_Store, BaseSystem.chunklist, and BaseSystem.dmg.

 
- Connect the target USB drive to your Mac.
 - Launch Disk Utility, located at /Applications/Utilities/.
 - Select the BaseSystem.dmg item listed in the left-hand pane of the Disk Utility window. It may be listed near the bottom, after your Mac's internal and external drives. If the BaseSystem.dmg item is not present in the Disk Utility sidebar, drag it into the sidebar from the Finder window that appeared when you mounted the InstallESD.dmg file.
 - Make sure you select BaseSystem.dmg, not InstallESD.dmg, which will also appear in the list.
 - Select Restore.
 - In the Restore tab, you will see BaseSystem.dmg listed in the Source field. If not, drag the BaseSystem.dmg item from the left-hand pane to the Source field.
 - Drag the USB flash drive from the left-hand pane to the Destination field.
 - The next step will completely erase the contents of the USB flash drive, or whichever bootable device you dragged to the Destination field.
 - Select Restore.
 - You will be asked to confirm that you want to erase the USB flash drive and replace its contents with BaseSystem.dmg. Select Erase.
 - If requested, supply your administrative password and select OK.
 - The restore process will take some time. Once it's complete, the Flash drive will mount on your desktop and open in a Finder window named OS X Base System. Keep this Finder window open, because we'll be making use of it in subsequent steps.

 
##   How to Modify the OS X Base System on Your Flash Drive  
 

All that's left to do is modify the OS X Base System (the flash drive) to make the OS X Yosemite installer work correctly from a bootable device.

 

Connect the target USB drive to your Mac.

 

Launch Disk Utility, located at /Applications/Utilities/.

 

Select the BaseSystem.dmg item listed in the left-hand pane of the Disk Utility window. It may be listed near the bottom, after your Mac's internal and external drives. If the BaseSystem.dmg item is not present in the Disk Utility sidebar, drag it into the sidebar from the Finder window that appeared when you mounted the InstallESD.dmg file.

 
Make sure you select BaseSystem.dmg, not InstallESD.dmg, which will also appear in the list.
 

Select Restore.

 

In the Restore tab, you will see BaseSystem.dmg listed in the Source field. If not, drag the BaseSystem.dmg item from the left-hand pane to the Source field.

 

Drag the USB flash drive from the left-hand pane to the Destination field.

 
The next step will completely erase the contents of the USB flash drive, or whichever bootable device you dragged to the Destination field.
 

You will be asked to confirm that you want to erase the USB flash drive and replace its contents with BaseSystem.dmg. Select Erase.

 

If requested, supply your administrative password and select OK.

 

The restore process will take some time. Once it's complete, the Flash drive will mount on your desktop and open in a Finder window named OS X Base System. Keep this Finder window open, because we'll be making use of it in subsequent steps.

 
- In the Finder window named OS X Base System, open the System folder, and then open the Installation folder.
 - Within the Installation folder, you will find an alias named Packages. Delete the Packages alias by dragging it to the trash, or by right-clicking the alias and selecting Move to Trash from the pop-up menu.
 - Leave the Installation window open, because we'll use it below.
 - From the OS X Install ESD window, drag the Packages folder to the Installation window you left open in the previous step.
 - From the OS X Install ESD window, drag the BaseSystem.chunklist and BaseSystem.dmg files to the OS X Base System window (the root level of the USB flash drive) to copy them to the flash drive.
 - Close all of the Finder windows once your computer finishes copying the files over.

 

Your USB flash drive is now ready to be used as a bootable OS X Yosemite installer.

 

In the Finder window named OS X Base System, open the System folder, and then open the Installation folder.

 

Within the Installation folder, you will find an alias named Packages. Delete the Packages alias by dragging it to the trash, or by right-clicking the alias and selecting Move to Trash from the pop-up menu.

 

Leave the Installation window open, because we'll use it below.

 

From the OS X Install ESD window, drag the Packages folder to the Installation window you left open in the previous step.

 

From the OS X Install ESD window, drag the BaseSystem.chunklist and BaseSystem.dmg files to the OS X Base System window (the root level of the USB flash drive) to copy them to the flash drive.

 

Close all of the Finder windows once your computer finishes copying the files over.

 

You can boot from the Yosemite installer you just made by inserting the USB flash drive into your Mac, and then starting your Mac while holding down the option key. The computer will start at the Apple boot manager, which will let you select the device you wish to start up from.

 
To keep your Finder as usable as possible, make the files you unhid invisible again.
 

Get the Latest Tech News Delivered Every Day




