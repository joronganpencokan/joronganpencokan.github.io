---
title: "Unlock the Secret: Learn How to Move, Delete, and Rename Locked Files with These Genius Tricks!"
ShowToc: true 
date: "2023-02-06"
author: "Conrad Roades"
---
*****
Title: Unlock the Secret: Learn How to Move, Delete, and Rename Locked Files with These Genius Tricks!

Introduction:

Have you ever encountered an annoying message on your computer saying, "Cannot delete file: Access is denied" or "File in use by another program?" If yes, then you've faced the frustrating issue of locked files. Locked files are a common problem among Windows users, and when you try to modify them, you run into errors.

Fortunately, there are several ways to handle locked files, and you don't have to be a tech guru to do so. In this article, we'll show you some genius tricks to move, delete, and rename locked files quickly and easily.

Method #1: Use Task Manager to End the Process

The first trick is to use Task Manager to end the process that's using the locked file. Here's how:

Step 1: Press Ctrl+Shift+Esc to open Task Manager.

Step 2: Find the program that's using the locked file and click on it.

Step 3: Click on "End Task" to close the program.

Step 4: Try to delete, move or rename the file.

Method #2: Use Command Prompt to Force Delete

The second trick is to use Command Prompt to force delete the file. Here's how:

Step 1: Press the Windows key + R to open the Run dialog box.

Step 2: Type "cmd" and hit Enter to open Command Prompt.

Step 3: Type "del /f filename" (replace "filename" with the name of the locked file) and hit Enter.

Step 4: Try to delete, move, or rename the file.

Method #3: Use Unlocker

Unlocker is a free tool that helps you to unlock and delete locked files, folders, and other objects. Here's how to use it:

Step 1: Download and install Unlocker from the official website.

Step 2: Right-click on the locked file and click "Unlocker."

Step 3: Click "Unlock All" and then "OK."

Step 4: Try to delete, move, or rename the file.

Method #4: Use Safe Mode

If the above methods fail, you can try to access the file in Safe Mode. Safe Mode is a Windows mode that starts with a minimal set of drivers and services. Here's how to boot into Safe Mode:

Step 1: Restart your computer.

Step 2: Press F8 before Windows logo appears.

Step 3: Select "Safe Mode" from the menu.

Step 4: Try to delete, move, or rename the file in Safe Mode.

Conclusion:

Locked files can be a frustrating problem, but with these genius tricks, you can easily move, delete, and rename them. Whether you use Task Manager, Command Prompt, Unlocker, or Safe Mode, you can finally get rid of that file that's been bugging you for so long.

{{< youtube 2jYbGwPoFTg >}} 




This article explains how to move, delete, and rename locked files. It also covers how to tell if a file is locked, and how to back it up. All operating systems use locked files.

 
### 
What to Know
 
- Identify which program or process has the locked file open and close it. There are several free programs to move, rename, or delete a locked file when you're unsure what's locking it. To lock a file over a network, open Computer Management > Shared Folders > right-click file > Close.

 
##   How to Unlock a Locked File  
 

Moving, renaming, or deleting a locked file can sometimes be difficult if you're not sure what program or process has it open...which you'll need to close.

 

Sometimes it's very easy to tell what program has the file locked because the operating system will tell you in the error message, like in the PowerPoint example shown in the image above. Often times, however, that doesn't happen, complicating the process.

 

For example, with some locked files, you'll be met with a prompt that says something very general like "the folder or a file in it is open in another program." In this case, you can't be sure which program it is. It may even be from a process running in the background that you can't even see is open!

 

Fortunately, there are a number of free programs that clever software makers have created that you can use to move, rename, or delete a locked file when you're unsure of what's locking it. Our favorite is LockHunter. With it, you can just right-click a locked file or folder to clearly see what's holding it, and then easily unlock the file by shutting down the program that's using it.

 

Files can also be locked over a network; if one user has that file open, it can prevent another user on a different computer from opening the file in a way that lets him or her make changes.

 

When this happens, the Shared Folders tool in Computer Management comes in really handy. Just tap-and-hold or right-click on the open file or folder and choose Close Open File.

 

If you're dealing with a specific error like the "virtual machine" error from above, you might need to investigate what's going on. In that case, it's usually a VMware Workstation problem where LCK files are not letting you take ownership of the VM. You can just delete the LCK files associated with the virtual machine in question.

 

Once a file is unlocked, it can be edited or moved like any other file.

 
##   How to Back Up Locked Files  
 

Locked files can also be a problem for automatic backup tools. When a file is in use, it often can't be accessed to the degree that a backup program needs to ensure that it gets backed up. Enter Volume Shadow Copy Service, or VSS.

 

Volume Shadow Copy Service is a feature that was first introduced in Windows XP and Windows Server 2003 that enables snapshots to be taken of files or volumes even while they're being used.

 

VSS enables other programs and services like System Restore (in Windows Vista and newer), backup tools (like COMODO Backup), and online backup software (like Carbonite) to access the clone of the file without touching the original, locked file.

 

Using Volume Shadow Copy with a backup tool is a huge plus because you'll never have to worry about closing all of your open programs just so the files they're using can be backed up. With this enabled and in use, you can use your computer like you normally would, with VSS working in the background and out of sight.

 

You should know that not all backup programs or services support Volume Shadow Copy, and even for the few that do, you often have to explicitly enable the feature.

 
##   How to Tell if a File Is Locked  
 

A computer file that can be used by only a single program or process at one time is considered a locked file. In other words, the file in question is "locked away" from being used by any other program on the computer it's on or even over a network.

 

In most cases, the purpose of locking a file is to make sure it can't be edited, moved, or deleted while it's being used, either by you or some computer process.

 

You won't normally go hunting around for files that are locked—it's not a file attribute or some sort of thing you can pull up a list for. The easiest way to tell if a file is locked is when the operating system tells you so after you've tried to modify it or move it from where it's at.

 

For example, if you open a DOCX file for editing in Microsoft Word, that file will be locked by that program. If you try to delete, rename, or move it while the program is using it, you'll be told that you can't because the file is locked.

 

Other programs will actually generate a locked file with a particular file extension like .LCK, which is used by programs from Autodesk, VMware, Corel, Microsoft, and likely others. Others might use the .LOCK file extension or something similar.

 

Locked file messages vary a lot, especially from operating system to operating system, but most of the time you'll see something like this:

 
- The source or destination file may be in use.The action can't be completed because the file is open in another program.You must close the file before proceeding.The process cannot access the file because another process has locked a portion of the file.This virtual machine appears to be in use.

 

It's similar to folders, which often show a Folder in Use prompt, followed by a Close the folder or file and try again message.

 

Get the Latest Tech News Delivered Every Day




