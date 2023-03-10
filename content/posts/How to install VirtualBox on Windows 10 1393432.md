---
title: "Revolutionize Your Computer Experience: Learn How To Install VirtualBox on Windows 10 now!"
ShowToc: true 
date: "2023-06-26"
author: "Angel Trax"
---
*****
# Revolutionize Your Computer Experience: Learn How To Install VirtualBox on Windows 10 now!

Are you tired of running multiple operating systems on different machines or partitions? Or are you a developer who needs to test their application on different operating systems? If yes, then it's time to revolutionize your computer experience with VirtualBox.

VirtualBox is a powerful virtualization tool that lets you run multiple operating systems on a single machine. It's a free and open-source software that is compatible with Windows, macOS, Linux, and other operating systems. In this article, we will guide you on how to install VirtualBox on Windows 10.

## Step 1: Download VirtualBox

The first step is to download VirtualBox from the official website. You can download the installer for Windows hosts, which is a self-extracting executable file. The latest version of VirtualBox is 6.1.26 at the time of writing this article.

## Step 2: Install VirtualBox

Once you've downloaded the VirtualBox installer, double-click on the executable file to start the installation process. Follow the installation wizard and accept the license agreement. You can also choose the location where you want to install VirtualBox.

## Step 3: Configure VirtualBox

After the installation is complete, launch VirtualBox from the start menu or desktop shortcut. In the VirtualBox Manager window, click on the "New" button to create a new virtual machine.

Give your virtual machine a name and select the operating system you want to install. You can choose from a wide range of operating systems, including different versions of Windows, Linux, macOS, and more. You can also select the amount of RAM and storage space you want to allocate to your virtual machine.

## Step 4: Install the Operating System

Once you've configured your virtual machine, it's time to install the operating system. Select the virtual machine and click on the "Start" button. VirtualBox will prompt you to select an installation media, which can be an ISO image file or a physical CD/DVD.

Follow the operating system's installation wizard and complete the installation process. Once the installation is complete, you should be able to run your virtual machine from the VirtualBox Manager window.

## Step 5: Customize your Virtual Machine

VirtualBox offers several advanced features to customize your virtual machine. You can configure the network settings, create snapshots, and even share folders between your virtual machine and the host operating system.

## Conclusion

In conclusion, VirtualBox is a powerful virtualization tool that lets you run multiple operating systems on a single PC. It's easy to install and configure, and it's free and open-source software. By following the steps outlined in this article, you can revolutionize your computer experience by learning how to install VirtualBox on Windows 10. So, what are you waiting for? Start experimenting with different operating systems today!

{{< youtube wX75Z-4MEoM >}} 



Oracle’s VirtualBox is a free virtualization application that you can install on Windows 10, Mac, and Linux to create and use virtual machines to run other versions of Windows or other platforms alongside the main operating system without the need to set up dual-boot or configure another computer.
 
Usually, you would use this virtualization technology to test pre-releases of Windows 10 available through the Windows Insider Program, run other operating systems like Ubuntu or Kali Linux, or create another virtual machine to test software without affecting the main installation.
 
VirtualBox has been designed to run on Intel as well as AMD hardware. While it is meant to be an enterprise product, it’s also available for home use with support for many guests operating systems, including Windows 10, Windows 8, Windows 7, Vista, and older version, Linux (2.4, 2.6, 3.x and 4.x), Solaris and OpenSolaris, OS/2, OpenBSD, and many more.
 
In this guide, you will learn steps to install and configure the basic settings to get started with VirtualBox on Windows 10.
 
- Install VirtualBox on Windows 10
 - Configure VirtualBox on Windows 10
 - Install VirtualBox extension pack on Windows 10

 
## Install VirtualBox on Windows 10
 
To install VirtualBox on Windows 10, use these steps:
 
- Open Oracle download page.
 - Under the “VirtualBox binaries” section, click the Windows hosts link and save the installers on your Windows 10 device.
 - VirtualBox download page
 - Double-click the VirtualBox-x.x.x-x-Win.exe file to launch the installer.
 - Click the Next button.
 - Use the default settings selection, and click the Next button.
 - VirtualBox default install settings
 - (Optional) Clear the options you do not want to use.
 - Click the Next button to continue with VirtualBox install on Windows 10.
 - Custom setup options
 - Click the Yes button to confirm the virtual network adapter install warning on Windows 10.
 - VirtualBox network adapter warning
 - Click the Install button (if applicable).
 - Click the Finish button.

 
Once you complete the steps, the software will finish the installation, and it will launch automatically. You can also launch VirtualBox from the Start menu like any other application.
 
Open Oracle download page.
 
Under the “VirtualBox binaries” section, click the Windows hosts link and save the installers on your Windows 10 device.
 
VirtualBox download page

 
Double-click the VirtualBox-x.x.x-x-Win.exe file to launch the installer.
 
Click the Next button.
 
Use the default settings selection, and click the Next button.
 
VirtualBox default install settings

 
(Optional) Clear the options you do not want to use.
 
Click the Next button to continue with VirtualBox install on Windows 10.
 
