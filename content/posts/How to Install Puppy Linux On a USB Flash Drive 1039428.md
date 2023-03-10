---
title: "Revolutionize Your Computing Experience: Install Puppy Linux on a USB Flash Drive like a Pro!"
ShowToc: true 
date: "2022-11-17"
author: "Kim Jackson"
---
*****
Revolutionize Your Computing Experience: Install Puppy Linux on a USB Flash Drive like a Pro!

In today's world, technology is constantly evolving, and with it, so are the needs of computer users. One of the latest trends in the computing world is the use of Linux operating systems. If you are looking for a fast, reliable, and easy-to-use operating system, then you should consider using Puppy Linux. This lightweight operating system is designed to run on older computers, making it perfect for those who are looking to revive their old systems. Moreover, Puppy Linux can be installed on a USB flash drive, allowing you to carry your operating system with you wherever you go. In this article, I will guide you on how to install Puppy Linux on a USB flash drive like a pro.

First, you need to download the Puppy Linux ISO file from the official website. After downloading the ISO file, you need to create a bootable USB flash drive. To do this, you can use several tools such as Rufus, UNetbootin, or Etcher. Insert your USB flash drive into your computer and run the chosen tool. Select the ISO file you have downloaded and click on the "Create" button to start the process. Wait until the process is complete, and your bootable USB flash drive is ready.

The next step is to boot your computer from the USB flash drive. To do this, you need to change the boot order in your computer's BIOS. Boot your computer and press the key to access the BIOS settings. The key depends on your computer's manufacturer, but it is usually F2, F12, or Delete. Once you are in the BIOS settings, look for the Boot menu and change the boot order to boot from the USB flash drive. Save the changes and exit the BIOS settings.

When your computer boots from the USB flash drive, you will see the Puppy Linux welcome screen. Press Enter to continue. Next, you will see the Puppy Linux desktop. You can now start exploring the operating system and its features.

One of the great features of Puppy Linux is that you can install it on your computer's hard drive directly from the USB flash drive. To do this, click on the "Install Puppy" icon on the desktop. Follow the installation wizard instructions to set up your hard drive for Puppy Linux. You can choose to install Puppy Linux alongside your existing operating system or replace it entirely. Be sure to select the correct options, and backup any important files before proceeding.

In conclusion, installing Puppy Linux on a USB flash drive is an excellent way to revolutionize your computing experience. With its lightweight design, fast performance, and easy installation process, Puppy Linux is an operating system that should not be overlooked. Follow the steps outlined in this article, and you will be able to install Puppy Linux on a USB flash drive like a pro. So go ahead and give it a try!

{{< youtube Iqj6JJjC1yw >}} 



Puppy Linux is a family of distributions that provide a simple way to use Linux on lower-end machines. Unlike regular distros, Puppy Linux uses popular versions of existing distributions and it modifies them to run with lower system requirements.
 
This allows you to install this distribution on just about any system and storage medium possible. For example, you can install and boot a working copy of the latest version of Puppy Linux on a 512MB flash drive. This article shows you how you can do just that.
 
## Why Use Puppy Linux
 
One of the biggest advantages of Puppy Linux is its ability to completely load and run from your machine’s memory.
 
The way it works is that it separates the system into two parts:
 
- A read-only file system that contains all the default settings and programs. This loads into memory and starts the initial distribution.Any user files and modifications are placed in a “Save file” on your disk. This file then loads after and modifies the live system in your machine’s memory.

 
This approach ensures that your system is both lightweight and secure. For example, you can install Puppy Linux on a small flash disk and place your “Save file” on a separate larger drive. This will prevent bad actors from seeing any of your data if they end up loading the distribution.
 
Lastly, the developers of Puppy Linux designed the system to be usable out of the box. This means that you can start doing your work as soon as it is booted up.
 
## Obtaining Puppy Linux
 
You can obtain a copy of Puppy Linux by going to the project’s download page. In here, you can choose between three general “flavors” of this distribution:
 
- FossaPup, BionicPup, XenialPup and TahrPup are all flavors of Puppy Linux that uses Ubuntu LTS as its base. All these versions use apt and are compatible with any program that runs in Ubuntu.RasPup uses Raspbian as its base. This is meant for you to run Puppy Linux on a Raspberry Pi.SlackoPup uses Slackware as its base. This is a flexible version of Puppy Linux that you can customize to your own needs.

 
For the purpose of this article, we are going to use FossaPup64 since it closely matches Ubuntu 20.04 LTS.
 
Once you’ve downloaded the software, you can proceed to writing the ISO file to your device by using balenaEtcher to create a bootable flash drive.
 
## Booting Up the Puppy Linux Installer
 
