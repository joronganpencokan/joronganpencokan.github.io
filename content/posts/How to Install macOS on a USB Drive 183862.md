---
title: "Unlock the Secret to Portable MacOS - Learn How to Install It on a USB Drive Now!"
ShowToc: true 
date: "2022-11-22"
author: "Beverly Huey"
---
*****
- Article -
Title: Unlock the Secret to Portable MacOS - Learn How to Install It on a USB Drive Now!

Are you tired of being tethered to a single computer or having to carry around a bulky laptop? If you own a Mac, you may be able to unlock the secret to a portable computing experience by installing MacOS on a USB drive.

With MacOS on a USB drive, you can carry your entire operating system with you and use it on any Mac computer. This means you can keep your files, settings, and applications with you at all times, even if you’re using a computer that’s not your own.

To get started, you’ll need a few things:

- A USB drive with at least 16GB of storage space
- A Mac computer with MacOS installed
- A copy of the MacOS installer (which you can download from the App Store)

Once you have all of these things, you can begin the process of creating a bootable USB drive with MacOS on it.

Step 1: Format the USB Drive

First, you’ll need to format the USB drive so that it can be used as a bootable drive. To do this, open Disk Utility (which you can find in the Applications > Utilities folder) and select the USB drive from the list of devices.

Next, click on the Erase button and choose the following options:

- Name: Give your USB drive a name (such as “MacOS Install”)
- Format: Choose “Mac OS Extended (Journaled)”
- Scheme: Choose “GUID Partition Map”

Click Erase to format the USB drive.

Step 2: Download the MacOS Installer

Next, you’ll need to download the MacOS installer from the App Store. This can take some time, as the installer is several gigabytes in size.

Once the download is complete, the installer will automatically open. Don’t proceed with the installation just yet - instead, quit the installer and make a copy of it on your desktop.

Step 3: Create the Bootable USB Drive

Now it’s time to create the bootable USB drive. To do this, follow these steps:

1. Open Terminal (which you can find in the Applications > Utilities folder).
2. Type in the following command, but do not hit enter yet: sudo /Applications/Install\ macOS\ Mojave.app/Contents/Resources/createinstallmedia --volume /Volumes/MacOS\ Install --applicationpath /Applications/Install\ macOS\ Mojave.app
3. Replace “Mojave” in the command above with the version of MacOS that you downloaded. For example, if you downloaded High Sierra, the command would be: sudo /Applications/Install\ macOS\ High\ Sierra.app/Contents/Resources/createinstallmedia --volume /Volumes/MacOS\ Install --applicationpath /Applications/Install\ macOS\ High\ Sierra.app
4. Insert the USB drive into your Mac.
5. Select the entire command you typed in Step 2 and copy it (Cmd+C).
6. In Terminal, paste (Cmd+V) the command.
7. Press enter and authenticate with your administrator password.

The process can take some time, so be patient. Once it’s complete, your USB drive will be ready to use.

Step 4: Boot from the USB Drive

To use MacOS on your USB drive, you’ll need to boot your Mac from the USB drive. To do this:

1. Shut down your Mac.
2. Insert the USB drive into your Mac.
3. Turn on your Mac while holding down the Option key.
4. Select the USB drive from the list of bootable devices.

Your Mac will now boot into MacOS from the USB drive. You can use it just like you would on any other Mac computer.

Conclusion

Installing MacOS on a USB drive is a great way to make your computing experience more portable. It can be especially handy if you need to work on multiple computers or if you want to carry your entire operating system with you wherever you go.

With this guide, you should now be able to create a bootable USB drive with MacOS on it. Happy computing!

{{< youtube ttPz5eA_2SI >}} 



A cloned version of your macOS installation on a portable USB drive can be invaluable if your system suddenly fails to boot. It can give you troubleshooting options and even permit you to keep working with an identical copy of your files. While internal hard drives are the best way to create bootable copies of your system, a USB drive can also work. You will learn in this guide how to install macOS on a USB drive.
 
## How to Install macOS on a USB Drive
 
You’ll want to use the Disk Utility app for this method. First, right-click the USB drive in Disk Utility and click “Erase.” 
 
Format your USB drive as “Mac OS Extended (Journaled)” and choose the GUID Partition Map scheme.
 
If you can’t find the option to set the partition table, make sure you’re selecting the “View -> Show All Devices” option.
 
Right-click on the USB drive, click Erase, and select the partition table.
 
When the process is complete, download macOS. Unless you have a specific reason to install an older version of macOS, download the most recent installer from the App Store.
 
