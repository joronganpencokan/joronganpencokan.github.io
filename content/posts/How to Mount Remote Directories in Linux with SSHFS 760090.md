---
title: "Easiest Way to Access Remote Files in Linux Revealed- Learn How to Mount Remote Directories with SSHFS Now!"
ShowToc: true 
date: "2023-03-04"
author: "Brad Fortenberry"
---
*****
Easiest Way to Access Remote Files in Linux Revealed- Learn How to Mount Remote Directories with SSHFS Now!

Linux is a powerful operating system used by many individuals and organizations worldwide. However, sometimes Linux users may need to access remote files on a different server without having to manually transfer them every time. If you are one of such users, then you may want to learn how to mount remote directories with SSHFS.

SSHFS is an acronym for Secure Shell File System, which enables you to access remote files on a different server or computer using the SSH protocol. Essentially, you can use SSHFS to access remote directories as if they were local files, which can save you a great deal of time and energy.

In this article, we will take a closer look at how to mount remote directories with SSHFS on Linux. The process is quite simple, and all you need is an active SSH connection to the remote server and a directory that you would like to mount.

Step-by-Step Guide to Mounting Remote Directories with SSHFS on Linux

Step 1: Install SSHFS

The first step is to ensure that SSHFS is installed on your Linux system. In most cases, SSHFS should already be installed, but if not, you can install it using the following command:

sudo apt-get install sshfs

Step 2: Create a Mount Point

Next, you need to create a directory where you will mount the remote directory. You can create a directory anywhere on your local machine, but for simplicity, we will create it in the home directory.

mkdir ~/remote

Step 3: Mount the Remote Directory

You are now ready to mount the remote directory. To do this, use the following command:

sshfs username@remote:/remote/directory ~/remote

In the command above, replace “username” with your remote server username and “remote” with the IP address or hostname of the remote server. Also, replace “/remote/directory” with the path to the remote directory you wish to mount.

Once you have provided all the necessary details, hit enter, and your remote directory will be mounted in the “remote” directory you created earlier.

Step 4: Unmount the Remote Directory

Once you have finished working with the remote directory, you can unmount it using the following command:

fusermount -u ~/remote

In Conclusion

In conclusion, SSHFS is an incredibly useful tool for Linux users who need to access remote files on a different server. The process of mounting remote directories with SSHFS is easy, and with the step-by-step guide provided above, you can quickly start using it in your Linux system.

By mounting remote directories with SSHFS, you can save valuable time and energy that would otherwise be spent on manual file transfers. With this knowledge, you can take your Linux experience to the next level and simplify your workflow with minimal effort.

{{< youtube bEKfUbOyo1A >}} 



There’s certainly no shortage of solutions when it comes to syncing files between two devices. While Google Drive and Microsoft OneDrive may not give you official Linux clients, NextCloud and others do. But maybe you don’t trust a big corporation to store your files. Or, maybe, you want more security than NextCloud offers. With all the components that go into building something like NextCloud, chances are it has more undiscovered security holes than simpler solutions.
 
## Why Use SSHFS?
 
From the end-user perspective, this is very easy to use, clean and simple. It’s also incredibly secure since it relies on the battle-hardened and proven OpenSSH server. Encryption is also top notch, so you can rest assured that no one can steal your files while they are in transit. A correctly configured up-to-date server that only listens for SSH connections is usually impossible to crack for all but the most skilled attackers (think NSA, security specialists, etc.). And they probably don’t want your files.
 
## Why You Wouldn’t Want to Use SSHFS
 
If you want the best possible transfer speed, you might want to use other solutions such as NFS. SSHFS is not the slowest if your Internet connection is of high quality, but it’s not the fastest either. And if you want to transfer directories that contain hundreds of small files, it becomes horrible. Also, if you want to fine-tune file sharing settings, based on individual users or other factors, you might want to use other software.
 
To summarize, if all you need is an easy, secure way to synchronize a remote directory with a local one and aren’t in a huge hurry, you will probably be satisfied with this solution.
 
## Install SSHFS
 
On Arch Linux based installations, use this command:
 
If you’re on a Fedora-based distro, use:
 
On Debian, Ubuntu and family, use:
 
For those of you that use OpenSUSE, enter this command:
 
## Server Configuration
 
If you rent a server or VPS, the OpenSSH server daemon is already configured. Follow the steps recommended by your cloud service provider to configure a regular user (non-root). Some let you do this directly from their web control panel and even let you import the public key to allow SSH access. In this case, generate the key pairs locally, with the ssh-keygen command. After, import the public key from “/home/your_username/.ssh/id_rsa.pub.”
 
If the cloud provider doesn’t offer a tool to easily import SSH public keys, do it manually. At the very least, disallow root login and disable password logins. Use SSH keys exclusively instead: they are impossible to brute-force, as is the case with passwords.
 
If you want to sync files between two computers at home, just treat one as the server (install openssh-server package and configure) and the other one as the client. The same steps apply.
 
## Mount a Remote Directory Locally with SSHFS
 
First, create a directory that will be synced with the remote side.
 
Next, mount the remote directory locally through SSHFS. Replace “user” with the actual username created on your server and “203.0.113.1” with the actual IP address of your remote instance.
 
Of course, if you don’t want to sync the entire home directory of the user on the server side, just replace “/home/user” with “/home/user/some_other_directory” after you create it on the server.
 
When you want to unmount, use this command:
 
## Conclusion
 
If you want a directory to permanently sync to the remote side, add a command like sshfs user@203.0.113.1:/home/user $HOME/sshfs in your autostart manager. Each graphical manager has a different autostart configuration manager, so consult your desktop environment help manual(s). Some sources recommend adding an entry to “/etc/fstab,” but we advise you to avoid that, as failure to mount the directory may result in your system failing to boot entirely.
 
Hopefully this covers all your needs. But, if it doesn’t, you can read about more command line options in the online SSHFS manual.
 
Fell in love with computers when he was four years old. 27 years later, the passion is still burning, fueling constant learning. Spends most of his time in terminal windows and SSH sessions, managing Linux desktops and servers.
 
Our latest tutorials delivered straight to your inbox