- Insert your bootable USB drive to your PC and boot it up. You can do so by accessing your computer’s Boot Menu and manually select your device. We’re booting from a Lenovo Thinkpad using the F12  key.

 
- The GRUB menu will load up showing the system modes that Puppy Linux can boot into. In this menu select “fossapup64 9.5.”

 
- Once the distribution is done booting, it will display a small “Quick Start” window from where you can set your system preferences. For the most part, you can leave these settings on default and click “OK.”

 
## Installing Puppy Linux
 
While Puppy Linux is perfectly usable as a live system, it is also possible to run it on a separate USB flash drive. This is useful in cases where you want a quick and easy way to duplicate your installation.
 
- Press right-click on the live disk’s desktop and select “System -> Gparted” to format the disk.

 
- Once Gparted is running, you need to choose the disk that you want to install the distribution on. In this example, it’s “/dev/sda.”

 
- Next, you should delete any existing partitions in your disk. Click on “Device -> Create Partition Table” from the menu bar at the top.

 
- Select the new format of your disk. To make sure that that your disk is compatible with Puppy Linux, you need to select “gpt.”

 
### Preparing the Partition Layout
 
- You can now create the basic partition layout for Puppy Linux. Press right-click on the “unallocated” partition and select “New.”

 
- Create a small partition that will contain all the EFI data for your BIOS. Set the “New size” option to 100 MiB, the file system to “fat32” and write “EFI” on the “Label” text field.

 
- Make sure that this partition is bootable. Right-click on the new partition and select “Manage Flags.” Inside, check the “Boot” option.

 
- Next, select a dedicated root partition. Similar to the EFI partition, right-click on an “unallocated” space and select “New.”

 
- For the root partition, set the “New size” option to the amount of space in MiB that you want Puppy Linux to take. For example, if you want to dedicate 8GB, write 8000 MiB.

 
- Finally, you need to set the file system of the root partition to “ext3” and write “linux” on the “Label” text field.

 
### Installing FrugalPup
 
You can now start installing to your USB flash disk through FrugalPup. This is a program that copies all the system files from live session to a different storage medium.
 
- To begin using FrugalPup, press right-click on the live disk’s desktop and select “Setup -> FrugalPup.”

 
- This will bring up a small window where you can either install or update an existing Puppy Linux disk. To create a new install, press “Puppy.”

 
- Select where you want to get the installation files for your disk. Click on “this.”

 
- Pick where you want to copy the installation files. We selected “sda2” since it is our root partition.

 
- Decide where in the drive do you want to copy the installation files. Puppy Linux does not need any special directory to install to. For instance, you can press “Create Folder” and name it anything you want.

 
### Installing the Puppy Linux Bootloader
 
- The installer will now bring you back to the main menu. Press on “Boot.”

 
- FrugalPup will let you choose where you want to install the bootloader. For this, you also need to select your root partition.

 
- Provide the installation directory that you made earlier. We named it “maketecheasier.”

 
- Select the location of the disk’s EFI partition. For us, it is “/dev/sda1.”

 
- The installer will print the changes that you are making. Confirm them by pressing “OK.”

 
## Frequently Asked Questions
 
Image credit: Ali Zolghadr via Unsplash All screenshots by Ramces Red.
 
### Puppy Linux is throwing a kernel panic error. How do I fix this?
 
This is most likely due to an ACPI error with your computer. By default, some versions of Puppy Linux do not have proper ACPI support. To fix this, you need to disable this feature in your computer’s BIOS. In most cases, ACPI is located either under the computer’s chipset or CPU-related settings.
 
One important thing to note is that disabling ACPI will also disable any power saving features for your computer. This can be issue if you are installing the distribution on a portable laptop. 
 
### I am using a Non-EFI system. Is it still possible to install Puppy Linux on my machine?
 
Yes! You can install Puppy Linux even on older machines that use the Legacy BIOS (MBR) system. To do this, you only need to create a single root partition while preparing your disk.
 
Further, you also need to run the GRUB4DOS program instead of using FrugalPup to generate the boot partition. You can access this utility by pressing right-click on the live desktop and selecting “Setup -> grub4dos.”
 
### Is it possible to replace the default desktop environment in Puppy Linux?
 
Sadly, no. By default, Puppy Linux uses a simple desktop environment to make sure that the entire operating system can easily load from memory. It is possible to install a new desktop environment through Puppy’s Package Manager. However, the distribution will not be able to load these on startup.
 
Ramces is a technology writer that lived with computers all his life. A prolific reader and a student of Anthropology, he is an eccentric character that writes articles about Linux and anything *nix.
 
Our latest tutorials delivered straight to your inbox




