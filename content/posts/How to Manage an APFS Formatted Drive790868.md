---
title: "Unlock the Secret to Flawlessly Managing Your APFS Formatted Drive with These Simple Tricks!"
ShowToc: true 
date: "2023-02-04"
author: "David Honeywell"
---
*****
Title: Unlock the Secret to Flawlessly Managing Your APFS Formatted Drive with These Simple Tricks!

Introduction:
As a modern Mac user, you must be well aware of the APFS (Apple File System), which is the default file system in recent macOS versions. APFS is a reliable and efficient file system that has made it easier for us to manage our files and perform various tasks on our Macs. However, managing an APFS formatted drive can be a bit challenging if you are not familiar with the tricks and tips. That's why we have come up with some simple tricks to help you manage your APFS formatted drive flawlessly.

Trick 1: Create a Backup of Your APFS Drive
Before you start managing your APFS drive, it's always advisable to create a backup of your data. There are several ways to back up your APFS drive, including Time Machine, disk cloning, and cloud backup. Time Machine is built into the macOS, and it's the easiest and most convenient method to backup your data. You can also Use third-party cloning software like Carbon Copy Cloner or SuperDuper! to backup your APFS drive.

Trick 2: Use Disk Utility to Manage APFS Drive
Disk Utility is a built-in utility in macOS that allows you to manage and maintain your APFS drive. You can use Disk Utility to format your drive, repair disk errors, create, resize, and delete partitions, and much more. To access Disk Utility, go to the Applications folder, then Utilities, and finally, launch Disk Utility. Here, you can select your APFS drive and perform the necessary actions.

Trick 3: Use Terminal to Manage APFS Drive
Terminal is a command-line interface that allows you to perform advanced tasks on your Mac, including managing your APFS drive. Using Terminal, you can perform tasks such as creating, deleting, and resizing partitions, mounting and unmounting disks, and much more. However, to use Terminal, you need to have some knowledge of the commands. You can find a list of useful commands online or refer to the macOS user guide.

Trick 4: Use Third-Party Tools to Manage APFS Drive
Several third-party tools can also help you manage your APFS drive efficiently. By using these tools, you can perform advanced tasks like deleting files permanently, monitoring your disk usage, and recovering lost data. Some of the popular third-party tools for managing APFS drives include Stellar Data Recovery, Disk Drill, and DaisyDisk.

Conclusion:
Managing an APFS-formatted drive can be a bit challenging, but with the above tricks and tips, you can do it with ease. Remember to create a backup of your data before performing any tasks on your APFS drive. Use Disk Utility or Terminal to manage your drive, or consider using third-party tools to make your tasks even easier. Start managing your APFS drive like a pro today!

{{< youtube RuGGWVT39-U >}} 




APFS (Apple File System) brings new concepts for formatting and managing your Mac's drives. Among these is working with containers that can dynamically share free space with any volumes contained within them.

 

To get the most out of the new file system, learn how to format drives with APFS; create, resize, and delete containers; and create APFS volumes that have no size specified using Disk Utility.

 

For additional information on Disk Utility or if you need to work with HFS+ (Hierarchical File System Plus) formatted drives, learn how to use Disk Utility in macOS. It is also a good idea to learn more about APFS and disk types.

 
##   Format a Drive With APFS  
 

Using APFS as a disk format has a few restrictions you should be aware of:

 
Information in this article applies to macOS Catalina (10.15) through macOS High Sierra (10.13).
 
- Time Machine drives must be formatted as HFS+. Do not format or convert a Time Machine drive to APFS.
 - Apple does not recommend using APFS on standard rotational hard drives. APFS is best used on solid-state drives.
 - If you encrypt a drive using macOS High Sierra or later, the drive is converted to APFS encrypted format. Be careful when doing this, as some apps and utilities such as Time Machine do not work with the APFS format.

 

Here's a look at how to format a drive to use APFS.

 
Formatting a drive will result in the loss of all data contained on the disk. Be sure you have a current backup.
 
- Launch Disk Utility, located in /Applications/Utilities/.
 - From the Disk Utility toolbar, select the View button and choose Show All Devices.
 - In the sidebar, select the drive you want to format with APFS. The sidebar shows all drives, containers, and volumes. The drive is the first entry at the top of each hierarchal tree.
 - In the Disk Utility toolbar, select Erase.
 - A sheet drops down where you choose the type of format. Use the Format drop-down menu to select one of the available APFS formats.
 - Select GUID Partition Map as the formatting Scheme to use. You can select other schemes for use with Windows or older Macs.
 - Provide a name. The name will be used for the single volume that is always created when formatting a drive. You can add additional volumes or delete this volume later using the Create, Resize, and Delete Volumes instructions in this guide.
 - When you have made your choices, select Erase.
 - A sheet drops down and displays a progress bar. When the formatting is complete, select Done. The sidebar shows that an APFS container and a volume have been created.

 
