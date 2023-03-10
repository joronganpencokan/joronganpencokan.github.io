---
title: "Unleash the Power of Remote Access: Learn How to Install and Master TeamViewer on Linux Now!"
ShowToc: true 
date: "2023-05-25"
author: "Emery Mclean"
---
*****
# Unleash the Power of Remote Access: Learn How to Install and Master TeamViewer on Linux Now!

Gone are the days when access to a PC or a server was restricted to a physical location. Today, remote access tools have come to the rescue of professionals who need to access their work data or systems from any location. TeamViewer is one such tool that connects different devices over the Internet and allows users to access and control them remotely. The good news is, TeamViewer is not just for Windows and Mac OS, it can also be installed on a variety of Linux distributions such as Ubuntu, Fedora, SUSE, and more.

In this article, we will discuss how to install and set up TeamViewer on a Linux system, as well as how to master its features to make the most out of remote access.

## Installing TeamViewer on Linux

Before we begin with the installation, let's make sure the Linux system meets the minimum requirements to run TeamViewer. The system should have a minimum of 1 GB of RAM, an unrestricted internet connection, and a working graphics card for the best experience. Once the system has met these requirements, we can proceed with the installation. Follow these steps:

1. Open the official TeamViewer website, and select the "Download for Linux" option.
2. Choose the package that is compatible with your Linux distribution.
3. Download the package and save it to your local directory.
4. Once the download completes, launch the terminal and navigate to the directory where the package is saved.
5. Execute the command to unpack and install the package: 

 ```bash
sudo dpkg -i teamviewer.deb
```
   Replace `teamviewer.deb` with the appropriate package name for your distribution.

6. During the installation process, TeamViewer may also prompt you to install additional dependencies. Follow the instructions to install them.

Once the installation is complete, you can launch TeamViewer from the application menu, or the terminal by typing teamviewer.

## Setting up TeamViewer on Linux

After launching TeamViewer for the first time, you will need to set it up by creating an account. Follow these steps:

1. Select the "Create account" option, and enter the required details such as your name, email address, and password.
2. Once the account is created, you will be prompted to login to your account.
3. After logging in, you can set up your computer to be remotely accessible by assigning an alias (name) to it.

You are now ready to use TeamViewer on your Linux system.

## Mastering TeamViewer on Linux

TeamViewer offers a wide range of features that allow users to access and control remote systems effortlessly. Here are some tips to help you master these features:

1. Use unattended access: By setting up unattended access, you can control a remote computer even if there is no one physically present at that location. To set up unattended access, assign an alias (name) to the remote computer, and assign a personal password to the connection.

2. Remote printing: TeamViewer allows users to print documents remotely. To do this, select the "Remote printing" option from the menu bar, and enable "Automatically start remote printing when connecting to this computer".

3. File transfer: TeamViewer makes it easy to transfer files between remote devices. To do this, select the "File transfer" option from the menu bar, choose the file you want to transfer, and drag and drop it to the desired location.

4. Collaboration tools: TeamViewer offers several collaboration tools such as video and voice calls, chat, whiteboard, and more. To access these tools, select the "Meeting" option from the menu bar.

In conclusion, TeamViewer is a powerful tool that makes remote access a breeze, and it offers a variety of features that can help improve productivity. By following the steps outlined in this article, we hope you can unleash the power of remote access on your Linux system.

{{< youtube 3_h9lpqpZSk >}} 



Teamviewer is a powerful tool that allows teams to collaborate and share their screens in real time. It’s also incredibly useful for remote tech support to gain immediate access to a computer remotely with a complete graphical desktop.
 
As a result, it’s not hard to see why Teamviewer supports Linux and packages for both Debian and Redhat distributions. Don’t worry if you’re on a different distribution, they do offer a generic tarball, and some, like Arch, do have packages available.
 
## Install Teamviewer
 

 
Before you start, you’re going to need to download Teamviewer for your Linux distribution. If you’re on Debian, Ubuntu, any of their derivatives or a Redhat distribution, like Fedora or CentOS, swing by the Teamviewer Linux download page. Download either the 64bit DEB or RPM for your distribution. You can try using your distribution’s graphical method to install it, but this guide is going to cover the command line.
 
### Ubuntu/Debian
 
Open your terminal and change into the directory where your Teamviewer package downloaded.
 
Then, use dpkg to install the package. You can use the first command to locate it.
 
Dpkg will probably fail. That’s not a big deal, as you can use Apt to clean up the mess and finish the installation.
 
That will fetch the missing dependencies and configure Teamviewer.
 
### Fedora
 
The process for Fedora is much like the one for Debian distributions. You’re going to use RPM to install the package that you downloaded. First, though, you’ll need to grab the dependencies for Teamviewer.
 
Now, change the directory to where your package is downloaded, and install it with RPM.
 
After the installation has completed, you’re going to need to start the Teamviewer service.
 
To run the Teamviewer service automatically when you start your computer, run the following as well.
 
When you first open Teamviewer, you may see a warning saying that Teamviewer won’t work with Wayland. You’ll need to log out and select GNOME with Xorg to use Teamviewer.
 
### Arch Linux
 
Teamviewer doesn’t officially support Arch, but that didn’t stop the community from adding a package to the AUR. If you don’t have an AUR helper, follow the process below to download and install Teamviewer.
 
If you do have an AUR helper, the process is obviously simpler.
 
Before you can open and use Teamviewer, you’ll need to start the accompanying service.
 
If you want it to run at startup, enable it as well.
 
## Running Teamviewer
 
Teamviewer is a graphical application that you can find classified under the “Internet” section on most desktop environments. After you find it listed alphabetically under “Teamviewer” on GNOME, open it.
 
Before Teamviewer starts, it’ll present you with its EULA. Accept to continue.
 
In the center of your Teamviewer window, you’ll find your current ID and password. These are specific to your computer, and they aren’t tied to any particular account. You can create or sign in to a Teamviewer account, if you like, but it’s not necessary to access another computer.
 
### Connecting
 
It’s extremely simple to connect to another computer with Teamviewer. Ask for the Teamviewer ID of the computer you want to access. Enter it in the “Partner ID” field at the top of your Teamviewer window or in the right third of the “Remote Control” tab.
 
Teamviewer will then ask for the password of the computer that you want to control. Enter that, too. Teamviewer will open a new window with your partner computer’s desktop visible. This window is your portal to the other machine. You can access everything on that computer through this window, just like if you were sitting at it.
 
Take a look at the controls near the top of the window. You can send files, communicate, and change the way you display the connection through this menu. To end the connection, click on the “Actions” section, and select the option to close the connection.
 
That’s all for the basics. You can now remotely access another computer via Teamviewer and help troubleshoot or simply access files. It’s a versatile way for teams to work together, and it provides a convenient way to access a remote machine.
 
Nick is a freelance tech. journalist, Linux enthusiast, and a long time PC gamer.
 
Our latest tutorials delivered straight to your inbox




