---
title: "Revolutionize Your Server Game: Learn How to Effortlessly Migrate from CentOS to AlmaLinux!"
ShowToc: true 
date: "2023-05-18"
author: "Elfrieda Hudman"
---
*****
# Revolutionize Your Server Game: Learn How to Effortlessly Migrate from CentOS to AlmaLinux!

Are you a CentOS user who recently received the news that CentOS will be EOL (End of Life) by the end of the year? Are you now left with the daunting task of moving your infrastructure to a new, reliable distribution? Fear not, as we have a solution for you: AlmaLinux! 

AlmaLinux is a 1:1 binary-compatible fork of Red Hat Enterprise Linux (RHEL) which means that, like CentOS, it follows the same update frequency as RHEL but with no usage limitations, providing a free and stable operating system. AlmaLinux was created by the CloudLinux team as a direct response to the CentOS EOL situation, and their goal is to be a long-term, stable and reliable alternative. 

Migrating your servers from CentOS to AlmaLinux should be a straightforward process, as they are almost identical. Let's go over some simple steps to make the transition as easy as possible.

## Step 1: Backup Your Data

Although the migration from CentOS to AlmaLinux is expected to be seamless, it never hurts to be cautious. Backup all your data from your CentOS servers to ensure nothing is lost during the migration process. This will also help to speed-up and recover from any potential setbacks. 

## Step 2: Install AlmaLinux

The next step is to download and install AlmaLinux. AlmaLinux installation ISO files can be found on their official website. You can easily install AlmaLinux on servers using the standard installation method. 

## Step 3: Copy Your Data

After the installation of AlmaLinux, copy your previously backed up data to your new server. This will ensure that all your data, including vital configuration files, are also migrated from CentOS to AlmaLinux. 

## Step 4: Verify Your Installation

Once AlmaLinux is installed and your data copied over, it is time to verify your new system. Reconfigure your security settings, services and applications to confirm they are operational, and test to ensure everything is working as expected. 

## Step 5: Enjoy the Benefits!

Congratulations! You’ve successfully migrated from CentOS to AlmaLinux. You now have an efficient and reliable operating system that's built for enterprise-level infrastructure. With AlmaLinux, you will continuously receive updates and fixes just as if you were on RHEL. Plus, with no usage limitations, you are free to use and run as many instances as you desire.

### Conclusion

Migrating from CentOS to AlmaLinux is a critical decision for many IT professionals and organizations. AlmaLinux makes this transition an easy and pain-free process. With this guide, we hope you can now effortlessly migrate your infrastructure to AlmaLinux and reap its many benefits!

{{< youtube MgyIzAkz1Ts >}} 



CentOS 8 reached its end of life on December 31, 2021, and there will be no further updates or security fixes released for the operating system. If you are running a CentOS 8 server, it’s time to start thinking about migrating to a new operating system.
 
In this tutorial, you will learn how to migrate from CentOS 8 to AlmaLinux.
 
## What Is AlmaLinux OS?
 
AlmaLinux OS is a reliable, user-friendly, and powerful operating system based on Red Hat Enterprise Linux (RHEL). AlmaLinux is sponsored by CloudLinux and released under the GNU General Public License. AlmaLinux is very similar to CentOS and is the best option if you are looking to move away from CentOS.
 
## Why Use AlmaLinux?
 
There are many reasons to use AlmaLinux. Some of the benefits include:
 
- A fork of RHEL, so it is compatible with all RHEL software and applications.

 
- Backed by a large and active community.

 
- Provides regular updates and security fixes.

 
- Includes all the features you need in a server operating system.

 
## Prerequisites
 
Before you begin this guide, you should have the following:
 
- CentOS server. You should also be logged in as a user with sudo privileges. CentOS 8  is used as an example, but the steps should be similar for other versions of CentOS.

 
- 10GB of free disk space, as the migration process will require space to download the new AlmaLinux files from the Internet and install them.

 
- Sufficient RAM for the migration process (4GB or more is recommended).

 
## Updating Your CentOS Server
 
Before you can migrate from CentOS to AlmaLinux, you need to make sure that your CentOS server is up to date. You will want to make sure that all of the latest security patches and software updates have been installed to ensure a smooth transition to AlmaLinux.
 
You can update your server by running the following command:
 
After the updates have been installed, you will need to reboot your server to ensure that they have been applied properly.
 
Reboot your server by running the following command:
 
## Checking Your Server’s Hardware Compatibility
 
