---
title: "Unleash the Power of Linux on Windows 11 - Easy Guide to Install WSL in a Few Clicks!"
ShowToc: true 
date: "2023-01-16"
author: "Louisa Decourcey"
---
*****
Title: Unleash the Power of Linux on Windows 11 - Easy Guide to Install WSL in a Few Clicks!

Are you a developer or a power user who loves Linux but is forced to work on Windows for one reason or another? Do you miss the power and flexibility of the Linux command-line interface? Well, good news, my friend! With the introduction of Windows Subsystem for Linux (WSL), you can now run a full-fledged Linux environment right on your Windows 11 machine! In this article, we'll walk you through the process of installing WSL, and show you how to get started with Linux on Windows 11. So, grab a cup of coffee, sit back, and let's begin!

What is WSL?

The Windows Subsystem for Linux (WSL) is a feature that allows users to install and run a Linux environment directly on their Windows machine. It provides a fully-functional Linux kernel and allows you to run Linux commands and tools natively on Windows, without the need for a virtual machine or a dual-boot setup.

WSL comes in two flavors: WSL1 and WSL2. WSL1 is a compatibility layer that translates Linux system calls into Windows system calls, while WSL2 is a virtualized environment that runs a full-fledged Linux kernel. WSL2 provides better performance and more accurate compatibility with Linux file systems and devices.

How to install WSL on Windows 11

Installing WSL is a straightforward process that can be completed in a few clicks. Here's how to do it:

Step 1 - Enable the Windows Subsystem for Linux feature:

Go to Settings -> Apps -> Apps & features -> Optional features -> Add a feature -> Windows Subsystem for Linux -> Install

Step 2 - Download and install a Linux distribution of your choice:

Go to the Microsoft Store and search for the Linux distribution you want to install. There are several popular distributions available, including Ubuntu, Debian, and Kali Linux. Click on the distribution you want to install, and then click on the "Get" button to download and install it.

Step 3 - Launch the Linux distribution:

Once the installation is complete, you can launch the Linux distribution from the Start menu, or by typing its name in the search bar. The first time you launch the distribution, it will take a few minutes to set up the environment and configure your user account.

Step 4 - Update the Linux distribution:

After launching the Linux distribution, run the following command to update it to the latest version:

sudo apt update && sudo apt upgrade

That's it! You now have a fully-functional Linux environment running on your Windows 11 machine.

Getting started with Linux on Windows

Now that you have installed WSL and a Linux distribution, the next step is to start using it. Here are a few tips to get you started:

1. Use the Windows Terminal app to launch and manage multiple Linux distributions.

2. Use the "wsl" command to launch Linux commands from the Windows command prompt.

3. Use the Linux "apt" package manager to install and update software packages.

4. Use the "nano" or "vi" text editors to edit text files.

5. Use the "ssh" command to connect to remote Linux servers.

6. Use the Linux file system to access and manipulate your Windows files.

Conclusion

Windows Subsystem for Linux (WSL) is a powerful feature that allows Windows users to run a Linux environment directly on their machines. With WSL, you can enjoy the power and flexibility of the Linux command-line interface, without the need for a virtual machine or a dual-boot setup. In this article, we showed you how to install WSL on Windows 11, and gave you some tips on getting started with Linux on Windows. So, what are you waiting for? Go ahead and unleash the power of Linux on your Windows 11 machine!

{{< youtube 28Ei63qtquQ >}} 



- To install WSL on Windows 11, open PowerShell or Command Prompt (admin), run the “wsl –install” command, and restart the computer.
 - The command will install WSL alongside the Ubuntu distribution.
 - Or, to install WSL with a specific distro, run the “wsl –install -d DISTRO-NAME” command.
 - Or, to install WSL from Microsoft Store, enable the “Virtual Machine Platform” feature and then download the WSL app from the Store.

 
On Windows 11, Microsoft simplified the installation process of the Windows Subsystem for Linux 2 (WSL) to only one command to download and install all the required components, which includes the virtual machine platform and Linux GUI apps.
 
In addition, the command also installs the latest Ubuntu distro by default. If you prefer another distribution of Linux, you can append an option in the command to install any of the supported distros. Alongside the new quick and easy process, you will also find another way to make it easier to update the kernel with only one command.
 
