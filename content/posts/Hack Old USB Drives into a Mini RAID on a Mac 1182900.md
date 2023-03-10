---
title: "Transform Your Old Useless USB Drives into a Powerful Mac Mini RAID with this Genius Hack!"
ShowToc: true 
date: "2022-12-20"
author: "Earl Robinson"
---
*****
Transform Your Old Useless USB Drives into a Powerful Mac Mini RAID with this Genius Hack!

Do you have a bunch of old USB drives lying around that you don't use anymore? Don't throw them away yet! With a little ingenuity and the help of your Mac Mini, you can turn those useless USB drives into a powerful RAID storage system.

A RAID (Redundant Array of Inexpensive Disks) is a storage technology that combines multiple hard drives into a single logical unit for increased performance or data redundancy. In this case, we'll be creating a RAID using USB drives, which are not the fastest or most reliable storage devices, but they're certainly inexpensive.

To get started, you'll need a Mac Mini, your old USB drives, a USB hub (if you have more than four drives), and a software tool that can create a RAID. The software tool we'll be using is called SoftRAID, which is a powerful and affordable RAID solution that provides a variety of features for both Mac and PC users.

Here's how to create a Mac Mini RAID using your old USB drives:

Step 1: Organize your USB drives
First, collect all your old USB drives and connect them to your Mac Mini using a USB hub. Make sure they're all empty and formatted correctly. It's important to note that all the USB drives should have the same capacity because the RAID will use the lowest capacity of all the drives.

Step 2: Install SoftRAID
Next, download SoftRAID and install it on your Mac Mini. This software allows you to create and manage RAID volumes in various configurations, including RAID 0 (striping) for maximum performance, RAID 1 (mirroring) for data redundancy, or RAID 5 and RAID 6 for a balance of performance and data protection.

Step 3: Create your RAID
Open SoftRAID and select the "Create Volume" button in the main window. Choose the RAID configuration that suits your needs and name your volume. Select the USB drives that you want to include in the RAID and click the "Create" button.

Step 4: Optional settings
You can now set various options for your RAID volume, such as block size, stripe size, and cache size. These settings will determine the performance and efficiency of your RAID volume.

Step 5: Format your RAID
Once you've created your RAID volume, you'll need to format it for your Mac to recognize and use it. Open the Disk Utility app and select your RAID volume. Click the "Erase" button and choose the file system format you prefer.

Step 6: Enjoy your new RAID
That's it! Now you can enjoy the benefits of a RAID system without spending a fortune on expensive hard drives. Your old USB drives have now become a reliable storage solution for your Mac Mini.

Conclusion

Turning your old USB drives into a Mac Mini RAID may not give you the fastest or most reliable storage system, but it's an excellent way to use what you already have and save money. By following these steps and using SoftRAID software, you can create a RAID volume that suits your needs and provides the peace of mind that comes with data redundancy. Give it a try and see how much you can save!

{{< youtube 6LqFY5yymKQ >}} 



Most of us have a lot of old USB thumb drives lying around. Sometimes you just got a new larger capacity or less grubby looking one, but often you just accumulate them as they are the most popular storage medium and are used and discarded as needed because they are cheap.
 
Once they have served their purpose, the ones you don’t use just sit in a drawer or on a desk until you throw them away or lose them (and you don’t even remember it existed). But what if you could combine them and make a higher capacity drive to plug into a media player in a TV or back up your USB drives that are in use?
 
This article explains how to turn old USB drives into a mini RAID to give them new life.
 
## What is RAID?
 
RAID stands for Redundant Array of Independent Disks. A RAID combines multiple drives into a single “logical unit” for the purposes of what is called data redundancy or performance improvement, so in other words, either secure, fast, big, or combos of all three.
 
Data is spread across the drives in one of several “RAID levels” depending on the intended use. Each RAID level contains different levels of error correction, distribution of data etc. but we don’t need to know all that – the three modes we will concern ourselves with here are “striped”, “mirrored” and “JBOD”.
 

 
“Striped” combines drives of equal size as a large fast unit. “Mirrored” takes one drive and copies it to all the others continuously so it is secure; the data never gets lost because it’s backed up multiple times automatically. If one drive fails, it can be replaced. JBOD (meaning “Just A Bunch Of Disks”) chains together drives of any size and makes them a continuous logical drive.
 
Obviously the mode you choose depends on the use. Striped is faster, Mirrored is the best backup but JBOD uses every drive you have and makes a big drive.
 
## Hacking a Mini RAID for Mac OS X
 
To make a collection of USB drives into a RAID on OS X is simple. First plug all the USB drives you have into a USB hub. (See above) They will all show up on the desktop.
 
Open Disk Utility either by going to “Applications -> Utilities -> Disk Utility” or from the Finder, press “Command + Shift + U” to go to the Utilities folder and start Disk Utility.
 
All the drives you have attached show up in the panel.
 
Select one of the drives you want to turn into a RAID and click the RAID tab.
 
You will be presented with a range of options: naming the RAID and which type of RAID you want to make, either mirrored, striped or concatenated (JBOD). In this case, we will select concatenated as the drives are of assorted 4Gb, 8Gb and 16Gb sizes. If they were all the same, you can use striped or mirrored. 
 
Note: you CAN use drives of different sizes in the other two modes but the drives will be partitioned to be the same size as the smallest drive.
 
Drag every drive you want to be a part of the RAID. Warning: Do this carefully as these drives will be formatted and you DON’T want to include your system drive by accident.
 
You will see the projected final size of the finished drive in the panel above the drive window.
 
Press the “Create” button and you will be warned that you are about the delete all these disks and make them into a RAID.
 
Click OK and the drives will all be unmounted, partitioned and formatted one by one.
 
When it’s finished and the drive has “spun up” . . .
 
. . . the new drive virtual unit will be displayed on the desktop ready for use.
 
## Conclusion
 
If you have a bunch of old USB drives, this is a good way to make good use of them rather than throwing them away. One thing to note is that old USB drives, especially USB 1.0, are slow, so it will take a while to copy stuff to them, but hey, you have a free SSD drive of much higher capacity than the component parts, so speed is a luxury. Obviously faster USB 3.0 drives will be better if have them.
 
Phil South has been writing about tech subjects for over 30 years. Starting out with Your Sinclair magazine in the 80s, and then MacUser and Computer Shopper. He's designed user interfaces for groundbreaking music software, been the technical editor on film making and visual effects books for Elsevier, and helped create the MTE YouTube Channel. He lives and works in South Wales, UK.
 
Our latest tutorials delivered straight to your inbox




