---
title: "Unlocking The Secret To Superfast File Transfers: Master The Rsync Command In Linux Now!"
ShowToc: true 
date: "2023-06-26"
author: "Freddie Strickland"
---
*****
Title: Unlocking The Secret To Superfast File Transfers: Master The Rsync Command In Linux Now!

Introduction:
Are you tired of slow file transfers in Linux? Do you want a solution that can transfer large files and directories quickly and efficiently? If so, then Rsync is the answer you've been looking for. Rsync is a powerful command-line tool that can transfer files between local and remote locations with lightning-fast speed. In this article, we will show you how to use Rsync to achieve superfast file transfers in Linux.

Body:
1. What is Rsync?
Rsync is a command-line utility that is used to copy and synchronize files and directories between local and remote locations. Rsync uses a delta-transfer algorithm, which means that only the differences between the source and destination files are transferred. This makes Rsync much faster than traditional file transfer methods.

2. How to Install Rsync?
Rsync is usually pre-installed in most Linux distributions. If it's not, you can install it using the package manager of your Linux distribution. For example, in Ubuntu, you can install Rsync using the following command:
sudo apt-get install rsync

3. How to use Rsync?
Using Rsync is easy. The basic syntax of Rsync is as follows:
rsync [options] source destination

Here, source is the location of the files or directories you want to transfer, and destination is the location where you want to transfer the files. Options are used to specify additional settings.

4. Rsync Options
The following are some of the commonly used options of Rsync:

-a: This option is used to preserve the permissions, ownership, timestamp, and other attributes of the files being transferred.

-v: This option is used to enable verbose output, which displays detailed information about the transfer.

-z: This option is used to compress the data being transferred, which makes the transfer faster.

-h: This option is used to display the output in a human-readable format.

-P: This option is used to enable partial transfers, which means that if the transfer is interrupted, it can be resumed from where it left off.

5. Examples
Here are some examples of how to use Rsync:

Transfer a single file from a local location to a remote location:
rsync -avz /path/to/local/file.txt user@remote:/path/to/remote/folder/

Transfer a directory from a local location to a remote location:
rsync -avz /path/to/local/folder/ user@remote:/path/to/remote/folder/

Exclude specific files or directories from the transfer:
rsync -avz --exclude="*.txt" /path/to/local/folder/ user@remote:/path/to/remote/folder/

6. Conclusion:
Rsync is a powerful tool that can help you achieve superfast file transfers in Linux. By using the delta-transfer algorithm, Rsync can transfer only the differences between files, making the transfers much faster than traditional file transfer methods. With the options available in Rsync, you can customize the transfers to suit your needs. So, start using Rsync today and enjoy lightning-fast file transfers in Linux.

{{< youtube qE77MbDnljA >}} 



As its name suggests, rsync is a synchronization tool. The first time you use it, it simply copies files and directories from one location to another. Subsequent uses, however, synchronize only the differences between these locations. So, if you add one file to the source directory, rsync will copy only the new file to the destination. This saves a lot of time and bandwidth, especially when copying to a remote location.
 
Imagine you have 50GB of data you have to synchronize to a remote server. You can schedule rsync to run daily. Instead of having to copy the whole 50GB over and over again, the utility will only send the differences. This might mean it only has to upload a few megabytes of data every day, instead of gigabytes.
 
In the featured picture above, you can see how the first time 104MB were transferred, while during the second use only 31KB were required.
 
## How to Install rsync on Various Linux Distributions
 
On Debian and Debian-based distributions, like Ubuntu, you can install rsync with:
 

 
On Fedora, install with:
 
And on distributions derived from RedHat (e.g., CentOS):
 
To install rsync on Arch Linux, use the command:
 
On openSUSE, use:
 
If it isn’t included in your default repositories, consult the openSUSE rsync installation page.
 
## How to Use rsync to Synchronize Local Files or Directories
 
The general syntax of rsync is: rsync [options] /path/to/source /path/to/destination.
 
[options] stands for command line options which you can find in the manual:
 
Press q to quit the manual.
 
To copy a file:
 
The command above is equivalent to rsync /bin/ls /home/your_username. This copies the “ls” command to the directory you are currently in. By default, this should be /home/your_username. The dot . stands for current directory. Pathnames can be absolute (/home/your_username/Downloads/chrome.zip) or relative to your current directory (Downloads/chrome.zip).
 
When you deal with very large files, you can use this command:
 
This will show progress and allow you to resume an interrupted transfer. In case you need to resume, use:
 
Without --append, the transfer would start from scratch.
 
To synchronize directories:
 
Example command:
 
## Effect of Trailing Slash in rsync (Important)
 
In the previous command note that the path to the source directory doesn’t contain a trailing slash / (/bin vs /bin/). Without a trailing slash, rsync copies the directory itself. So rsync -av /bin . results in what is depicted in the following image.
 
When a trailing slash is used, rsync copies the contents in that directory. In this case every file in /bin would be scattered around in the destination directory. So rsync -av /bin/ . would result in what is depicted in the following image.
 
It’s very important to remember this difference, as using TAB to autocomplete directory names automatically adds a trailing slash at the end. So keep that in mind to avoid creating a mess in the destination directory.
 
## How to Use rsync to Synchronize with Remote Locations (e.g. Servers)
 
What was described in the previous section holds true when working with remote locations. The only difference is that you have to prepend the login username and address of the remote location. To send your /bin directory to a remote computer, use:
 
rsync connects through OpenSSH. This means you have to set up the OpenSSH server and login credentials on the remote destination beforehand. Note that your_username refers to the username created on the server. This might be different from the username you have on your local machine.
 
If you own a domain name and point it to your server IP, you can use the domain in the command:
 
On large transfers, it’s useful to also compress data before sending it through the wire by adding the -z parameter:
 
You can omit the compression parameter when you send files that are already compressed (audio files like MP3, videos, JPEG images). They cannot be compressed further, so you would actually waste time by using -z on these.
 
To copy files from the remote destination to your local computer, just reverse locations:
 
## Conclusion
 
This covers the most important rsync commands you need to know. If you ever need more control over how to synchronize directories, consult the online rsync manual and scroll a few pages down until you find “Options Summary.”
 
Fell in love with computers when he was four years old. 27 years later, the passion is still burning, fueling constant learning. Spends most of his time in terminal windows and SSH sessions, managing Linux desktops and servers.
 
Our latest tutorials delivered straight to your inbox




