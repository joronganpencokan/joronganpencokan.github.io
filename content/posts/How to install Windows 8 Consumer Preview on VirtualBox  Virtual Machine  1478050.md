---
title: "Unlock the Secret to Installing Windows 8 Consumer Preview on Virtualbox in Just 5 Easy Steps!"
ShowToc: true 
date: "2023-03-15"
author: "Mary Bouknight"
---
*****
Unlock the Secret to Installing Windows 8 Consumer Preview on Virtualbox in Just 5 Easy Steps!

If you are a tech enthusiast, you may be thrilled with the prospect of installing Windows 8 Consumer Preview on your computer to test its features. However, you may have reservations about doing so on your main system, as it may disrupt your workflow or cause compatibility issues with your applications. Fortunately, you can use a virtual machine to install Windows 8 Consumer Preview without jeopardizing your primary OS. Moreover, you can employ Virtualbox, a free and open-source virtualization software, to run Windows 8 smoothly and securely. In this article, we will guide you through the process of setting up Virtualbox and installing Windows 8 Consumer Preview on it in just five easy steps.

Step One: Download and Install Virtualbox

First, you need to download and install Virtualbox from the official website (https://www.virtualbox.org/). Make sure you select the correct version for your operating system. Once you have downloaded the installation file, run it and follow the on-screen instructions to complete the installation. Virtualbox is a user-friendly software that does not require any advanced settings, so you should be able to install it without any issues.

Step Two: Create a New Virtual Machine

After you have installed Virtualbox, launch it and click on the "New" button on the top left corner of the window. This will open the "Create Virtual Machine" wizard, where you need to specify the name and operating system of your virtual machine. Since you want to install Windows 8 Consumer Preview, select "Windows" as the type and "Windows 8 (64-bit)" as the version. If you have a 32-bit computer, choose "Windows 8 (32-bit)" instead. Click on "Next" to proceed.

Step Three: Allocate Resources

In this step, you need to allocate resources to your virtual machine, such as the amount of RAM, CPU cores, and storage. The recommended minimum for Windows 8 Consumer Preview is 2 GB of RAM, 2 CPU cores, and 20 GB of storage. However, you can adjust these values according to your preferences and available hardware. Keep in mind that allocating too many resources to your virtual machine may affect the performance of your host system. Click on "Next" to proceed.

Step Four: Create a Virtual Hard Disk

In this step, you need to create a virtual hard disk for your virtual machine. This disk will serve as the storage space for your Windows 8 installation. You can choose between a dynamically allocated or a fixed-size virtual disk. A dynamically allocated disk will expand as you add more data to it, whereas a fixed-size disk will assume its maximum size at the start. Choose the option that suits your needs and select a location for your virtual disk. Keep in mind that the size of the disk should be at least 20 GB for Windows 8 Consumer Preview. Click on "Create" to proceed.

Step Five: Install Windows 8 Consumer Preview

In this final step, you need to install Windows 8 Consumer Preview on your virtual machine. To do so, click on the "Start" button on the top left corner of the Virtualbox window. This will launch your virtual machine and prompt you to select the installation media for Windows 8. You can either use a DVD, a USB flash drive, or an ISO image of Windows 8 Consumer Preview. Once you have selected the media, click on "Start" to begin the installation process. Follow the on-screen instructions to install Windows 8, but make sure to choose the virtual disk you created earlier as the destination for the OS. After the installation is complete, you should be able to run Windows 8 Consumer Preview in Virtualbox.

In conclusion, installing Windows 8 Consumer Preview on Virtualbox is a straightforward process that can help you explore the new features of the OS without jeopardizing your primary operating system. By following these five easy steps, you can set up Virtualbox, create a virtual machine, allocate resources, create a virtual hard disk, and install Windows 8 Consumer Preview in just a few minutes. So why not give it a try and see what Windows 8 has to offer?

{{< youtube ydGLx1Mn3u0 >}} 



Learn step-by-step how to install Windows 8 Consumer Preview on VirtualBox avoiding scary errors.
 
Even though Microsoft recommends to install Windows 8 Consumer Preview on a physical machine, many people only have one computer, the one they use everyday for work, email, browsing, banking, etc., and installing a pre-release operating system in a primary machine is not a wise idea — if you have a spare machine lying around in the house, go ahead with that option and follow these instructions to successfully complete the Windows Setup, but if you don’t have it, do not risk it.
 
One solution for these users will be using a virtual machine, and you can use VMware Workstation, you can also use VirtualBox (the one we are going to use today), which is a virtualization software from Oracle that works in the same way as VMware, or other type of virtualization solution.
 
Now Consumer Preview is more stable that previous releases, so this time around it’ll be easier to create a virtual machine using VirtualBox that how it was in the past with Developer Preview.
 

 
## Instructions
 
Before we start, you’ll need to download and install VirtualBox if you haven’t done so. When you done with this installation continue with the process:
 
1.  Open VirtualBox, to create a new virtual machine, click New and in the welcome wizard, click Next.
 
2.  In the VM Name and OS Type step: name your virtual machine with a descriptive name, and in the OS Type make sure that Operating System is on Microsoft Windows and the version to Windows 8. Then click Next.
 
3.  Set the amount of memory to at least 1024MB and click Next.
 
4.  In Virtual Hard Disk leave the default settings and click Next, a new dialog box (refer to the second image below) will appear, which will guide you in the creation of a virtual disk, select VDI (VirtualBox Disk IMage) and click Next.
 
5.  Now in Virtual disk storage details, leave the default setting Dynamically allocated and click Next.
 
6.  The next step is Virtual disk file location and size, there do just that: choose the location where to store the virtual machine — you may find that saving the virtual machine in another hard drive will boost performance — and don’t forget the name of the folder that will contain the VM. Windows 8 Consumer Preview requires a minimum of 16GB of free space for the 32-bit version, so to be safe set the disk size to 20GB, which is the minimum requirement for the 64-bit version, then click Next.
 
7.  Then you’ll get a summary of your virtual machine in VirtualBox, click Create and Create one more time.
 
8.  Select the VM that you just created, click Settings and navigate to Storage, under IDE Controller, select Empty, and on the right, click the CD icon to browse and locate the Windows 8 Consumer Preview ISO image, and click OK to finish with the settings customization.
 
4. Next start the virtual machine and if everything went according to plan, you will see the Windows Setup for Windows 8 Consumer Preview.
 
If you need some help going through the Windows Setup head over to this article — Walkthrough Windows 8 Consumer Preview installation (Windows Setup) step-by-step.
 
Enjoy Windows 8 Consumer Preview on VirutalBox!




