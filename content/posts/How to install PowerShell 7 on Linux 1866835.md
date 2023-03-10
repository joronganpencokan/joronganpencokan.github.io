---
title: "Revolutionize Your Linux Game: Easy Guide to Installing Powershell 7!"
ShowToc: true 
date: "2023-06-08"
author: "Don Dunkle"
---
*****
# Revolutionize Your Linux Game: Easy Guide to Installing Powershell 7!

Have you ever wished that you could use PowerShell on Linux, but didn't know how to get started? Well, the good news is that you can now easily install and use PowerShell 7 on your Linux machine! In this article, we'll walk you through the simple steps required to install Powershell 7 on Linux and take your Linux game to the next level.

## What is Powershell 7?

PowerShell is a command-line shell and scripting language, which was originally developed by Microsoft for Windows. With PowerShell, you can automate complex tasks, manage your system configurations and perform data analysis. PowerShell provides access to a large and growing library of modules, which you can use to perform many different tasks from managing Active Directory to managing Azure resources.

PowerShell 7 is the latest version of PowerShell that runs on all major operating systems including Windows, Linux, and macOS. It provides several improvements over earlier versions, including better performance and support for more platforms.

## How to Install Powershell 7 on Linux?

The installation process for PowerShell 7 on Linux is straightforward and easy to follow. Follow these simple steps to get started:

### Step 1: Add Microsoft repository

Open your terminal and type the following command to add the Microsoft repository:

```
wget -q https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
sudo dpkg -i packages-microsoft-prod.deb
```

### Step 2: Install PowerShell 7

Now that you've added the Microsoft repository, you can install PowerShell 7. Run the following command in your terminal:

```
sudo apt-get update
sudo apt-get install -y powershell
```

Once the installation is complete, you can launch PowerShell by typing "pwsh" in the terminal.

### Step 3: Verify the installation

To verify that PowerShell 7 is installed correctly, type the following command in your terminal:

```
pwsh --version
```

You should see the PowerShell 7 version number displayed in the terminal.

## Conclusion

That's it! You have successfully installed PowerShell 7 on your Linux machine. You can now use the automation and configuration management features of PowerShell to manage your Linux environment efficiently. With PowerShell 7, your Linux game will never be the same again! So, what are you waiting for? Go, revolutionize your Linux game now!

{{< youtube ZdhU2-TPj7o >}} 



If you use PowerShell on Windows 10, but you also require to use a Linux distribution (such as Ubuntu) for work, you can now install the Microsoft command-line shell and scripting language in the most popular flavors of the open source operating system.
 
At the time of this writing, you can install PowerShell 7, which is built on .NET Core 3.1, but it’s backward compatible with the modules for older releases.
 
In this guide, you’ll learn the steps to install PowerShell 7 on Ubuntu using graphical user interface (GUI) or command line. (These are the steps to install the tool on Windows 10.)
 
- How to install PowerShell using Ubuntu Software
 - How to install PowerShell using package installer
 - How to install PowerShell using Snap command on Ubuntu
 - How to install PowerShell using using Package Repository on Ubuntu

 
## How to install PowerShell using Ubuntu Software
 
- Open Ubuntu Software app.
 - Search for PowerShell.
 - Select the powershell option.
 - Click the Install button.
 - Install PowerShell Ubuntu Software app

 
Once you complete the steps, you can access the app using the pwsh on the Linux Terminal.
 
Open Ubuntu Software app.
 
Search for PowerShell.
 
Select the powershell option.
 
Click the Install button.
 
Install PowerShell Ubuntu Software app

 
If you want to uninstall it, then on the “Ubuntu Software” app, click the Installed tab, and click the Remove button for PowerShell.
 
## How to install PowerShell using package installer
 
To install PowerShell on Linux using GUI installer, use these steps:
 
- Open PowerShell download page on GitHub.
 - Under the “Assets” section, click the powershell_7.x.x-x.ubuntu.xx.xx_amd64.deb depending on the version of Ubuntu on your device.
 - PowerShell 7 deb package download
 - Quick note: PowerShell is also available for other flavors of Linux, including CentOS, Alpine, Red Hat, and Debian.
 - Save the file on your device.
 - Double-click the *.deb file to launch the installer.
 - PowerShell Ubuntu amd64 deb package
 - Click the Install button.
 - PowerShell GUI installer

 
Once you complete the steps, PowerShell will install, and you can launch it from the Terminal using the pwsh command.
 
Open PowerShell download page on GitHub.
 
Under the “Assets” section, click the powershell_7.x.x-x.ubuntu.xx.xx_amd64.deb depending on the version of Ubuntu on your device.
 
Save the file on your device.
 
Double-click the *.deb file to launch the installer.
 
PowerShell Ubuntu amd64 deb package

 
PowerShell GUI installer

 
If you run into dependencies problems, then use the steps below to install PowerShell using command lines.
 
## How to install PowerShell using Snap command on Ubuntu
 
