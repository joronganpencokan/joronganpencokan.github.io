---
title: "Unleash the Power of Linux on Windows 11! Learn How to Mount Linux File System using WSL NOW!"
ShowToc: true 
date: "2022-12-29"
author: "Gregory Berhe"
---
*****
Unleash the Power of Linux on Windows 11! Learn How to Mount Linux File System using WSL NOW!

Windows 11 has included a new feature called Windows Subsystem for Linux (WSL) that allows users to run Linux software directly within the Windows environment. This innovation means that Linux files can now be accessed and manipulated using the Windows File Explorer. This new feature is an exciting development for tech-savvy individuals who want to combine the power of the Linux operating system with the familiarity of Windows 11's user interface. 

One of the most impactful aspects of WSL is the ability to mount Linux file systems within Windows 11. By doing so, users can access and manipulate Linux files similar to how they would on a Linux system. This article aims to guide users on how to mount Linux file systems using WSL in Windows 11.

The first step in this process is to ensure that WSL is enabled on your Windows 11 system. Ensure that the “ Windows Subsystem for Linux” feature is turned on in the “Turn Windows features on or off” panel. Once enabled, install the necessary Linux distribution using the Microsoft Store app on your Windows 11 device.

After installing the Linux distribution, launch a CMD or PowerShell terminal and run the "wsl" command to open the Linux distribution in a terminal window. Once in the terminal, a user needs to identify the name of the Linux file system they wish to mount within Windows 11. 

To do so, run the command "sudo fdisk -l". This command will list out all the available partitions and file systems within the Linux distribution. Once the name of the file system has been identified, a user can proceed to mount the file system in Windows 11.

In the same terminal window, run the command "mkdir /mnt/linux" to create a mount point for the Linux file system within Windows. The mount point can be named anything the user desires. In this example, the name given is 'linux.'

To mount the Linux file system within Windows, run the following command:

"sudo mount /dev/sdaX /mnt/linux"

Replace "/dev/sdaX" with the name of the file system that was identified earlier in the terminal window.

With these steps complete, the Linux file system is mounted within Windows 11, and users can easily access their Linux files through File Explorer. This ability to mount Linux file systems within Windows 11 adds immense convenience and flexibility for users who need to access both Windows and Linux files simultaneously.

In conclusion, the WSL feature within Windows 11 has made it entirely possible to mount a Linux file system within Windows, enhancing the capabilities and versatility of the Operating System. By learning and implementing the steps mentioned above, users can unlock this feature and achieve seamless access to both Windows and Linux files. Go ahead and modify, create, or manipulate your Linux files on Windows to unleash the full capability of your computer!

{{< youtube XST1XOhEr7A >}} 



On Windows 11, the Windows Subsystem for Linux (WSL) ships with a new feature that allows you to attach and mount physical drives to access Linux file systems (for example, ext4) not natively supported on Windows.
 
The new feature allows users to access Linux files using File Explorer on a dual-boot system running Windows 11 and a Linux distro on a different drive.
 
In this guide, you will learn the steps to mount and unmount drives using the Windows Subsystem for Linux.
 
- Mount Linux file system on Windows 11
 - Mount any Linux file system on Windows 11
 - Access Linux file system on Windows 11
 - Unmount Linux file system on Windows 11

 
## Mount Linux file system on Windows 11
 
To mount a Linux file system using WSL, use these steps:
 
- Open Start on Windows 11.
 - Search for PowerShell, right-click the top result, and select the Run as administrator option.
 - Type the following command to list the available physical disks and press Enter:
 - wmic diskdrive list brief
 - Confirm the drive path under the “Device ID” column.
 - Type the following command to mount the Linux file system and press Enter:
 - wsl --mount DISKPATH
 - In the command, make sure to replace DISKPATH for the drive path with the Linux distribution you want to mount. For example, wsl --mount \\.\PHYSICALDRIVE2. If you’re going to mount a specific partition, you’ll need to use the --partition option with the partition number. For example, wsl --mount \\.\PHYSICALDRIVE2 --partition 1.

 
Once you complete the steps, the drive with Linux files will mount, and it’ll be visible from Windows 11.
 
Open Start on Windows 11.
 
Search for PowerShell, right-click the top result, and select the Run as administrator option.
 
Type the following command to list the available physical disks and press Enter:
 
wmic diskdrive list brief
 
Confirm the drive path under the “Device ID” column.
 
Type the following command to mount the Linux file system and press Enter:
 
wsl --mount DISKPATH
 

 
In the command, make sure to replace DISKPATH for the drive path with the Linux distribution you want to mount. For example, wsl --mount \\.\PHYSICALDRIVE2. If you’re going to mount a specific partition, you’ll need to use the --partition option with the partition number. For example, wsl --mount \\.\PHYSICALDRIVE2 --partition 1.
 
## Mount any Linux file system on Windows 11
 
The previous steps only attempt to mount a physical drive as ext4. If you want to specify another file system, you will need to use a different command with the Windows Subsystem for Linux 2 (WSL2).
 
To mount a specific Linux file system on Windows 11, use these steps:
 
- Open Start.
 - Search for PowerShell, right-click the top result, and select the Run as administrator option.
 - Type the following command to list the available physical disks on Windows 11 and press Enter:
 - wmic diskdrive list brief
 - Confirm the drive path under the “Device ID” column.
 - Type the following command to mount a drive and press Enter:
 - wsl --mount DISKPATH -t FILESYSTEM
 - In the command, make sure to replace DISKPATH and FILESYSTEM for the path of the Linux drive and file system you want to mount. For example, to mount a disk as fat, use this command: wsl --mount DISKPATH  -t vfat.

 
After you complete the steps, the drive with Linux files will mount, and it will be accessible using File Explorer.
 
Open Start.
 
Type the following command to list the available physical disks on Windows 11 and press Enter:
 
Type the following command to mount a drive and press Enter:
 
wsl --mount DISKPATH -t FILESYSTEM
 
In the command, make sure to replace DISKPATH and FILESYSTEM for the path of the Linux drive and file system you want to mount. For example, to mount a disk as fat, use this command: wsl --mount DISKPATH  -t vfat.
 
## Access Linux file system on Windows 11
 
To access files from a Linux file system on Windows 11, use these steps:
 
- Open File Explorer.
 - Click the Linux item from the left navigation pane.
 - In the address bar, navigate to \wsl$ and then access the mount folder. For example, \\wsl$\\DISTRO-NAME\\MOUNT-POINT.

 
Once you complete the steps, you should be able to browse the Linux files from a natively unsupported file system on Windows 11. In addition to using File Explorer, you can access file systems like “ext4” from the WSL2 console using command lines once the drive is mounted.
 
Open File Explorer.
 
Click the Linux item from the left navigation pane.
 
In the address bar, navigate to \wsl$ and then access the mount folder. For example, \\wsl$\\DISTRO-NAME\\MOUNT-POINT.
 
## Unmount Linux file system on Windows 11
 
To unmount the Linux file system on Windows 11, use these steps
 
- Open Start.
 - Search for PowerShell, right-click the top result, and select the Run as administrator option.
 - Type the following command to unmount and detach the drive and press Enter:
 - wsl --unmount DISKPATH
 - In the command, make sure to replace DISKPATH for the Device ID of the drive you want to unmount.

 
After you complete the steps, the drive with the Linux file system will unmount and detach from Windows 11.
 
Type the following command to unmount and detach the drive and press Enter:
 
wsl --unmount DISKPATH
 
In the command, make sure to replace DISKPATH for the Device ID of the drive you want to unmount.




