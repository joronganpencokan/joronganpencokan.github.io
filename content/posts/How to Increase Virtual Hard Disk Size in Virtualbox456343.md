---
title: "Unlock More Storage Heaven: Learn How to Skyrocket Virtual Hard Disk Size in Virtualbox in A Few Simple Steps!"
ShowToc: true 
date: "2023-01-24"
author: "David Gregory"
---
*****
+++ 
title = "Unlock More Storage Heaven: Learn How to Skyrocket Virtual Hard Disk Size in VirtualBox in A Few Simple Steps!" 
date = "2021-08-23" 
author = "VirtualMachineExpert" 
cover = "https://images.unsplash.com/photo-1606121481761-f28f24061574?ixlib=rb-1.2.1&auto=format&fit=crop&w=634&q=80" 
description = "Want to create more storage space in your VirtualBox VM? Follow these simple steps to skyrocket your virtual hard disk size and unlock more storage heaven!" 
categories = ["Virtualization", "VirtualBox", "Storage"] 
tags = ["Virtualization", "VirtualBox", "Storage", "Virtual Hard Disk", "Resize"] 
+++

Are you running low on storage space in your VirtualBox virtual machine? Don't worry; you don't need to delete any files or uninstall any programs. With a few simple steps, you can skyrocket your virtual hard disk size and unlock more storage heaven!

In this article, you'll learn how to resize your virtual hard disk in VirtualBox. Follow along with these simple steps to get more storage space in no time.

Step 1: Shut Down Your Virtual Machine

Before you can resize your virtual hard disk, you must shut down your virtual machine. Go to the VirtualBox Manager, select your virtual machine, and click on the "Close" button in the upper-right corner of the window. Then select "Power off the machine" and click "OK."

Step 2: Open the Virtual Media Manager

Once your virtual machine is shut down, select it in the VirtualBox Manager and click on the "Settings" button. In the settings window, click on "Storage" in the left sidebar. Then click on the virtual hard disk that you want to resize and click on the "Attributes" button in the right pane.

In the "Attributes" window that appears, click on the "Copy" button next to the location of the virtual hard disk, and then click on the "Close" button.

Now click on the "Virtual Media Manager" button at the bottom of the window. This will open the Virtual Media Manager.

Step 3: Increase the Virtual Hard Disk Size

In the Virtual Media Manager, select the virtual hard disk that you want to resize and click on the "Modify" button.

In the "Modify Virtual Hard Disk" window that appears, you can increase the size of the virtual hard disk by dragging the slider or entering a new value in the "Size" field. Keep in mind that the size must be greater than the current size of the virtual hard disk.

After you've increased the size, click on the "OK" button to close the window.

Step 4: Apply the Changes to Your Virtual Machine

You're almost done! Now you just need to apply the changes to your virtual machine.

In the "Settings" window for your virtual machine, click on the "Storage" section in the left sidebar. Then click on the virtual hard disk that you just resized and click on the "Remove Attachment" button.

Next, click on the "Add Hard Disk" button and select "Choose Existing Disk." Browse to the location of the virtual hard disk that you just resized and select it. Then click on the "OK" button.

Finally, click on the "OK" button in the "Settings" window to apply the changes to your virtual machine.

Step 5: Start Your Virtual Machine

You're all done! Start your virtual machine, and you should see the new storage space reflected in your operating system.

Now you have more space to install programs, save files, and work without worrying about running out of storage.

Conclusion

With these few steps, you can easily resize your virtual hard disk in VirtualBox and unlock more storage heaven. Don't let a lack of storage space hold you back from running your virtual machine smoothly. Use these simple steps to get the storage you need and keep working without interruption.

{{< youtube 7Aqx-VHv2_k >}} 



When you first create a virtual machine in your Virtualbox, it will always prompt you to create a new virtual hard disk. While creating the hard disk, most people will opt for the default storage space (20GB). However, if you are using it as frequent as me, you will find that the 20GB of storage space get filled up very quickly. If you are looking to increase the virtual hard disk size, here is how you can do it.

If you are using a Linux host, open the terminal. For WIndows, open the command prompt. Type the following:
 
The “x” in the command is the amount of space (in megabyte) that you want to resize to. For example, if you want to resize from 20GB to 30GB, the command is:
 
Press Enter. You should see the progress bar. When it reaches 100%, the resizing process is completed. 
 

 
The next step is to get the respective OS to recognize the increase in storage space.
 
## For Windows Guest
 
In your Virtualbox screen, you should be able to see that the virtual size has increased, but when you run the OS, it will still show the old partition size. 
 
In your Windows OS, Click on Start and type “partition” in the search bar. In Windows 8, you can perform a search using the “Search” icon in the sidebar, but you will need to select the “Settings” option.
 
Select the “Create and format hard disk partitions” option.
 
In the screen that show up, you should see a new blank unallocated partition at the right of the active partition. 
 
Right click on the active partition and select “Extend Volume”. 
 
Click Next.
 
That’s it. In your Windows Explorer, you should be able to verify that the hard drive has increased in size. 
 
## For Linux Guest
 
Depending on your hard drive setup, it can be a difficult (or easy) task to extend the active partition. If all you want is to add extra space to store your files, it is easier to format the newly created space and access it as an external partition in Ubuntu.
 
Start the Linux VM. Install Partition Editor app. 
 
Run GParted. You should see an unallocated partition. Right click on the unallocated partition and select “New”. 
 
For the file system, I chose “FAT32” since it is well supported by both Linux and Windows. You can also choose ext2/3/4. Click Ok.
 
Click the “Tick” button at the top to apply the changes. 
 
Once that is done, you can open your file manager and mount the newly created partition.
 
That’s it. You can make use of the external partition to store your things now.
 
If you are looking to shrink your VM instead, here is the tutorial.
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




