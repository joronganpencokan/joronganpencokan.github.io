---
title: "Protect Your Server Like a Fort Knox: Learn the 10 Easy Steps to Harden Ubuntu 14.04!"
ShowToc: true 
date: "2023-06-11"
author: "Scott Jeffers"
---
*****
# Protect Your Server Like a Fort Knox: Learn the 10 Easy Steps to Harden Ubuntu 14.04!

If you have an Ubuntu 14.04 server, it is important to keep it secure from possible cyber attacks. You don't want unauthorized users to gain access to your server, and potentially important data that it may hold. To safeguard your server, you need to harden it. This simply means to make it more secure by making it more difficult for those who are unauthorized to access your server. Here, we’ll outline the 10 easy steps you can take to harden Ubuntu 14.04.

## Step 1: Create a User Account for Administrators

First, create a user account for administrators to use when accessing your server. This is a small step that can go a long way in securing your server from potential attackers. It will also help to ensure that only authorized persons can make changes to your server’s configuration.

## Step 2: Patch the Server Regularly

While it may seem like a no-brainer, patching the server regularly cannot be overstated. Ubuntu 14.04 is a relatively old system, but security vulnerabilities can still be found in the system. Keep the system updated to protect it from cyber threats.

## Step 3: Install a Firewall

A firewall is a crucial component of any server security system. It acts as a barrier between the internet and your server, and it can help identify and stop unauthorized access. Ubuntu comes with its own firewall called ‘UFW’ which can be enabled with a few simple commands.

## Step 4: Disable Unused Services

Unused services on your server may still be running even if you don't use them. Hackers could exploit flaws in them to gain access to your system. Disable any unnecessary services on your server to reduce its attack surface.

## Step 5: Install Only Secure Software Packages

Installing only secure software packages can go a long way in securing your Ubuntu 14.04 server. Avoid installing software from unknown sources. Stick with software that is necessary to operate your server, and regularly update those packages to ensure they remain secure.

## Step 6: Use a Strong Password

Passwords that are easy to guess are a hacker's delight. Ensure you use strong passwords that are difficult to crack. Use uppercase and lowercase letters, numbers and special characters. Train employees on password management best practices.

## Step 7: Limit Remote Access to Your Server

Limiting remote access to your server can help protect it from unauthorized access. Configure your server’s access control in such a way that access is limited only to authorized parties.

## Step 8: Activate Disk Encryption

Encrypting your hard disk will safeguard your sensitive data should it get into the wrong hands. Set up Ubuntu's full disk encryption feature to make sure data is encrypted at rest.

## Step 9: Enable SSH Key Authentication

Secure Shell (SSH) key authentication is a more secure way to access your server compared to passwords. Once enabled, authorized users with the matching private key can log in without a password.

## Step 10: Set Up Log Monitoring

It's important to know what is happening on your server. Log monitoring will enable you to detect and respond to any suspicious activity on your server.

# Conclusion

Harden Ubuntu 14.04 with these 10 easy steps to protect against possible cyber attacks. Don't fall prey to the hackers. Implement security best practices to ensure the safety of your server and its information.

{{< youtube ZhMw53Ud2tY >}} 



Hardening is the process of reducing vulnerabilities and securing a system from possible attack points. Reducing vulnerabilities includes the removal of unnecessary services, usernames and logins and disabling unnecessary ports. In this article we are going to show you how you can harden a Ubuntu server.
 
## Requirements
 
Ubuntu 14.04 LTS server with Open SSH installed.
 
## Getting started: Update the system
 
Keeping the system up to date is necessary after installing any operating system. This will reduce known vulnerabilities that are in your system.
 
For Ubuntu 14.04 run the following:
 
## Enable automatic security updates
 
Enabling automatic updates can be very important to secure your server. To install the “unattended-upgrades,”  run
 
To enable it, run the following command:
 
This will create the “/etc/apt/apt.conf.d/20auto-upgrades” file shown below.
 
## Create “shadow user” with sudo powers
 
Using a “shadow user” instead of the root account is necessary for security reasons. You can create a user that will not be easy for other users to guess. In this tutorial we will use “maketech111” as the username.
 
To create a user, run the following command:
 
To give the user sudo access, run the following command:
 
To set a password, run the following command:
 
Note: make sure your password is at least eight characters long and contains a complex combination of numbers, letters, and punctuation marks.
 
To remove the password prompt for sudo, edit the sudoers file.
 
Add / edit as described below.
 
Save the file and exit.
 
## Disable root account
 
Disabling the root account is necessary for security reasons.
 
To disable the root account, use the following command:
 
If you need to re-enable the account, run the following command:
 
## Add a SWAP Partition
 
