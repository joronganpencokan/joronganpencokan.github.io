---
title: "Unlock the Secret to Boosting Your Virtualbox Storage Space in One Click with Clonezilla!"
ShowToc: true 
date: "2023-06-05"
author: "Treena Taylor"
---
*****
# Unlock the Secret to Boosting Your Virtual Box Storage Space in One Click with Clonezilla!

If you're a virtual machine enthusiast, you know the pain of running out of storage space in your VirtualBox. It's a frustrating experience not being able to download or install new software, or even add new data files to your project. The good news is that Clonezilla can help you unlock this problem in just one click! 

Clonezilla is a disaster recovery, disk cloning, disk imaging, and partitioning solution that is open-source and free. It's a simple yet powerful tool that provides users with the ability to clone hard disks entirely, create backups of data, and restore data backups in the case of system failure. With Clonezilla, you can copy data and applications from one disk to another disk, or one partition to another partition effortlessly.

Here are the steps you need to follow to increase your VirtualBox storage space with Clonezilla:

## Step 1: Download and Install Clonezilla

The first step is to download Clonezilla and install it on your computer. You can download it from the official Clonezilla website. Choose the appropriate version of Clonezilla that is compatible with your computer.

## Step 2: Create a Clonezilla Bootable USB

Once the Clonezilla download is complete, you need to create a bootable USB drive. You can use software like Rufus or UNetbootin to create the bootable USB drive.

## Step 3: Boot into Clonezilla

Insert the bootable USB drive into your computer and restart your computer. Access the BIOS menu, and ensure that your boot priority is set to USB. Select the USB drive and boot into Clonezilla.

## Step 4: Clone the VirtualBox Disk

Once you're booted into Clonezilla, select the "Device image" option from the main menu. Then, select the source and destination disks. In this case, you will choose the virtual disk as the source and the external hard drive as the destination. Clonezilla will start cloning your VirtualBox disk to the external hard drive.

## Step 5: Expand the VirtualBox Disk

After cloning the VirtualBox disk, you have to expand the disk size. You can achieve this by opening VirtualBox and selecting the virtual machine you want to expand. Click on "Settings," then "Storage," and then select the cloned disk. Click on the "Size" slider and increase it to your desired storage capacity.

## Step 6: Replace the Cloned Disk with the Expanded Disk

Once you've expanded the VirtualBox disk, you have to replace the cloned disk with the expanded disk. You can achieve this by creating a new disk image and selecting the expanded disk as the source. Then, you will replace the old disk image with the new expanded disk image.

Congratulations! You've successfully expanded your VirtualBox disk space with just a few clicks using Clonezilla. You can now download and install more software and data files, and continue working on your projects without any storage space restriction.

In conclusion, Clonezilla is a robust tool that provides an easy and effective solution to expand your VirtualBox disk space. With just a few clicks, you can clone your VirtualBox disk, expand it, and replace it with the expanded disk image. Get started with Clonezilla today, and take control of your VirtualBox storage space.

{{< youtube 7Aqx-VHv2_k >}} 



You finally decided to try Linux in a virtual machine. You chose and downloaded a Linux distribution that looked good, created a virtual machine, installed it, played with it, ended up loving it. And now you want to see more of this fascinating Linux Land but can’t because your virtual HDD is full. Unfortunately, there’s no easy way out of this problem.
 
You can try the conventional way – use command-line tools to expand it and a partition tool to expand the HDD size in the guest OS.
 
There is another unconventional way – expand the HDD size in Virtualbox and treat your virtual PC as a real one!
 
Instead of trying to alter the virtual machine’s HDD, we’ll do what we’d do with a “normal” PC: create and “attach” a second HDD, then use a standard, bootable version of the favorite imaging/backup tool CloneZilla to copy the contents of the old virtual HDD to the new one and then remove the old HDD, leaving you with more storage without having to deal with cryptic commands and strange failures. There is no need to back up things since your old virtual HDD will still exist if need be. As a bonus, the latest versions of CloneZilla deal with the resizing of any partitions, so if everything goes according to plan, after this you only have to swap virtual HDDs and boot your virtual PC.
 
## Resize VirtualBox HDD
 
With the approach we’ll follow, you will need to download a bootable ISO of CloneZilla (on the Host OS). You might need the bootable ISO version of GParted, too, in case the resizing process fails. 
 
1. Download CloneZilla and GParted‘s Live ISO version. Both offer different versions for different architectures, but since we’re talking about a virtual PC, most versions will work, so you don’t have to overthink which one to download.
 
You might not end up needing GParted if CloneZilla successfully resizes the partitions in your virtual HDD. Still, it’s better to have it readily available in case CloneZilla fails this step.
 
2. From VirtualBox’s main window, select from the virtual PC that’s out of storage space from the list on the left.
 
3. Visit its Settings by either clicking the gear icon, right-clicking and selecting Settings from the menu that appears or by pressing Ctrl + S on your keyboard.
 
4. Select the “Storage” options tab on the left side of its window. If you have not changed the default options, your virtual PC will typically come with two controllers. On the first one you’ll see a virtual optical drive that allows the use of ISO files as if they were “normal” optical media (CDs and DVDs). On the second one you’ll find the virtual hard drive that’s filled to the brim.
 
Select the controller with the HDD and notice that two icons appear to the right. Select the second one: “Adds hard disk.”
 