Given the size of macOS Big Sur (around 13GB), it may take a while. It may open and begin to take you through the installation process when it finishes downloading, but you don’t want to do this. Follow the instructions below for another way to create a bootable installer.
 
Open Terminal (found in the Utilities folder) and copy the snippet below. Note that you’ll want to change the placeholder for whatever your USB drive is called:
 
This code makes a couple of assumptions:
 
- You’re installing macOS Big Sur onto your USB drive.The downloaded installer will get stored in your Applications folder.

 
Of course, you’ll need to change the file paths if neither of these are true. For other Operating Systems, Apple provides the necessary snippets you need.
 
Once you press the Return key, the installation process will begin. Note that you’ll need to input your administrator password and confirm that you want to erase the current drive.
 
It could take a while to erase the USB, but at some point, you will be asked whether Terminal can access files on your USB drive. You should confirm that it can.
 
From there, the install process will copy files to your USB. It will also rename the USB to whatever is set for the installer you downloaded. In our example, it’s “Install macOS Big Sur.”
 
At this point, you can quit Terminal and eject the USB drive.
 
## How to Clone Your Hard Drive to a USB Drive
 
If you have a USB drive large enough to accommodate the data on your boot drive, you can create a direct clone of your boot drive. If you use the proper software, this disk will also be bootable.
 
There are many options here, although SuperDuper or Carbon Copy Cloner are fantastic. This tutorial is using Carbon Copy Cloner (CCC) to create a clone of your hard drive.
 
The process is super straightforward. 
 
1. Select your boot drive as the source for the clone.
 
2. Set your USB drive as the target for the cloning operation.
 
3. Click “Start” to begin the cloning process. This will overwrite and replace the content of the USB drive with the clone of the boot drive. 
 
From here, you’ll want to boot from the drive itself. 
 
## How to Boot Up from a USB Drive
 
Once you’ve installed macOS on a USB drive, or cloned your hard drive, you’ll need to restart your computer and boot from your USB drive.
 
You can run macOS from a bootable USB installation much like you’d run one from from an internal drive. There’s no operational difference between the two systems. Though, running off of a USB drive is going to be slower than the internal SSD. 
 
To boot from your USB drive, set your bootable USB as your startup disk for the next boot in “System Preferences -> Startup Disk,” then click “Restart” to reboot your Mac.
 
Your Mac will reboot from the USB instead of your default startup disk. You could also use the Startup Manager to select your boot drive when you start macOS.
 
If you’re using an Apple Silicon machine, you’ll need to insert the USB drive, shut the Mac down, then reboot and hold the Power key until you come to the Startup Manager.
 
For Intel Macs, restart and hold the Option key to enter into the boot selection dialog.
 
For both types of machines, use your keyboard’s arrow keys to select the USB drive from the list of bootable devices, click to confirm, and your USB drive will begin to boot.
 
You can now run the operating system as normal and use this USB drive to boot up your Mac. Disk operations on the boot drive can be performed safely from a USB stick as well.
 
## Frequently Asked Questions
 
### 1. Can I split an installation across multiple USB drives?
 
In our experience, you will not be able to do this. As such, you’ll need a large enough USB drive to store Big Sur. We recommend 16GB to give yourself enough “wiggle room” when it comes to the installation process.
 
### 2. Am I able to use a USB connection other than USB-C?
 
Yes. Our testing gave us no issues when using a USB 2.0 to USB-C connector, so you’re able to press your older USB drives into service.
 
### 3. Can I boot older versions of macOS from a USB drive?
 
Our tests were inconclusive here. In theory, there’s no reason why you couldn’t boot an older version of macOS, and Apple does offer ways to install older versions on a USB. Though, if your Mac is based on Apple Silicon, you may find incompatibilities.
 
We also don’t know whether you’ll experience issues if you look to install an older OS you don’t own. In short, we don’t recommend it, and it’s likely not supported.
 
## Wrapping Up
 
Linux users know that booting from a USB drive is a useful way to get into the OS. macOS users can also install the OS onto a USB drive and work with the same installation that’s on your internal (and faster) drive. In fact, you have a couple of ways to do this: either using Disk Utility to format the drive before installing macOS or cloning your drive using a third-party tool.
 
If you have a USB drive that needs to be fixed, find out how to fix unformattable USB drives. What will you use your USB installation of macOS for? Let us know in the comments section below!
 
Tom Rankin is a quality content writer for WordPress, tech, and small businesses.



When he's not putting fingers to keyboard, he can be found taking photographs, writing music, playing computer games, and talking in the third-person.
 
Our latest tutorials delivered straight to your inbox