Before you can install AlmaLinux, you need to make sure that your server’s hardware is compatible. AlmaLinux requires a 64-bit processor and at least 4 GB of RAM.
 
Check your server’s processor type by running the following command.
 
If the command returns “x86_64” as shown, your server’s processor is compatible with AlmaLinux.
 
You can check your server’s RAM by running the following command, which will return information about your server’s memory usage. Make sure that the “free” value is greater than 4000MB.
 
Finally, check the release version of your CentOS server.
 
If the command returns “CentOS” and “8,” as shown in the below output, then your server is running CentOS 8 and is compatible with AlmaLinux.
 
## Downloading the AlmaLinux Deployment Script
 
At this point, you should have a server that is running CentOS 8 and up to date. The next step is to download the AlmaLinux deployment script. There are two ways to migrate from CentOS to AlmaLinux.
 
You can manually migrate your server, but it requires much more time and effort. You will need to remove all of the existing CentOS packages, keys, and branding, then install AlmaLinux. This can be a difficult process, so it’s recommended that you only use this method if you are an experienced Linux user.
 
Alternatively, you can use the AlmaLinux deployment bash script that automates most of the migration process. This tutorial will show you how to use the AlmaLinux deployment script.
 
Download the AlmaLinux deployment script by running the following command. This tutorial uses curl to transfer and downloads the AlmaLinux deployment script to your server.
 
The -O option tells curl to save the file with the same name that it has on the server.
 
After the AlmaLinux deployment script has been downloaded, run the ls command to verify that the file exists on your server.
 
You will see output similar to the following:
 
Finally, open the AlmaLinux deployment script in a text editor to review the contents. You should always review the contents of a script that is downloaded from the Internet before you run it on your server. Close the file when you are satisfied.
 
## Migrating From CentOS to AlmaLinux
 
Before you run the script, you must make it executable. By default, the AlmaLinux deployment script is not executable – it’s just a text file.
 
Make the AlmaLinux deployment script executable by running the following command:
 
Type the following command to run the AlmaLinux deployment script:
 
The ./ portion of the command tells Linux to look in the current directory for the “almalinux-deploy.sh” script.
 
The AlmaLinux deployment script will start running and the necessary files for the migration. This process can take some time depending on your server’s Internet connection and specs.
 
Once the AlmaLinux deployment script downloads the files, it will start migrating and reinstalling your server as shown.
 
The script cleans up the old RPM database and replaces it with a new one that is compatible with AlmaLinux. 
 
Once the process completes, you will see the following message. As you can see, using the AlmaLinux deployment script is a breeze, and it only takes a few minutes to migrate your server from CentOS to AlmaLinux.
 
## Verifying the Migration
 
With all the hard work done, the final step is to verify the migration by checking the version of AlmaLinux that is running on your server.
 
To check the version of AlmaLinux, type the following command:
 
You will see output similar to the following. At the time of writing, AlmaLinux 8.6 is the latest version, so the server is running AlmaLinux and up to date.
 
Access the GUI (graphical user interface). This time, you will see the AlmaLinux welcome screen, which completes the migration from CentOS to AlmaLinux. Enter your login information and start using AlmaLinux.
 
You have successfully migrated your server from CentOS to AlmaLinux using the AlmaLinux deployment script. Having done so, you may want to use these tools to secure your Linux server or make use of SELinux that comes with AlmaLinux.
 
## Frequently Asked Questions
 
Image credit: Laptop computer displaying logo of CentOS by 123RF. All screenshots by Nicholas Xuan Nguyen.
 
### Is AlmaLinux Safe?
 
Yes, AlmaLinux is a safe and secure operating system. It is based on CentOS, which is a rock-solid stable platform. AlmaLinux has undergone multiple security audits and is trusted by some of the largest companies in the world.
 
### Is AlmaLinux Free?
 
Yes, AlmaLinux is free to use. You can take a look at the AlmaLinux page for more information.
 
### Is AlmaLinux the same as CentOS?
 
Yes and no. AlmaLinux is based on CentOS and shares many similarities with CentOS. AlmaLinux has its own dedicated team of developers and is not affiliated with Red Hat. However, it’s compatible with all Red Hat Enterprise Linux (RHEL) software.
 
I am a big fan of Linux and open source software. I have been using Linux for over a decade and I absolutely love it. I am also a big fan of writing. In my spare time, I enjoy reading, playing video games.
 
Our latest tutorials delivered straight to your inbox