Custom setup options

 
Click the Yes button to confirm the virtual network adapter install warning on Windows 10.
 
VirtualBox network adapter warning

 
Click the Install button (if applicable).
 
Click the Finish button.
 
### Installation with winget command
 
Alternatively, you can also install VirtualBox using the Windows Package Manager (winget) in Command Prompt.
 
To install VirtualBox with the winget command, use these steps:
 
- Open Start.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - (Optional) Type the following command to search for the name of the application and press Enter:
 - winget search virtualbox
 - Quick note: While the search command is not required, the install query must match the ID, name, or moniker of the package, which can change at any time. So, it’s a good practice to search the application to execute the correct install command.
 - Type the following command to install VirtualBox on Windows 10 with winget and press Enter:
 - winget install Oracle.VirtualBox
 - winget install VirtualBox

 
After you complete the steps, the package manager will download and install the virtualization application without extra steps.
 
Open Start.
 
Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 
(Optional) Type the following command to search for the name of the application and press Enter:
 
winget search virtualbox
 
Type the following command to install VirtualBox on Windows 10 with winget and press Enter:
 
winget install Oracle.VirtualBox
 
winget install VirtualBox

 
## Configure VirtualBox on Windows 10
 
Although the default settings will suit more users, VirtualBox comes with many settings and features. In the steps below, we will outline some of the most basic ones everyone should consider changing when working with virtual machines.
 
To configure VirtualBox settings, use these steps:
 
- Open VirtualBox.
 - Click the File menu and select the Preferences option.
 - VirtualBox preferences
 - Click on General.
 - In the Default Machine Folder option, specify the folder location to store the virtual machines on Windows 10. Usually, you want to use an external hard drive since using the primary drive can slow down the system.
 - Change VM default folder location
 - Click on Update.
 - Select the Check for updates option.
 - Confirm the update settings and whether you want to use pre-releases of the software.
 - VirtualBox update settings
 - (Optional) Click on Display.
 - In the Maximum Guest Screen size option, specify the maximum screen resolution for virtual machines.
 - Maximum guest screen size settings
 - Quick tip: You can also select the “Hint” option to create a default maximum screen resolution. Usually, you want to leave the default settings and configure the resolution in the virtual machine settings.
 - In the Scale Factor option, select the scale virtual machines should use to make text and visual elements smaller or bigger.
 - Click the OK button.

 
After you complete the steps, the custom configuration will apply to the virtualization software.
 
Open VirtualBox.
 
Click the File menu and select the Preferences option.
 
VirtualBox preferences

 
Click on General.
 
In the Default Machine Folder option, specify the folder location to store the virtual machines on Windows 10. Usually, you want to use an external hard drive since using the primary drive can slow down the system.
 
Change VM default folder location

 
Click on Update.
 
Select the Check for updates option.
 
Confirm the update settings and whether you want to use pre-releases of the software.
 
VirtualBox update settings

 
(Optional) Click on Display.
 
In the Maximum Guest Screen size option, specify the maximum screen resolution for virtual machines.
 
In the Scale Factor option, select the scale virtual machines should use to make text and visual elements smaller or bigger.
 
Click the OK button.
 
Since the virtualization application configures NAT (Network Address Translation) automatically on each host you create, you do not need to configure the networking settings to get started. However, VirtualBox includes networking settings to create different host-only adapters and bridges, internal networks, and more.
 
## Install VirtualBox extension pack on Windows 10
 
The extension pack is not a requirement, but it enables USB 2.0 and 3.0 devices, VirtualBox RDP, drive encryption, NVMe, and PXE boot for Intel Cards.
 
To install the extension pack for VirtualBox, use these steps:
 
- Open Oracle download page.
 - Under the “VirtualBox Extension Pack” section, click the All supported platforms link to download the latest pack.
 - Download VirtualBox extension pack
 - Open VirtualBox.
 - Click the File menu and select the Preferences option.
 - Click on Extensions.
 - Click the Adds new package button in the top-right corner.
 - Extension settings
 - Select the “.vbox-extpack” file containing the extensions.
 - vbox-extpack file
 - Click the Open button.
 - Click the Install button.
 - Install extension pack
 - Scroll down the page.
 - Click the I agree button to confirm the terms option.
 - Click the OK button.
 - Click the OK button again.

 
Once you complete the steps, the Oracle VM VirtualBox Extension Pack will install on the device. Then you can proceed with the virtual machine creation, followed by the Guest Additions installation.
 
Under the “VirtualBox Extension Pack” section, click the All supported platforms link to download the latest pack.
 
Download VirtualBox extension pack

 
Click on Extensions.
 
Click the Adds new package button in the top-right corner.
 
Extension settings

 
Select the “.vbox-extpack” file containing the extensions.
 
vbox-extpack file

 
Click the Open button.
 
Click the Install button.
 
Install extension pack

 
Scroll down the page.
 
Click the I agree button to confirm the terms option.
 
Click the OK button again.
 
If you want to remove it, select the package on the “Extensions” page, and click the Remove Selected Package button in the top-right.




