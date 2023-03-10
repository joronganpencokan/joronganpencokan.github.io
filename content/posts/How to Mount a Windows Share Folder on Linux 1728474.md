---
title: "Linux Users Won't Believe How Easy It Is To Access Windows Share Folders – Learn the Simple Trick Here!"
ShowToc: true 
date: "2023-05-28"
author: "Merle Taveras"
---
*****
# Linux Users Won't Believe How Easy It Is To Access Windows Share Folders – Learn the Simple Trick Here!

If you're a Linux user, chances are you've come across some difficulties in accessing share folders from Windows machines. In the past, this was a frustrating process that required several steps and a lot of technical know-how. Fortunately, that's no longer the case, and accessing Windows share folders on Linux is easier than ever. So, if you're ready to learn a simple trick to make your life a lot easier, keep reading.

## The Simple Trick

The trick to accessing Windows share folders on Linux is to use the CIFS (Common Internet File System) protocol. This protocol allows Linux to mount Windows share folders as if they were local files. With CIFS, you can access Windows share folders in the same way you would access any other directory on your Linux machine.

Here are the steps you need to follow:

1. Install the CIFS utilities on your Linux machine. The command to do this varies depending on the Linux distribution you're using. For example, on Ubuntu, you would use the following command:

   ```
   sudo apt-get install cifs-utils
   ```

2. Create a directory where you want to mount the Windows share folder. For example, you might create a directory called "windows-share" in your home directory.

   ```
   mkdir ~/windows-share
   ```

3. Mount the Windows share folder using the following command:

   ```
   sudo mount -t cifs //WINDOWS_MACHINE/SHARE_NAME ~/windows-share -o username=WINDOWS_USER,password=WINDOWS_PASSWORD
   ```

   Replace "WINDOWS_MACHINE" with the name or IP address of the Windows machine that has the share folder you want to access. Replace "SHARE_NAME" with the name of the share folder. Replace "WINDOWS_USER" and "WINDOWS_PASSWORD" with the username and password you use to log in to the Windows machine.

That's it! Now you can access the Windows share folder by navigating to the "windows-share" directory you created. You can copy files to and from the share folder just like any other directory on your Linux machine.

## Conclusion

Accessing Windows share folders on Linux used to be a frustrating process, but with the CIFS protocol, it's now easier than ever. By following the simple steps outlined above, you can mount a Windows share folder as a local directory on your Linux machine in just a few minutes. So, if you're a Linux user who needs to access Windows share folders, give this trick a try – you won't believe how easy it is!

{{< youtube A3G-3hp88mo >}} 



Linux and Windows systems have major differences, with different file systems and protocols in use. Sharing files between them can be difficult, especially because they use two different sharing protocols. That doesn’t mean it’s impossible to mount a Windows share folder on Linux, however. Follow along below to find out how.
 
## Share Your Windows Folder
 
Before you do anything, you need to ensure that Windows has been correctly set up to allow for networking file sharing.
 
To enable this on Windows, right-click on the network icon in the notifications area of your Windows taskbar. From here, click “Open Network & Internet Settings.”
 
Under the “Status” category, click “Sharing options.”
 
In your Windows sharing options menu, make sure that “Turn on network discovery” and “Turn on file and printer sharing” are enabled.
 
Click the radio buttons next to both options to make sure this is the case.
 
Click “Save changes” to save your settings. Once this is done, open Windows File Explorer and locate the folder you’re looking to share with your Linux PC.
 
Right-click the folder and click “Properties.”
 
In your folder properties, click the “Sharing” tab, then click “Advanced Sharing.” Click to enable the “Share this folder” checkbox, then click “Permissions.”
 
Under the “Permissions” section, set the control rights for your folder. By default, Windows will grant read-only access to your files.
 
If you want to allow everyone to read or write to the folder, click “Allow” for the “Full Control” permissions set. Set these permissions to suit your own requirements.
 
Once you’re done, click “OK” three times to close each of the dialog boxes.
 
Your folder should now be shared on your network, ready for you to access from your Linux PC.
 
