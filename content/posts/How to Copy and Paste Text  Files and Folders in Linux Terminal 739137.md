---
title: "Unlocking The Secret To Lightning Fast File Transfers In Linux Terminal: Learn How To Copy And Paste Like A Pro!"
ShowToc: true 
date: "2023-03-30"
author: "Autumn Wright"
---
*****
Title: Unlocking The Secret To Lightning Fast File Transfers In Linux Terminal: Learn How To Copy And Paste Like A Pro!

Introduction

File transfers are an essential aspect of everyday computing activities. However, copying files from one location to another in a Linux terminal can be a daunting task, especially for new users. Nonetheless, learning how to copy and paste files using Linux terminal commands can help you transfer data in a lightning-fast manner. In this article, we will explore the secret to unlocking fast file transfers in Linux terminal using simple copy and paste commands.

Copying Files and Directories in Linux Terminal

To copy files and directories in Linux terminal, you can use the cp command followed by the source file or directory and the destination directory. For example, to copy a file named mydoc.txt from the home directory to the documents directory, you can use the following command:

cp ~/mydoc.txt ~/Documents

On the other hand, to copy a directory and its contents, you can use the -r option to recursively copy all the subdirectories and files within the given directory. For example, to copy a directory named myfolder from the home directory to the documents directory, you can use the following command:

cp -r ~/myfolder ~/Documents

Copying Files and Directories Between Remote and Local Systems

Sometimes you may need to copy files and directories between remote and local systems. In this case, you can use the scp (secure copy) command to transfer files using secure shell (ssh) protocol. To copy a file named mydoc.txt from a remote system with the IP address 192.168.1.100 to the local system, you can use the following command:

scp user@192.168.1.100:/path/to/mydoc.txt ~/Documents

In this command, replace the user with the user account on the remote system and /path/to/mydoc.txt with the actual path to the file on the remote system.

Copying Files and Directories Over Network Shares

If you want to copy files and directories over network shares, you can use the smbclient command to access Windows shared drives and copy files. To copy a file named mydoc.txt from a Windows shared drive named share1 to the local directory, you can use the following command:

smbclient //server/share1 -U user%password -c 'get mydoc.txt'

In this command, replace the server with the name or IP address of the Windows system, user with the user account on the Windows system, password with the corresponding password, and mydoc.txt with the actual file name.

Conclusion

Copying and pasting files in Linux terminal can be easy and fast once you learn the basic commands. Whether you want to copy files locally or remotely, between Linux systems or Windows systems, the cp, scp, and smbclient commands can streamline your file transfers efficiently. So, unlock the secret to lightning-fast file transfers in Linux terminal today and learn how to copy and paste like a pro!

{{< youtube -ykeT6kk4bk >}} 



Copying and pasting is one of the most used actions on a computer. While it is easy to do so with the Ctrl + C and Ctrl + V keyboard shortcuts, on the Linux terminal it is not so straightforward. You have several options to get the job done. Here is how you can copy and paste text, files and directories in Linux terminal.
 
## Copy and Paste Text
 
If you just want to copy a piece of text in the terminal, all you need to do is highlight it with your mouse, then press Ctrl + Shift + C to copy.
 
To paste it where the cursor is, use the keyboard shortcut Ctrl + Shift + V.
 
The Paste shortcut also applies when you copy a section of text from a Word document (or any other application) and want to paste it in the terminal. For example, you can copy a command from a web page in your browser and use the Ctrl + Shift + V shortcut to paste it in the terminal.
 
If for some reason these keyboard shortcuts don’t work, the terminal might not be properly configured for it. Look for options that allow you to customize keyboard shortcuts. These are instructions for the most popular terminals:
 
- Gnome Terminal – Click the hamburger menu and click “Preferences.” Navigate to “Shortcuts” and scroll to “Edit.” The options for “Copy” and “Paste” will appear there ready to be configured.Konsole – Go to “Settings” and then click on “Configure Keyboard Shortcuts.” Search for “Copy,” configure it to use the key combos mentioned previously, then do the same for “Paste.”

 
Most other terminals will lock you into the default universal combination for copying/pasting in the console without the ability to configure them.
 