##   Convert an HFS+ Drive to APFS Without Losing Data  
 

You can convert an existing volume to use the APFS format without losing information already present. Make a backup of your data. If something goes wrong while converting to APFS, you could lose the data.

 

Launch Disk Utility, located in /Applications/Utilities/.

 

From the Disk Utility toolbar, select the View button and choose Show All Devices.

 

In the sidebar, select the drive you want to format with APFS. The sidebar shows all drives, containers, and volumes. The drive is the first entry at the top of each hierarchal tree.

 

In the Disk Utility toolbar, select Erase.

 

A sheet drops down where you choose the type of format. Use the Format drop-down menu to select one of the available APFS formats.

 

Select GUID Partition Map as the formatting Scheme to use. You can select other schemes for use with Windows or older Macs.

 

Provide a name. The name will be used for the single volume that is always created when formatting a drive. You can add additional volumes or delete this volume later using the Create, Resize, and Delete Volumes instructions in this guide.

 

When you have made your choices, select Erase.

 

A sheet drops down and displays a progress bar. When the formatting is complete, select Done. The sidebar shows that an APFS container and a volume have been created.

 
- In the Disk Utility sidebar, select the HFS+ volume you want to convert. The volume is the last item in the drive's hierarchical tree.
 - From the Edit menu, select Convert to APFS.
 - A sheet displays a warning that you are about to change the format and that the change to APFS can't be undone without losing data. If this is OK, select Convert.

 
##   Create Containers for an APFS Formatted Drive  
 

APFS brings a new concept to the format architecture of a drive. One feature included in APFS is its ability to change the size of a volume dynamically to meet the user's needs.

 

In the Disk Utility sidebar, select the HFS+ volume you want to convert. The volume is the last item in the drive's hierarchical tree.

 

From the Edit menu, select Convert to APFS.

 

A sheet displays a warning that you are about to change the format and that the change to APFS can't be undone without losing data. If this is OK, select Convert.

 

With the older HFS+ file system, you formatted a drive into one or more volumes. Each volume had a set size determined at the time of its creation. While, under certain conditions, a volume could be resized without losing information, those conditions often did not apply to the volume you needed to enlarge.

 

APFS does away with most of those old resizing restrictions by allowing volumes to acquire any of the unused space available on an APFS formatted drive. The shared unused space can be assigned to any volume where it is needed without worrying about where the free space is physically stored—with one exception. The volumes and any free space must be within the same container.

 

Apple calls this feature Space Sharing. It allows multiple volumes, regardless of the file system they may be using, to share the available free space within the container.

 

You can also pre-assign volume sizes and specify minimum or maximum volume sizes as well.

 
##   Create an APFS Container  
 

Containers can only be created on APFS formatted drives. Here's how:

 
- Launch Disk Utility located in /Applications/Utilities/.
 - In the Disk Utility window that opens, select View and then select Show All Devices from the drop-down list. The Disk Utility sidebar changes to show physical drives, containers, and volumes. The default for Disk Utility is to show volumes in the sidebar.
 - Select the drive you want to add a container to. In the sidebar, the physical drive occupies the top of the hierarchical tree. Below the drive, you see containers and volumes listed (if present). An APFS formatted drive has at least one container. This process adds an additional container.
 - With the drive selected, choose Partition from the Disk Utility toolbar.
 - A sheet drops down asking if you want to add a volume to the current container or partition the device. Select Partition.
 - The partition map appears, displaying a pie chart of the current partitions. To add an additional container, select the plus icon (+).
 - Give the new container a name, select a format, and give the container a size. Because Disk Utility uses the same partition map interface for creating volumes and containers, it can be confusing. The name will apply to a volume that is automatically created within the new container. The format type refers to the volume, and the size you select will be the size of the new container.
 - Make your choices and select Apply.
 - A drop-down sheet appears listing the changes that will occur. If it looks OK, select Partition.

 

At this point, you have created a new container that includes a single volume taking up most of the space within. You can now use the Create Volumes section to modify, add, or remove volumes within a container.

 

Launch Disk Utility located in /Applications/Utilities/.

 

