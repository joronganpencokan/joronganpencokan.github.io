---
title: "Unlock the Secret to Effortlessly Mounting ISO Files on Virtual Machines with Virtualbox!"
ShowToc: true 
date: "2023-02-01"
author: "Kathryn Claudio"
---
*****
Introduction

Virtual Machines are a crucial aspect of modern computing. They allow developers and other tech enthusiasts to run multiple operating systems simultaneously on one computer. Among the many benefits of using virtual machines is that it creates an environment for testing, development, and even running multiple applications without interfering with the primary operating system.

Virtualbox is an open-source virtualization tool that offers a wide range of functionalities. One of the significant features of Virtualbox is its capability to mount ISO files on Virtual Machines. The process of mounting an ISO file on Virtualbox might seem complicated initially, but with a few steps, the process can be effortless. In this article, we will unlock the secret to effortlessly mounting ISO files on Virtual Machines with Virtualbox.

Step 1: Download Virtualbox

The first step to mounting ISO files on Virtual Machines is to download Virtualbox. Virtualbox is available for free on the Oracle website or any other reliable website. Once the download is complete, install the application and launch it.

Step 2: Create a new Virtual Machine

After launching Virtualbox, click on the "New" button to create a new Virtual Machine. A new dialog box will appear prompting you to input the name of the Virtual Machine, the type of operating system, and the version. Input the necessary details and click "Next" to proceed to the next step.

Step 3: Allocate memory and hard disk space

In this step, allocate memory and hard disk space for your Virtual Machine. Allocate enough memory depending on the requirements of the operating system. Also, ensure that you allocate sufficient disk space for the Virtual Machine to function correctly.

Step 4: Configure settings

After allocating memory and hard disk space, click on the "Settings" button to configure additional settings such as network settings, display settings, and USB settings. Configure these settings according to your preference and click "OK" to proceed.

Step 5: Mount ISO file

Lastly, it's time to mount the ISO file on your Virtual Machine. Click on the "Storage" tab and then "Add CD/DVD Device." On the right side of the screen, click on the "Choose Virtual Optical Disk File" option and browse through your computer's files to locate the ISO file. Select the ISO file and click "OK."

Conclusion

That's it! Following these five steps should help you effortlessly mount ISO files on Virtual Machines with Virtualbox. Additionally, when creating a Virtual Machine in the first step, ensure that the operating system version matches the specifications of your ISO file. The process of mounting an ISO file may seem complex to some, but with time it becomes easy and familiar, especially with practice. Happy virtualizing!

{{< youtube l75sHNKhnn0 >}} 



On VirtualBox, if you create a virtual machine or install an application on the guest machine, you will probably need to mount an ISO file to access the setup files.
 
An ISO file is a container (also called a “disk image”) containing an exact copy of all the contents available on a physical disc. Also, since no physical discs are involved, it has become the most common medium to ship software and other information over the internet.
 
If you use VirtualBox, you can connect ISO files in at least two ways through the VirtualBox Manager or from the virtual machine interface when the guest operating system is running.
 
This guide will teach you two ways to insert an ISO file into a VirtualBox virtual machine on Windows 10 (or 11).
 
- Mount ISO to a virtual machine with VirtualBox Manager
 - Mount ISO to a running virtual machine on VirtualBox

 
## Mount ISO to a virtual machine with VirtualBox Manager
 
To mount an ISO file to a VM through the VirtualBox Manager, use these steps:
 
- Open VirtualBox.
 - Right-click the virtual machine and select the Settings option.
 - Click on Storage.
 - Under the “Storage Drives” section, select the disc (Empty) item.
 - Under the “Attributes” section, click the disc icon and select the Choose a disk file button.
 - Select the ISO file.
 - Click the Open button.
 - (Optional) Check the Live CD/DVD option to keep the ISO mount even when the guest operating system tries to eject it.
 - (Optional) Check the Hot-pluggable option to make the virtual drive appear as a hot-pluggable peripheral.
 - Click the OK button.

 
Once you complete the steps, the ISO file will mount to the virtual machine. The setup will appear on the guest device if this is an installation media. If you connect the image to a virtual machine with an OS, the disk will appear in the operating system.
 
Open VirtualBox.
 
Right-click the virtual machine and select the Settings option.
 

 
Click on Storage.
 
Under the “Storage Drives” section, select the disc (Empty) item.
 
Under the “Attributes” section, click the disc icon and select the Choose a disk file button.
 
Select the ISO file.
 
Click the Open button.
 
(Optional) Check the Live CD/DVD option to keep the ISO mount even when the guest operating system tries to eject it.
 
(Optional) Check the Hot-pluggable option to make the virtual drive appear as a hot-pluggable peripheral.
 
Click the OK button.
 
If you want to unmount the ISO file, click the “Choose a disk file” button while in the “Storage” settings and select the “Remove disk from virtual drive” option.
 
## Mount ISO to a running virtual machine on VirtualBox
 
To mount an image file while the VirtualBox guest machine is running, use these steps:
 
- Open VirtualBox.
 - Right-click the virtual machine, select the Start submenu and choose the Normal start option.
 - Click the Devices menu.
 - Select the Optical Drives submenu and the “Choose a disk file” option.
 - Select the ISO file.
 - Click the Open button.

 
After you complete the steps, the ISO file will mount to a virtual drive.
 
Right-click the virtual machine, select the Start submenu and choose the Normal start option.
 
Click the Devices menu.
 
Select the Optical Drives submenu and the “Choose a disk file” option.
 
If you want to unmount the ISO file on Windows 11 (or 10), open File Explorer, right-click the disk drive in “This PC,” and select the Eject option.
 
Alternatively, on VirtualBox, you can open the “Devices” menu, select the “Optical Drivers” submenu, and choose the “Remove disk from virtual drive” option.
 
If the optical device feature doesn’t work, you could alternatively mount the image to the host operating system, extract its content, and then make it available to the guest machine using a shared folder.




