---
title: "Revolutionize Your Coding Game: Learn How to Install WSL2 and Unlock Endless Possibilities on Your Windows 10!"
ShowToc: true 
date: "2023-05-25"
author: "Christopher Butterfield"
---
*****
# Revolutionize Your Coding Game: Learn How to Install WSL2 and Unlock Endless Possibilities on Your Windows 10!

As a developer or programmer, you already know the importance of having a powerful and efficient system to work on. Whether you’re building applications, developing web pages or working with AI tools, having a computer that can handle all your demands is essential.

The good news is that as a Windows 10 user, you can now take advantage of the Windows Subsystem for Linux (WSL2), a feature that enables developers to run full versions of Linux directly on their Windows desktop without the need for a virtual machine.

In this article, we'll guide you through the process of installing WSL2 on your Windows 10 machine and show you how it can revolutionize your coding game and unlock endless possibilities.

## What is WSL2?

The Windows Subsystem for Linux (WSL) is a feature that allows developers to run Linux environments on Windows without the need for a virtual machine or other third-party software. WSL2 is the latest version that was released in mid-2020 and provides a new architecture that promises faster and more efficient performance than its predecessor.

With WSL2, you can run full versions of Linux on your Windows 10 desktop and access all the tools and utilities that come with Linux, such as the Bash shell, Git, Apache web server, and others. It also provides a seamless integration between the two operating systems, allowing you to access files and resources on either platform.

## Installing WSL2 on Windows 10

Before you can start using WSL2, you need to enable it on your Windows 10 machine. Here’s a step-by-step guide to help you get started:

1. Open the Start Menu and search for "Windows Features."

2. Select "Turn Windows features on or off" from the list of results.

3. Scroll down to find "Windows Subsystem for Linux" and check the box next to it.

4. Click the "OK" button to accept the changes and allow Windows to install the required files.

5. Restart your device to complete the installation process.

6. Once your device has restarted, open the Microsoft Store and search for "Ubuntu." Click the "Install" button to download and install the Ubuntu app on your Windows 10 machine.

7. Launch the Ubuntu app and start exploring the Linux environment on your Windows 10 device!

## Unlocking Endless Possibilities with WSL2

With WSL2 installed on your Windows 10 machine, you can now access a whole new world of tools and utilities that were previously unavailable on Windows. Here are just a few examples of what you can do with WSL2:

- Run Linux-based applications directly on your Windows 10 desktop, such as Apache web server, MySQL database, and PHP programming language.

- Run command-line tools and utilities that are only available on Linux, such as the Bash shell, Git, and others.

- Create and experiment with different Linux-based development environments, such as Python, Ruby, Node.js, and others.

- Access the vast repositories of open-source software available on Linux and add new tools to your programming arsenal.

- Test and debug software on multiple operating systems without the need for virtual machines or other third-party software.

In conclusion, installing WSL2 on your Windows 10 machine can revolutionize your coding game and unlock endless possibilities for your development work. It provides a seamless integration between Windows and Linux, giving you access to powerful tools and utilities that were previously unavailable on Windows. So why not give it a try and see how WSL2 can take your programming skills to the next level?

{{< youtube 1ap3hL-UR9I >}} 



- To install WSL2 on Windows 10, open Command Prompt as admin and run “wsl –install.”
 - The command will install all the WSL2 components and the Ubuntu Linux distro.
 - To install a specific distro, run “wsl –install -d DISTRO-NAME.”
 - To update the WSL2 kernel, run the “wsl –update” command.

 
WSL2 (Windows Subsystem for Linux version 2) is a new version of the architecture that allows you to use Linux on top of Windows 10 natively (using a lightweight virtual machine) and replaces WSL.
 
The feature runs an actual Linux kernel in a virtual machine, which improves performance and app compatibility over the previous version while maintaining the same experience as the first release.
 
This guide will teach you the steps to install the Windows Subsystem for Linux 2 on Windows 10.
 
- Install WSL2 on Windows 10
 - Install WSL2 on Windows 10 (older versions)

 
## Install WSL2 on Windows 10
 
Microsoft has simplified the installation process of the WSL on Windows 10 to only one command that downloads and installs all the required components, including the virtual machine platform and Ubuntu Linux by default.
 
To install Windows Subsystem for Linux on Windows 10, use these steps:
 
- Open Start on Windows 10.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to install the WSL on Windows 10 and press Enter:
 - wsl --install
 - Restart your computer to finish the WSL installation on Windows 10.
 - Continue with the Linux distro setup as necessary.

 
Once you complete the steps, the required Linux components will automatically install the latest version of the Ubuntu Linux distribution.
 
Open Start on Windows 10.
 
Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 
Type the following command to install the WSL on Windows 10 and press Enter:
 
wsl --install
 

 
Restart your computer to finish the WSL installation on Windows 10.
 
Continue with the Linux distro setup as necessary.
 
### Install WSL with specific distro
 
To install WSL with a specific distro on Windows 10, use these steps:
 