In the Disk Utility window that opens, select View and then select Show All Devices from the drop-down list. The Disk Utility sidebar changes to show physical drives, containers, and volumes. The default for Disk Utility is to show volumes in the sidebar.

 

Select the drive you want to add a container to. In the sidebar, the physical drive occupies the top of the hierarchical tree. Below the drive, you see containers and volumes listed (if present). An APFS formatted drive has at least one container. This process adds an additional container.

 

With the drive selected, choose Partition from the Disk Utility toolbar.

 

A sheet drops down asking if you want to add a volume to the current container or partition the device. Select Partition.

 

The partition map appears, displaying a pie chart of the current partitions. To add an additional container, select the plus icon (+).

 

Give the new container a name, select a format, and give the container a size. Because Disk Utility uses the same partition map interface for creating volumes and containers, it can be confusing. The name will apply to a volume that is automatically created within the new container. The format type refers to the volume, and the size you select will be the size of the new container.

 

Make your choices and select Apply.

 

A drop-down sheet appears listing the changes that will occur. If it looks OK, select Partition.

 
##   Delete a Container  
 

Follow these steps to delete a container.

 
- Follow steps 1 through 5 in the Create an APFS Container section above to display the partition map.
 - Select the partition or container you want to remove. Any volumes in the container will also be deleted.
 - Select the minus icon (-) and then select Apply.
 - A drop-down sheet lists what is about to happen. Select Partition if everything looks OK.

 
##   Create, Delete, and Resize Volumes  
 

Containers share their space with one or more volumes contained within. When you create, resize, or delete a volume, it is always referenced to a specific container.

 

Follow steps 1 through 5 in the Create an APFS Container section above to display the partition map.

 

Select the partition or container you want to remove. Any volumes in the container will also be deleted.

 

Select the minus icon (-) and then select Apply.

 

A drop-down sheet lists what is about to happen. Select Partition if everything looks OK.

 
###   How to Create a Volume  
 
- With Disk Utility open (Follow steps 1 through 3 of Creating Containers for an APFS Formatted Drive), select from the sidebar the container you want to create a new volume in.
 - From the Disk Utility toolbar, select Add Volume or Add APFS Volume from the Edit menu.
 - A sheet drops down where you give the new volume a name and specify the volume's format. After you have a name and format selected, select Size Options.
 - Size options allow you to set a reserve Size. This is the minimum size the volume will have. Enter the Reserve Size. The Quota Size sets the maximum size the volume is allowed to expand to. Both values are optional.
 - If no reserve size is set, the volume is only as large as the amount of data it contains. If no quota size is set, the volume size limit is based on the container size and the amount of space taken up by other volumes in the same container. The free space in a container is shared by all volumes.
 - Make your choices and select OK. Then, select Add.

 
###   How to Remove a Volume  
 
- Select the volume you wish to remove from the Disk Utility sidebar.
 - From the Disk Utility toolbar, select the minus icon (-) or choose Delete APFS Volume from the Edit menu.
 - A sheet drops down, warning you about what is about to occur. Select Delete to continue the removal process.

 
###   Resizing Is Unnecessary  
 

Because any free space within a container is automatically shared with all APFS volumes within the container, there is no need to force the resizing of a volume as was done with HFS+ volumes. Deleting data from one volume within a container makes that newly freed up space available to all volumes.

 

With Disk Utility open (Follow steps 1 through 3 of Creating Containers for an APFS Formatted Drive), select from the sidebar the container you want to create a new volume in.

 

From the Disk Utility toolbar, select Add Volume or Add APFS Volume from the Edit menu.

 

A sheet drops down where you give the new volume a name and specify the volume's format. After you have a name and format selected, select Size Options.

 

Size options allow you to set a reserve Size. This is the minimum size the volume will have. Enter the Reserve Size. The Quota Size sets the maximum size the volume is allowed to expand to. Both values are optional.

 

If no reserve size is set, the volume is only as large as the amount of data it contains. If no quota size is set, the volume size limit is based on the container size and the amount of space taken up by other volumes in the same container. The free space in a container is shared by all volumes.

 

Make your choices and select OK. Then, select Add.

 

Select the volume you wish to remove from the Disk Utility sidebar.

 

From the Disk Utility toolbar, select the minus icon (-) or choose Delete APFS Volume from the Edit menu.

 

A sheet drops down, warning you about what is about to occur. Select Delete to continue the removal process.

 

Get the Latest Tech News Delivered Every Day