In the new pop-up window that appears, select “Create new disk” to add a second HDD to the same controller as your existing one on your virtual PC.
 
5. VirtualBox will show you a series of simple steps for adding your new, blank HDD. In the first of these, hard disk file type, you are asked to select the type of file to be used. We recommend choosing the “official” format of VirtualBox, VDI (VirtualBox Disk Image). Proceed with a click on Next.
 
You will then have to choose if you want the new disk to be “Fixed” or “Dynamic.” We suggest the “Fixed” option  that specifies that virtual disks will occupy all their space on the drives of your real computer from the beginning. If they are 20GB in size, you are losing 20GB from your computer from the get-go. The “dynamic” option specifies that virtual disks will initially take up only the space of their actual contents, expanding until they reach their full size as you use them.
 
The problem with the second option is that when the virtual disks try to expand, if you do not have the space needed on your real computer, you may encounter problems. And in this case where we’re trying to move an entire installation of an operating system from one disk to another, it’s best to try to minimize any chance of problems appearing. So, “Fixed size” it is!
 
The last step of the hard drive creation process will have you select the size of the new hard drive. You need to declare a larger size than your existing, full HDD, to be able to “move over” to the new HDD and solve the “no space left” problem. In our case, our original, full virtual HDD was 10GB in size, so we chose double that, 20GB, for the new disk. This would leave us with 10GB of usable space after cloning the old HDD into the new one.
 
Click on Create, and VirtualBox will begin creating the disk file. If you chose the “Fixed” option and a large HDD size, this procedure can take some time.
 
## Drives and controllers
 
6. After the process completes, your virtual PC will have two HDDs connected to the controller you selected before. Now, move your attention to the optical drive on the other controller. Click on it to select it and then click on the button with the disc that appears on the right of the “Optical Drive” pull-down menu. Locate and select the CloneZilla ISO you downloaded earlier.
 
7. Start your virtual machine and boot into CloneZilla. Select the first of the options, “Clonezilla live.”
 
You will be prompted to select the language used in CloneZilla’s interface and the keyboard. If you don’t need to swap languages, you can accept the default options by pressing enter in both cases. Finally, select “Start_Clonezilla” to start the application itself.
 
8. CloneZilla allows you to back up a hard drive in many ways. In our case, we will be using the “device-device” option since we want to clone the contents of our existing HDD to a new one.
 
9. In the next step, select “Expert mode” to gain access to all of CloneZilla’s options, then choose that you want to copy the entire disk, not just a partition from it, with the “disk_to_local_disk” option.
 
10. To select what will be copied where, set the smaller drive as your “Source” and the larger one as your “target.”
 
When you reach the “Advanced” options, make sure the first five are active: -g, -e1, -e2, -j2, and -r.
 
The last of them is the most important in our case, and the one that makes our approach simpler. Thanks to this -r, CloneZilla will try to automatically resize the partitions as they’re copied from the old to the new hard drive, taking advantage of its larger space. Thus, it will save you from having to run GParted or any similar program to expand them manually.
 
That is, unless a problem appears, like some incompatibility of CloneZilla with a partition’s file system, errors in the virtual HDD structure, or something like that. We’ve never met such a problem, but we’ve also never used anything more “exotic” than EXT2/3/4 for Linux and the typical FAT32/NTFS file systems for Windows OSes.
 
## Partition resizing
 
11. Generally, unless your real PC’s HDDs are busted, it’s rare for a virtual HDD to have problems in its structure. Thus, in most cases, you can safely skip checking for any errors by selecting the -sfsck option.
 
12. When asked how you want the partitions distributed, don’t select the default option. Instead, choose “-k1 Create partition table proportionally” to have CloneZilla expand the partitions and file systems as they’re copied on the new HDD to take up its whole available space.
 
13. In the last option, select that you want the virtual computer to shut down with “-pa poweroff Shutdown” when done.
 
## Cloning in action
 
14. CloneZilla will ask a series of questions to which you can answer positively, and soon the process of cloning your old virtual disk into the new one will begin.
 
Just like during the new HDD’s creation, the larger the disk is, and the more “stuff” that has to be copied from the old to the new HDD, the longer this part of the process will take.
 
## Swap the disks
 
15. When the process is complete, the computer will shut down (if you had selected the shutdown option). Select Settings again from VirtualBox’s main window, visit the Storage tab once more, and this time remove your old, full disk. Right-click on it and select “Remove Attachment.”
 
Note that this won’t delete the actual file from your real PC, so you’ll still have access to everything in case something went wrong.
 
16. Now, with your new, larger hard drive as the main drive, you can start your virtual machine as usual. If everything went according to plan, you should be able to boot and log in to your OS. Check it out by typing df in a terminal to see how much free space is available in your HDD.
 
If the disk shows up as full again, then it is likely that CloneZilla has failed to resize the partitions. You can, therefore, continue resizing them with GParted. In this case, shut down the virtual machine, insert the GParted ISO as you did before with the CloneZilla ISO, and continue as in this guide.
 
When you’re sure that everything is working correctly, you can delete the old HDD file from your real computer to gain back the space it occupies.
 
Do you prefer the conventional way or this unconventional method to increase your Virtualbox HDD size? 
 
OK's real life started at around 10, when he got his first computer - a Commodore 128. Since then, he's been melting keycaps by typing 24/7, trying to spread The Word Of Tech to anyone interested enough to listen. Or, rather, read.
 
Our latest tutorials delivered straight to your inbox