## Install CIFS-utils
 
Depending on your Linux distribution, you may be able to mount your Windows-shared folder automatically in your distribution’s file explorer.
 
However, this may not work correctly. The safest way to mount Windows-shared folders on Linux is to use the CIFS-utils package and mount the folder using the Linux terminal.
 
This allows Linux machines to access SMB file shares used by Windows PCs.
 
To install CIFS-utils, open a new terminal window. For Ubuntu and Debian-based distributions, type:
 
For Arch users, type:
 
Once installed, you can then mount your Windows share folder from the Linux terminal.
 
## Mount Windows SMB Share on Linux
 
You’ll need to create a mount directory before you can mount your Windows SMB-shared folder on Linux. This is where Linux will mirror the contents of your shared folder.
 
To do that, open a terminal window and type:
 
Once created, type the following:
 
Replace “Windows” with the IP address or hostname for your Windows PC and “SharedFolder” with your shared folder name. For the username, replace “account” with your Windows username or full Microsoft account email.
 
You’ll be asked to provide your Windows password before the mounting process is complete. Type this in, then click Enter. If you used the correct information, your Windows folder should now be mounted and accessible in the folder you created.
 
## Sharing Files Between Linux and Windows in Dual Boot
 
Sharing files between Windows and Linux works great when you mount a shared folder between the two devices, but can you still share files with a dual boot setup? Linux and Windows have separate file systems. Linux usually uses Ext4, while Windows uses NTFS and also works with FAT32. This doesn’t mean it’s impossible to see and share files, though. 
 
You’ll need a compatible Windows system, build 20211 or higher, and a few other resources to make it work. Don’t worry. Everything is free. This guide walks you through each step in the process, including a way to read and share files between Windows and Linux.
 
## Frequently Asked Questions
 
### 1. Why do I get a syntax error when trying to mount a folder in Linux?
 
Either there’s a small error in the command in the terminal window, or you have a space in the folder name. Spaces don’t always come across correctly in the syntax. Instead of recognizing the command as the full name of the folder, the system sees two unrelated items.
 
Avoid this by placing the name in quotes. For instance, Shared Folder would become “Shared Folder.” Of course, you can also just rename the Windows 10 folder to place the words together or have a dash between them.
 
### 2. Can I mount a shared folder if I use VirtualBox? 
 
Yes. The process should work the same way. You can also share devices, such as USB drives.
 
### 3. Can I mount guest, network, or password protected folders?
 
Yes, but since you’re not using the main Windows 10 account, you will need to adjust the syntax a bit. Plus, if you’re mounting a network folder, you’ll also need the server or machine name. 
 
While this guide applies to Ubuntu, it should work for most major Linux distros as well. It lists the syntax for different scenarios, assuming you’ve already completed all of the steps (except the final mounting) above.
 
### 4. Why do I only have read access for the shared folder?
 
If you want to store files in the shared folder from Linux, make sure you have full read/write access to the folder in Windows. If the Windows user account only has read permission, this is the only permission you’ll have from Linux as well. You must change your account permissions from within Windows 10. For companies, you’ll need your IT admin to make the change for you.
 
### 5. Why aren’t folder changes showing up?
 
If you’ve made changes to the permissions of the folder, they may not show up immediately in Linux. You’ll need to remount the folder for changes to take effect. 
 
Use the command above to remount any shared folders. This should ensure things work as expected. If you have any random glitches, remounting typically fixes them.
 
## Wrapping Up
 
Mounting Windows and Linux shared folders gives you the freedom to access your most important files, no matter the operating system. The SMB protocol is well supported on Linux, so you shouldn’t find it difficult to continue accessing your Windows files and folders once you’ve installed the CIFS-utils package.
 
If you’d rather use a single system, here are five of the best Linux distros for Windows users you could use.
 
Crystal Crowder has spent over 15 years working in the tech industry, first as an IT technician and then as a writer.  She works to help teach others how to get the most from their devices, systems, and apps. She stays on top of the latest trends and is always finding solutions to common tech problems.
 
Our latest tutorials delivered straight to your inbox