Some Ubuntu servers are not configured with SWAP. SWAP is used when the amount of total physical memory (RAM) is full.
 
To check for SWAP space, run the following command:
 
If there’s no SWAP file, you should get a the following output.
 
To create the 4 GB SWAP file you will need to use the “dd” command.
 
To set up the SWAP file, run the following command:
 
To activate the swap file, run
 
This will output like the following:
 
To enable it permanently, edit the “/etc/fstab” file.
 
Add the following line:
 
## Improve SWAP performance
 
Set proper swappiness value to improve overall performance of the system.
 
You can do this with the following command:
 
Reboot the system to check whether SWAP gets activated properly.
 
## Disable IPv6
 
It is recommended to disable IPv6 because it cause issues with the Internet connection being slow.
 
To disable IPv6, edit the “/etc/sysctl.conf” file.
 
Edit as described below:
 
To reload the configuration, run
 
## Disable IRQBALANCE
 
IRQBALANCE is used to distribute hardware interrupts across multiple CPU to increase system performance. It is recommended to disable IRQBALANCE to avoid hardware interrupts in your threads.
 
To disable IRQBALANCE, edit “/etc/default/irqbalance”
 
and change the ENABLED value to 0:
 
## Fix OpenSSL heartbleed bug
 
The Heartbleed is a serious vulnerability in the OpenSSL. It allows a remote user to leak the memory in up to 64k chunks. Hackers can then retrieve the private keys to decrypt any data like user’s user name and passwords.
 
The heartbleed bug was found in OpenSSL 1.0.1 and is present in the following versions:
 
- 1.0.1
 - 1.0.1a
 - 1.0.1b
 - 1.0.1c
 - 1.0.1d
 - 1.0.1e
 - 1.0.1f

 
To check the version of OpenSSL in your system, run the following commands:
 
This will output something like the following:
 
If the date is older than “Mon Apr 7 20:33:29 UTC 2014,” and the version is “1.0.1,” then your system is vulnerable to the Heartbleed bug.
 
To fix this bug, update OpenSSL to the latest version and run
 
Now check the version and run
 
## Secure the Console, shared memory, /tmp and /var/tmp
 
### Secure the Console
 
By default, lots of terminals are enabled in your system. You can allow only one terminal and disable the other terminals.
 
To allow only “tty1” and disable other terminals, edit the “/etc/securetty” file.
 
Add / Edit the following lines:
 
To secure the “/etc/securetty” file, change the permission of the file and run the following commands:
 
### Secure Shared Memory
 
Any user can use shared memory to attack against a running service, like apache or httpd. By default, shared memory is mounted read/write with execute permission.
 
To make it more secure, edit the “/etc/fstab” file.
 
To make the changes without rebooting, you can run
 
### Secure /tmp and /var/tmp
 
Temporary directories such as /tmp, /var/tmp, and /dev/shm open the door for attackers to provide space to run scripts and malicious executables.
 
Secure /tmp folder
 
Create a 1GB filesystem file for the /tmp partition.
 
Create a backup of the current /tmp folder:
 
Mount the new /tmp partition, and set the right permissions.
 
Copy the data from the backup folder, and remove the backup folder.
 
Set the /tmp in the fbtab.
 
Test your fstab entry.
 
Secure /var/tmp:
 
Some software uses this folder as a temporary folder, so we should also secure this one.
 
To secure /var/tmp,  create a symbolic link that makes /var/tmp point to /tmp.
 
## Set security limits and disable unwanted services
 
### Set security limits
 
To protect your system from fork bomb attacks, you should set up a process limit for your users.
 
To set this up, edit the “/etc/security/limits.conf” file,
 
and edit the following line:
 
This will prevent users of a specific group from having a maximum of twenty processes and maximize the number of processes to one hundred to user1.
 
### Disable unnecessary services
 
Lots of services in Ubuntu takes memory and disk space that you might need to use. Disabling or removing unnecessary services can improve overall system performance.
 
To find out which services are currently running, run the following command:
 
You can disable it by running this command.
 
## Fix Shellshock Bash vulnerability:
 
The Shellshock vulnerability allows hackers to assign Bash environment variables and gain unauthorized access to the system. This vulnerability is very easy to exploit.
 
To check system vulnerability, run the following command:
 
If you see the below output, it means your system is vulnerable.
 
To fix this vulnerability, run the following command:
 
If you run the command again, you will see:
 
## Conclusion:
 
Here we have explained basic things that you could do to harden Ubuntu. You should now have enough understanding of basic security practices that you can implement on your Ubuntu server. I hope that this post will be useful to you.
 
Reference: Ubuntu Hardening Guide
 
Our latest tutorials delivered straight to your inbox




