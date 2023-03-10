---
title: "Unleash the Power of Ubuntu: Learn How to Create a Bootable USB in Windows Now!"
ShowToc: true 
date: "2022-12-06"
author: "Lorena Freeland"
---
*****
# Unleash the Power of Ubuntu: Learn How to Create a Bootable USB in Windows Now!

Are you tired of carrying around installation disks or searching for a CD/DVD drive every time you need to install Ubuntu? Did you know that you can create a bootable USB drive with Ubuntu on it instead? In this article, we will show you how to create a bootable USB drive with Ubuntu on it using Windows.

## What is a Bootable USB Drive?

A bootable USB drive is a removable storage device that contains an operating system and can be used to boot a computer. A bootable USB drive is an excellent tool for installing or using an operating system on a computer without a CD/DVD drive or the need for installation disks.

## Why Create a Bootable USB Drive with Ubuntu?

Ubuntu is a popular and user-friendly operating system that offers many benefits. It is free, stable, secure, and offers a wide range of software applications. By creating a bootable USB drive with Ubuntu on it, you can carry your entire operating system with you wherever you go. This means that you can use your favorite applications and work anywhere, without having to worry about the limitations of the operating system on the computer you are using.

## Creating a Bootable USB Drive with Ubuntu

Creating a bootable USB drive with Ubuntu on it is a simple process that can be done in a few easy steps. The following guide will show you how to create a bootable Ubuntu USB drive using Windows.

### Step 1: Download the Ubuntu ISO file

The first step is to download the Ubuntu ISO file from the official Ubuntu website. You can download the latest version of Ubuntu from [here](https://ubuntu.com/download).

### Step 2: Download and Install Rufus

The next step is to download and install Rufus, a free and open-source tool for creating bootable USB drives. You can download Rufus from [here](https://rufus.ie/).

### Step 3: Insert the USB Drive

Insert a USB drive into the computer with enough space to store the Ubuntu ISO file.

### Step 4: Open Rufus

Open Rufus and select the USB drive you inserted in Step 3 from the "Device" dropdown.

### Step 5: Select the Ubuntu ISO File

Click on the "Select" button next to the "Boot selection" dropdown and navigate to the location on your computer where you saved the Ubuntu ISO file.

### Step 6: Set the Partition Scheme and File System

Next, set the "Partition scheme" to "MBR," and the "File system" to "FAT32." These settings ensure that the USB drive is bootable.

### Step 7: Create the Bootable USB Drive

Click on the "Start" button to create the bootable USB drive. Rufus will format the USB drive and copy the Ubuntu ISO file onto it. The process may take several minutes, depending on the size of the ISO file and the speed of the USB drive.

### Step 8: Boot from the USB Drive

Once Rufus has finished copying the Ubuntu ISO file onto the USB drive, you can now use it to boot your computer. To boot from the USB drive, insert it into the computer and restart your computer. Depending on the computer, you may need to change the boot order in the BIOS to boot from the USB drive.

## Conclusion

Creating a bootable USB drive with Ubuntu on it is a simple and effective way to carry your operating system with you wherever you go. With the steps outlined in this article, you can easily create a bootable USB drive with Ubuntu on it, without the need for installation disks or a CD/DVD drive. So, unleash the power of Ubuntu and start creating your bootable USB drive today!

{{< youtube rJQk9KVekFI >}} 



A full transition from Windows to Linux may not be easy, that is why Ubuntu allows its users to test the live CD (or USB) first to see if they like it, then install it on their systems. This guide shows you how to create a bootable Ubuntu USB in Windows. Using this media, you can boot up Ubuntu on any computer, perform your tasks and leave the main OS unmodified.
 
To follow along with the guide, ensure:
 
- Internet connection to download the required tools.A USB Flash drive – at least 8GB (recommended).You have downloaded the latest version of the Ubuntu ISO from the official Ubuntu download page.

 
## Create Bootable Ubuntu USB with Rufus
 
The easiest method to create a bootable Ubuntu USB is to use Rufus. The ability to set persistence in Ubuntu USB drives is now supported in newer versions of Rufus.
 
1. Plug your USB drive into your Windows computer. Next, launch Rufus and click the “Select” button to select the Ubuntu ISO.
 
2. Set the size for your persistence file.
 
3. Configure the partition scheme.
 
4. Click “Start” to flash the ISO.
 
Once the flash process is completed, reboot the PC into your Ubuntu system.
 
## Create Bootable Ubuntu USB with UNetbootin
 
Another method to create a bootable Ubuntu USB in Windows is to use UNetbootin.
 
1. Download the UNetbootin tool from its official page.
 
2. Launch the UNetbootin tool. You may have noticed you can select the “Distribution” option, choose the distro you want to install and UNetbootin will download the ISO file for you. For this guide, we will use the “Disk Image” option since we have already downloaded the Ubuntu ISO.
 
3. Select the “three-dotted” section and navigate to the location of the downloaded Ubuntu ISO.
 
Select the Ubuntu ISO and load it into UNetbootin.
 
4. Before flashing the ISO to the USB, set up persistence. To do this, adjust the option “Space used to preserve files across reboots.” Allocate the desired space in MB.
 
Note: if you are flashing older Ubuntu ISOs, this might not work and you may need to perform a manual configuration as shown in the steps below.
 
5. In the “Type” drop-down at the bottom, make sure “USB Drive” is selected, select the Drive directory of your USB drive next to it, then click “OK” to start the process. After several minutes, the process will be complete.
 
You now have a bootable, portable Ubuntu build.
 
## Add Persistence Manually to the Bootable USB
 
In some instances, UNetbootin may fail to add the persistence. To resolve this, you can manually configure this option.
 
1. Download the Casper-RW-Creator file from the official link.
 
2. Once downloaded, launch the file and select the USB drive.
 
3. Set the persistence file.
 
Note: if you are using the Ubuntu 20.04 image, the persistence file has been renamed to writeable. However, for older images, select the persistence file as casper.
 
4. Select the size to allocate the persistence file and click “Create.”
 
5. Once the process is complete, you should have the file writeable or casper in the root of the drive for persistence.
 
To point Ubuntu to the persistence file, edit the “grub.cfg” file in “/boot/grub/grub.cfg.”
 
Find the entry:
 
Edit the file and add the casper module. The above entry should be:
 
Finally, save the file and reboot the computer into your Ubuntu session. During Boot, select the “Ubuntu” section to use the persistence file.
 
## Wrapping Up
 
You now have a bootable Ubuntu USB drive that you can take with you anywhere. It’s a great option in the way of security, ensuring you don’t have to enter and leave your data on strangers’ or public computers. As an extra measure, though, remember to password-protect your Ubuntu drive.
 
If you want to start from scratch and get yourself a blank flash drive, we can guide you through the process of formatting a USB drive in Windows. We can also show you how you to format a drive in FAT32 specifically, which isn’t possible using the native formatting tool in Windows 10.
 
John is a technical writer at MTE, when is not busy writing tech tutorials, he is staring at the screen trying to debug code.
 
Our latest tutorials delivered straight to your inbox