- Open Start.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to view a list of available WSL distros to install on Windows 10 and press Enter:
 - wsl --list --online
 - Quick note: At the time of this writing, you can install Ubuntu, Debian, Kali Linux, openSUSE, and SUSE Linux Enterprise Server.
 - Type the following command to install the WSL with a specific distro on Windows 10 and press Enter:
 - wsl --install -d DISTRO-NAME
 - Remember to replace “DISTRO-NAME” in the command with the distro’s name to install, such as Debian.
 - Restart your computer.
 - Continue with the Linux distro setup as necessary.

 
After you complete the steps, the Windows Subsystem for Linux 2 components will install with the distro of Linux you specified. 
 
Open Start.
 
Type the following command to view a list of available WSL distros to install on Windows 10 and press Enter:
 
wsl --list --online
 
Type the following command to install the WSL with a specific distro on Windows 10 and press Enter:
 
wsl --install -d DISTRO-NAME
 
Remember to replace “DISTRO-NAME” in the command with the distro’s name to install, such as Debian.
 
Restart your computer.
 
### Update WSL kernel
 
To update the WSL kernel to the latest version on Windows 10, use these steps:
 
- Open Start.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to update the WSL kernel and press Enter:
 - wsl --update

 
Once you complete the steps, if an update is available, it will download and install on the device.
 
Type the following command to update the WSL kernel and press Enter:
 
wsl --update
 
If the update command doesn’t work, open Settings > Update & Security > Windows Update > Advanced options, and turn on the “Receive updates for other Microsoft products when you update Windows” toggle switch.
 
## Install WSL2 on Windows 10 (older versions)
 
Alternatively, you can still install WSL on Windows 10 version 1909 and older versions using the legacy processes. The process requires enabling WSL1, the Virtual Machine Platform, converting existing distros (if applicable), and configuring the Windows Subsystem for Linux 2 as the new default for future distro installations.
 
If you have an ARM64 system, the Linux integration is supported on version 2004 and higher.
 
### Enable Windows Subsystem for Linux
 
If you are not already using Linux on Windows 10, you must enable the Windows Subsystem for Linux (version 1) with these steps:
 
- Open Start on Windows 10.
 - Search for Turn Windows features on or off and click the top result to open the app.
 - Check the “Windows Subsystem for Linux” option.
 - Click the OK button.
 - Click the Restart button.

 
Once you complete the steps, you must enable the Virtual Machine Platform feature.
 
Search for Turn Windows features on or off and click the top result to open the app.
 
Check the “Windows Subsystem for Linux” option.
 
Click the OK button.
 
Click the Restart button.
 
### Enable Virtual Machine Platform
 
To enable the Virtual Machine Platform on Windows 10, use these steps:
 
- Open Start.
 - Search for PowerShell, right-click the top result, and select the Run as administrator option.
 - Type the following command to enable the Virtual Machine Platform feature and press Enter:
 - Enable-WindowsOptionalFeature -Online -FeatureName VirtualMachinePlatform
 - Restart your computer.

 
After you complete the steps, you can set the Windows Subsystem for Linux version 2 as the new default architecture and convert existing distros.
 
Search for PowerShell, right-click the top result, and select the Run as administrator option.
 
Type the following command to enable the Virtual Machine Platform feature and press Enter:
 
Enable-WindowsOptionalFeature -Online -FeatureName VirtualMachinePlatform
 
### Enable Windows Subsystem for Linux 2
 
To start using WSL2 or covert WSL distros to WSL2, use these steps:
 
- Download this WSL 2 kernel update (required).
 - Double-click the wsl_update_x64.msi file and apply the update.
 - Open Start.
 - Search for PowerShell, right-click the top result, and select the Run as administrator option.
 - Type the following command to set Windows Subsystem for Linux 2 your default architecture for new distros that you install, and press Enter:
 - wsl --set-default-version 2
 - (Optional) Type the following command to convert the distro from WSL to WSL 2 and press Enter:
 - wsl --set-version Ubuntu 2
 - In the command, change “Ubuntu” for the distro’s name you want to convert. If you do not know the distro’s name, use the wsl -l -v command.

 
Once you complete the steps, your device will start using the new version of Windows Subsystem for Linux as the default architecture. (See video tutorial on the Pureinfotech YouTube channel.)
 
Download this WSL 2 kernel update (required).
 
Double-click the wsl_update_x64.msi file and apply the update.
 
Type the following command to set Windows Subsystem for Linux 2 your default architecture for new distros that you install, and press Enter:
 
wsl --set-default-version 2
 
(Optional) Type the following command to convert the distro from WSL to WSL 2 and press Enter:
 
wsl --set-version Ubuntu 2
 
In the command, change “Ubuntu” for the distro’s name you want to convert. If you do not know the distro’s name, use the wsl -l -v command.
 
### Confirm distro platform
 
To confirm distros are using the Windows Subsystem for Linux 2, use these steps:
 
- Open Start.
 - Search for PowerShell, right-click the top result, and select the Run as administrator option.
 - Type the following command to verify the version of the distro and press Enter:
 - wsl --list --verbose
 - Confirm the distro version is 2.

 
After you complete the steps, you will know if the process was successful or if you need to troubleshoot any of the steps.
 
Type the following command to verify the version of the distro and press Enter:
 
wsl --list --verbose
 
Confirm the distro version is 2.