This guide will teach you the easy steps to install the WSL platform on your computer. In addition, we will outline the steps to update the Linux kernel on Windows 11.
 
- Install WSL on Windows 11
 - Install WSL with specific distro on Windows 11
 - Update WSL kernel on Windows 11
 - Install WSL from Microsoft Store

 
## Install WSL on Windows 11
 
To install WSL (Windows Subsystem for Linux) on Windows 11 from Command Prompt, use these steps:
 
- Open Start on Windows 11.
 - Search for Command Prompt (or PowerShell), right-click the top result and select the Run as administrator option.
 - Type the following command to install the WSL on Windows 11 and press Enter:
 - wsl --install
 - Restart your computer to finish the WSL installation on Windows 11.
 - Continue with the Linux distro setup as necessary.

 
After you complete the steps, the required Linux components will install automatically on Windows 11 and the latest version of the Ubuntu Linux distribution.
 
Open Start on Windows 11.
 
Search for Command Prompt (or PowerShell), right-click the top result and select the Run as administrator option.
 
Type the following command to install the WSL on Windows 11 and press Enter:
 
wsl --install
 

 
Restart your computer to finish the WSL installation on Windows 11.
 
Continue with the Linux distro setup as necessary.
 
## Install WSL with specific distro on Windows 11
 
If you prefer another flavor of Linux, the WSL2 command includes an option to view and select a different distro.
 
To install WSL with a specific distro on Windows 11, use these steps:
 
- Open Start.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to view a list of available WSL distros you can install on Windows 11 and press Enter:
 - wsl --list --online
 - Quick note: You can install Ubuntu, Debian, Kali Linux, openSUSE, and SUSE Linux Enterprise Server.
 - Type the following command to install the WSL with a specific distro on Windows 11 and press Enter:
 - wsl --install -d DISTRO-NAME
 - In the command, remember to replace “DISTRO-NAME” with the name of the distro you want to install, such as Debian.
 - Restart your computer to finish the WSL installation on Windows 11.
 - Continue with the Linux distro setup as necessary.

 
Once you complete the steps, the Windows Subsystem for Linux 2 components will install along with the distro of Linux you specified. 
 
Open Start.
 
Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 
Type the following command to view a list of available WSL distros you can install on Windows 11 and press Enter:
 
wsl --list --online
 
Type the following command to install the WSL with a specific distro on Windows 11 and press Enter:
 
wsl --install -d DISTRO-NAME
 
In the command, remember to replace “DISTRO-NAME” with the name of the distro you want to install, such as Debian.
 
## Update WSL kernel on Windows 11
 
To update the WSL kernel from Command Prompt, use these steps:
 
- Open Start.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to update the WSL kernel on Windows 11 and press Enter:
 - wsl --update

 
After you complete the steps, if an update is available, it will download and install on your computer.
 
Type the following command to update the WSL kernel on Windows 11 and press Enter:
 
wsl --update
 
## Install WSL from Microsoft Store
 
You can also download all the components wrapped into an app from the Microsoft Store. The benefit of using this approach is that feature will run isolated from Windows 11, and updates will be available through the Microsoft Store without waiting for the next version of the operating system to install the newest version.
 
To install WSL from the Microsoft Store, use these steps:
 
### 1. Enable Virtual Machine Platform
 
- Open Start.
 - Search for Turn Windows Features on or off and click the top result to open the app.
 - Check the Virtual Machine Platform option.
 - Click the OK button.
 - Click the Restart button.

 
After completing the steps, you can download the app from the Microsoft Store.
 
Search for Turn Windows Features on or off and click the top result to open the app.
 
Check the Virtual Machine Platform option.
 
Click the OK button.
 
Click the Restart button.
 
### 2. Install Windows Subsystem for Linux app
 
- Open the Windows Subsystem for Linux store page.
 - Click the Get button.
 - Click the Open button.
 - Click the Get button again.

 
### 3. Install Linux distro
 
- Open Microsoft Store app.
 - Search for the Linux distro. For example, Debian.
 - Click the Get button.
 - Click the Open button.

 
Once you complete the steps, WSL will install on Windows 11, including the support for Linux GUI apps and the Linux distribution.
 
Open the Windows Subsystem for Linux store page.
 
Click the Get button.
 
Click the Open button.
 
Click the Get button again.
 
Open Microsoft Store app.
 
Search for the Linux distro. For example, Debian.