To update the PowerShell app on Linux, use these steps:
 
- Open Terminal.
 - Type the following command to install PowerShell and press Enter:
 - sudo snap install powershell --classic
 - Snap install PowerShell command

 
After you complete the steps, you can start the Microsoft scripting tool using the pwsh command in the Terminal.
 
Open Terminal.
 
Type the following command to install PowerShell and press Enter:
 
sudo snap install powershell --classic
 
Snap install PowerShell command

 
If you want to uninstall the tool, from the Terminal, type the sudo snap remove powershell command.
 
## How to install PowerShell using using Package Repository on Ubuntu
 
To install PowerShell on Linux using Package Repository, use these steps:
 
- Open Terminal.
 - Type the following command to download the Microsoft repository GPG keys and press Enter:
 - wget -q https://packages.microsoft.com/config/ubuntu/18.04/packages-microsoft-prod.deb
 - Type the following command to register the Microsoft repository GPG keys and press Enter:
 - sudo dpkg -i packages-microsoft-prod.deb
 - Package Microsoft prod command
 - Type the following command to update the list of products and press Enter:
 - sudo apt-get update
 - Type the following command to enable the “universe” repositories and press Enter:
 - sudo add-apt-repository universe
 - Type the following command to install PowerShell on Linux and press Enter:
 - sudo apt-get install -y powershell
 - Linux apt-get install PowerShell command

 
After you complete the steps, PowerShell will install on Ubuntu 18.04, and you can start it using the pwsh command.
 
Type the following command to download the Microsoft repository GPG keys and press Enter:
 
wget -q https://packages.microsoft.com/config/ubuntu/18.04/packages-microsoft-prod.deb
 
Type the following command to register the Microsoft repository GPG keys and press Enter:
 
sudo dpkg -i packages-microsoft-prod.deb
 
Package Microsoft prod command

 
Type the following command to update the list of products and press Enter:
 
sudo apt-get update
 
Type the following command to enable the “universe” repositories and press Enter:
 
sudo add-apt-repository universe
 
Type the following command to install PowerShell on Linux and press Enter:
 
sudo apt-get install -y powershell
 
Linux apt-get install PowerShell command

 
When you no longer need the command line tool, use the sudo apt-get remove powershell command in the Terminal to uninstall it.
 
### PowerShell dependencies
 
PowerShell builds portable binaries for all Linux distributions. However, Microsoft .NET Core runtime requires several dependencies on different flavors of Linux as well as PowerShell.
 
For example, on Ubuntu 18.04 and higher, the installation depends on libc6, libgcc1, libgssapi-krb5-2, liblttng-ust0, libstdc++6, libcurl3, libunwind8, libuuid1, zlib1g, libssl1.0.0, and libicu60.
 
If during the installation process, you come across dependency problems, you’ll have to find and install the components manually.
 
While preparing this guide, the installation of PowerShell 7 also required liblttng-ust0, libssl1.0.0, and libicu60. If you have the same issues, then you can get these packages with these commands:
 
- Open Terminal.
 - Type the following command to install liblttng-ust0 and press Enter:
 - sudo apt install liblttng-ust0
 - Type the following command to download libicu60 and press Enter:
 - wget http://security.ubuntu.com/ubuntu/pool/main/i/icu/libicu60_60.2-3ubuntu3.1_amd64.deb
 - Type the following command to install libicu60 and press Enter:
 - sudo dpkg -i libicu60_60.2-3ubuntu3.1_amd64.deb
 - Type the following command to download libssl1.0.0 and press Enter:
 - wget http://security.ubuntu.com/ubuntu/pool/main/o/openssl1.0/libssl1.0.0_1.0.2n-1ubuntu5.3_amd64.deb
 - Type the following command to install libicu60 and press Enter:
 - sudo dpkg -i libssl1.0.0_1.0.2n-1ubuntu5.3_amd64.deb
 - Type the following command to install PowerShell and Enter:
 - sudo apt-get install -y powershell

 
Once you complete the steps, PowerShell 7 should install on your Linux device.
 
Type the following command to install liblttng-ust0 and press Enter:
 
sudo apt install liblttng-ust0
 
Type the following command to download libicu60 and press Enter:
 
wget http://security.ubuntu.com/ubuntu/pool/main/i/icu/libicu60_60.2-3ubuntu3.1_amd64.deb
 
Type the following command to install libicu60 and press Enter:
 
sudo dpkg -i libicu60_60.2-3ubuntu3.1_amd64.deb
 
Type the following command to download libssl1.0.0 and press Enter:
 
wget http://security.ubuntu.com/ubuntu/pool/main/o/openssl1.0/libssl1.0.0_1.0.2n-1ubuntu5.3_amd64.deb
 
sudo dpkg -i libssl1.0.0_1.0.2n-1ubuntu5.3_amd64.deb
 
Type the following command to install PowerShell and Enter:
 
In case that you need to download a different version of the dependency packages, you can find them at the Ubuntu package repository.




