---
title: "Unleash the Power of Linux: Install Deepin Desktop on Ubuntu NOW!"
ShowToc: true 
date: "2023-02-17"
author: "Doris Bridges"
---
*****
Linux is undoubtedly one of the most popular operating systems in the world, mainly due to its stability, security, and flexibility. It is an open-source platform that allows users to customize it to meet their needs. One of the most popular Linux distributions is Ubuntu. It is user-friendly, and it has an extensive community that provides support and assistance to users. But what if you want to add some flavor to your Ubuntu system? What if you want a beautiful and powerful desktop environment that is also easy to use? In that case, you need to install the Deepin desktop on Ubuntu.

The Deepin desktop is an open-source desktop environment for Linux distributions, which features a modern and elegant interface. It is designed to provide users with a simple and intuitive interface, while also providing powerful tools and features for productivity and performance. Installing the Deepin desktop on Ubuntu is not difficult, and in this article, we will guide you through the process.

Step 1: Add the Deepin repository

Before installing the Deepin desktop, you need to add the Deepin repository to your Ubuntu system. This repository contains all the necessary packages and dependencies that are needed to install the Deepin desktop.

To add the Deepin repository, you need to open the terminal and enter the following command:

sudo sh -c 'echo "deb http://packages.deepin.com/deepin/ apricot main non-free universe" > /etc/apt/sources.list.d/deepin.list'

Step 2: Import the Deepin GPG key

Once you have added the Deepin repository, you need to import the GPG key that is used to sign the packages in the repository. This key is used to verify the authenticity of the packages, and it is essential for security purposes.

To import the Deepin GPG key, enter the following command in the terminal:

wget http://packages.deepin.com/deepin/project/deepin-keyring.gpg

sudo apt-key add deepin-keyring.gpg

Step 3: Update your Ubuntu system

Before installing any new software, it is always a good idea to update your Ubuntu system. This will ensure that all the packages and dependencies are up to date, and it will also fix any bugs or issues that may be present.

To update your Ubuntu system, enter the following command in the terminal:

sudo apt-get update && sudo apt-get upgrade

Step 4: Install the Deepin desktop

Once you have added the Deepin repository, imported the GPG key, and updated your Ubuntu system, you can now install the Deepin desktop. To do this, enter the following command in the terminal:

sudo apt-get install deepin-desktop-environment

This command will download and install all the necessary packages and dependencies that are needed to install the Deepin desktop on your Ubuntu system.

Step 5: Log out and log in

Once the installation is complete, you need to log out of your current session and log back in. You will notice that the login screen has been replaced by the Deepin login screen. Select the Deepin desktop from the list of available desktop environments, and you are ready to go.

Conclusion

Installing the Deepin desktop on your Ubuntu system is a simple and easy process that can be completed in just a few steps. The Deepin desktop environment is an excellent choice for users who want a beautiful and powerful desktop environment that is easy to use. It features a modern and elegant interface that is designed to provide users with an intuitive and productive experience. So, if you want to unleash the power of Linux, install Deepin desktop on Ubuntu now!

{{< youtube GH-QUi6Jamw >}} 



Linux Deepin is a beautiful Linux Distro based on Ubuntu. While we have reviewed Linux Deepin and has full of praise for it, the latest version 12.12 is even better, more elegant and is running more smoothly. If you have no intention to format your PC and install Linux Deepin from scratch, here is how you can install the Linux Deepin Desktop on Ubuntu and access it from the login screen.
 
In your Ubuntu, open a terminal.
 
The first thing we are going to do is to add the repository for Linux Deepin packages.
 
Add the lines at the end of the file:
 
Press Ctrl + O follow by Ctrl + x to save and exit the sources list. 
 
Next, we are going to fetch and import the public key for Linux Deepin packages.
 
Update the system.
 
Lastly, install the Linux Deepin desktop environment:
 
This will install a big bunch of files to your system and could take a long time, depending on your Internet connection. 
 
Additionally, you can add the Deepin Music Player, Software Center and Settings panel to the mix:
 
Once the installation finished, restart your computer (or log out of your existing session). You should find the new Deepin Desktop Environment available for selection in the login screen. 
 

 
Here are some screenshots:
 
Linux Deepin Desktop:
 
Linux Deepin Software Center:
 
Linux Deepin Music Player:
 
Linux Deepin System Settings
 
Note that this will not give you a complete Linux Deepin experience. Some of the applications (such as Nautilus) will retain their original look and feel. Nevertheless, this is still one of the best way to use Linux Deepin without reformatting your computer.  
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




