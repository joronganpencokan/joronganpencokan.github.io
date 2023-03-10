---
title: "Revamp Your Ubuntu Experience: Learn How to Effortlessly Move Your Home Folder for Enhanced Performance!"
ShowToc: true 
date: "2023-04-06"
author: "Arlene Pickett"
---
*****
Revamp Your Ubuntu Experience: Learn How to Effortlessly Move Your Home Folder for Enhanced Performance!

Ubuntu is an open-source operating system that has grown in popularity over the years due to its user-friendly interface and various features that cater to the needs of both casual and power users. However, Ubuntu may not always perform as efficiently as users want it to be, especially when the home folder is located on the same partition as the operating system. This can significantly slow down the system and make it prone to crashes and errors.

Luckily, Ubuntu comes with an easy solution to this problem: moving your home folder to a separate partition. This process is straightforward and can be done with just a few lines of code. By doing so, you can improve the overall performance of your system and enjoy a seamless Ubuntu experience.

If you're interested in revamping your Ubuntu experience, here is a step-by-step guide on how to move your home folder to a separate partition:

Step 1: Create a New Partition

The first step is to create a new partition where you'll move your home folder. To do this, open the Terminal and enter the following command:

sudo fdisk /dev/sdb

Replace 'sdb' with the name of the disk you want to partition. Once you're in the fdisk command line interface, press 'n' to create a new partition. Follow the on-screen prompts to set the partition size and file system.

Step 2: Mount the New Partition

Once you have created the new partition, you need to mount it so you can use it. In the Terminal, enter the command:

sudo mkdir /mnt/newhome

This creates a new directory called 'newhome' in the '/mnt' folder. Next, mount the new partition by entering the command:

sudo mount /dev/sdb1 /mnt/newhome

Again, replace 'sdb1' with the name of your new partition.

Step 3: Copy Your Home Folder

Now that you have a new partition and it's mounted, you can copy your entire home folder to it. Use the following command:

sudo rsync -av --exclude='.gvfs' /home/ /mnt/newhome

This may take some time, depending on the size of your home folder.

Step 4: Rename the Old Home Folder

Once you have copied your home folder to the new partition, you need to rename the old home folder with a different name. This is necessary to prevent the system from trying to use the old home folder when you log in. Use the following command to rename the old home folder:

sudo mv /home /old_home

Step 5: Mount the New Home Folder

Finally, you need to make the new home folder available to the system. Use the following command to mount the new home folder:

sudo mount /dev/sdb1 /home

Now, when you log in, Ubuntu will automatically use the new partition as your home folder.

In conclusion, moving your home folder to a separate partition is a simple yet effective way to enhance the performance of your Ubuntu system. With these easy-to-follow steps, you'll be able to efficiently move your home folder and optimize your Ubuntu experience. Happy computing!

{{< youtube MtBf1jp8x34 >}} 



If you have accepted the default option while installing Ubuntu, or that your computer comes with Ubuntu pre-installed, chances are that your Home folder and the system folders all lie in the same partition. This is perfectly fine, but if you want to upgrade your existing Ubuntu version, or reinstall Ubuntu, you won’t be able to preserve your app settings, or even retain your files and documents. One of the good practice is to give the Home folder its own partition, so whatever changes you made to the System folder won’t affect your Home directory, and you can easily upgrade or reinstall Ubuntu with ease. 
 
If you want to move your Home folder to another partition, here is how you can do so.
 
## Creating a new partition
 
Note: You can skip this step if you already has an existing external partition that you can use. 
 
Assuming that your computer has only one hard disk and it contains only one partition. To create a new partition, you have to first obtain a Ubuntu Live CD/USB and boot into it. You can’t partition the hard disk when it is running. 
 
Once you are booted into the Live session, open the app “GParted”. Select the hard disk from the list. It should be labelled something like “sda”.
 

 
You should see a number of entries in the list. Select the entry that corresponds to the main partition. It should be the one with the biggest file size and is either in the ext3 or ext4 filesystem format. Right click on it and select “Resize/Move”.
 
Set the size for the new partition in the “Free Space Following” field. The number is represented in MB, so if you want to set aside 10GB for the new partition, enter “10000”. You will notice that as you enter the number, the number in the “New Size” field will decrease accordingly. My usual practice is to set aside 10GB for the system files and allocate the rest to the Home partition.  Click “Resize/Move”.
 
Back to the GParted main screen, you should now see a new “Unallocated” entry with the file size that you have set earlier. Right click on it and select “New”. Select “ext4” as the filesystem and click “Add”. 
 
Lastly. click the green check button to apply the changes. Depending on your hard disk size, the resizing process might take a long time
 
After the process is completed, you should see something like the screen below. Record down the new partition number.
 
Now shut down the live session, remove the live CD/USB and boot up the computer.
 
## Migrating the Home folder
 
To migrate your current Home folder to an external partition, there are four things that you need to do:
 
- Mount the external partition onto a temporary Home location.
 - Copy the files from your current Home folder to this temporary Home folder.
 - Relocate the current Home folder
 - Mount the new Home folder.

 
### 1. Create a temporary Home folder
 
 Open a terminal and type the following:
 
This will display the UID of all the partitions. Record down the UUID for the partition that you have created earlier. 
 
Next, open the fstab file:
 
and add the following line to the end of the file.
 
Replace the UUID with the UUID value of the external partition.
 
Save (Ctrl + o) and exit (ctrl + x) the file. 
 
Next, create a mount point:
 
and reload the updated fstab.
 
You should now see a “home” folder in the Media directory. 
 
### 2. Copy the files from your current Home folder to the new Home folder
 
The next thing we are going to do is to copy all the files from the current Home folder to the new Home folder. You can simply do a “Select all”, “Copy” and “Paste” to transfer all the files to the new Home folder. However, you might be missing out the hidden files and some of the file permissions might not be preserved. A more complete method would be using rsync.
 
### 3. Relocate the current Home folder
 
Once we have set up the new Home folder, we need to remove the existing Home folder to make way for the new Home folder in the external partition. To do that, type the following commands in the terminal:
 
What the above commands do is to move the existing Home folder to Home_backup, and create an empty Home folder for the new Home folder to mount to.
 
### 4. Mount the new Home folder
 
The last step to complete the migration is to mount the new Home folder as “/home”. To do that, we have to revisit the fstab file again.
 
All you have to do is to change the “/media/home” to “/home”. Save and exit the file.
 
Lastly, reload the fstab file:
 
That’s it. You have now migrated your Home folder to an external partition. 
 
Optional: removing the Home_backup folder
 
Once you are done with the migration, you can either use the old Home folder as a backup, or remove it to release the storage space. To remove it, use the command:
 
Let us know in the comments if you encountered any difficulty. 
 
Image credit: Moving House – Kiwi Style
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