## Copy and Paste a Single File
 
Any time you want to copy a file or folder in the Linux command line, the above keyboard shortcut won’t work. You have to use the cp command. cp is shorthand for copy. The syntax is simple, too. Use cp followed by the file you want to copy and the destination where you want it moved.
 
That, of course, assumes that your file is in the same directory you’re working out of. You can specify both.
 
You also have the option of renaming your file while copying it. Specify the new name in the destination.
 
## Copy and Paste a Folder and Its Contents
 
In order to copy a folder and its contents, you’re going to need to tell the cp command to copy recursively. That’s simple enough with the -r flag.
 
All the rest of your syntax is exactly the same. The -r flag serves to tell cp that it’s working with a directory and should copy its contents.
 
If you want the paste action to overwrite existing files, you can add the -f flag:
 
## Copy and Paste Multiple Files
 
You can also copy multiple files. The Linux command line lets you target multiple items at once with brackets {}. You can use them to list the names of each file to be copied separated by commas.
 
All three files of differing file types will be copied to the Documents directory.
 
## Copy and Paste All Files of the Same Type
 
If you have a ton of files of the same type to copy, you can use the wildcard character *. The asterisk/wildcard tells the Linux command line to accept absolutely anything in that place. So, if you tell Linux to copy *.jpg, it’ll copy all JPG files, regardless of the name or whatever comes before the .jpg part.
 
If you want to use multiple file types, say JPG and PNG, you can use the brackets from before.
 
## Make Copying More Interactive
 
As you may have noticed while following this guide, using cp does not give you any sort of confirmation or prompt after finishing what it’s doing unless it encounters an error. This may cause a bit of discomfort especially when you’re doing very large file copy operations on slower hardware that could take a long time to complete.
 
By attaching the -v flag to your command, you tell cp to give you its most detailed output on what it does. The -i flag provides confirmation prompts so that you have a chance to cancel certain operations like overwriting certain files.
 
Generally the -v and -i flags are available in a large range of commands that are common to Linux.
 
## Rsync vs CP
 
If you need to do several copy operations that overwrite files (such as creating a backup that you will update once in awhile) for some reason, rsync might just put a smile on your face.
 
rsync is a little more advanced in that it goes into the minutiae of each file, does a full comparison of the data in both, and within the file itself, only overwrites the data that has changed. This is especially useful if the destination folder is in an SSD, as it saves write cycles and doesn’t needlessly degrade the drive’s health by overwriting entire files.
 
Learn how to make use of rsync to copy files in Linux.
 
## Move a File or Folder
 
If you came here looking to move a file from one place to another without making a duplicate, you can do that easily too, but moving a file requires the mv command. The syntax is very similar to cp.
 
Similarly, you can also rename the file.
 
There is one major difference, though. You don’t need the -r flag to move a whole folder.
 
## Frequently Asked Questions
 
Image credit: Neron Photos on Pexels
 
### Is rsync better than cp?
 
Neither is better than the other generally. rsync will make full comparisons of files in both the source and destination folders, taking up some computing resources to save on bandwidth or write cycles. It’s great if you’re constantly updating a backup of a particular folder, but less than ideal if you’re just doing a single copy operation.
 
cp functions more as a Swiss Army knife that just wants to get the job done. If you have to overwrite something, cp does it for you. Because of its capability for interactivity, it’s also more beginner-friendly and gives you a bit more control over the copying process.
 
### Why can't I just use Ctrl+C to copy items from my terminal?
 
In Linux terminal applications, pressing Ctrl + C on your keyboard sends a SIGINT (interrupt) signal to the kernel. It’s a simple way of telling Linux to stop whatever is running on that particular terminal.
 
If you configure the “Copy” function in your terminal to respond to that key combination, you will encounter problems when copying a line of text from an executing command while it’s still in the process of doing something.
 
Miguel has been a business growth and technology expert for more than a decade and has written software for even longer. From his little castle in Romania, he presents cold and analytical perspectives to things that affect the tech world.
 
Our latest tutorials delivered straight to your inbox




