---
title: "Unleash The Power Of Windows 8: Learn The Mind-Blowing Tutorial On Installing Developer Preview On VirtualBox Now!"
ShowToc: true 
date: "2023-03-10"
author: "Florence Musetti"
---
*****
Title: Unleash The Power Of Windows 8: Learn The Mind-Blowing Tutorial On Installing Developer Preview On VirtualBox Now!

Introduction:
Do you want to try the newest operating system from Microsoft, Windows 8 Developer Preview, without installing it on your computer? Maybe you're hesitant to make any changes to your system, or perhaps you don't want to purchase a new computer yet. Whatever reason you have for not wanting to install it onto your computer, we have a solution for you! In this tutorial, we will walk you through the steps of installing Windows 8 Developer Preview on VirtualBox. 

Section 1: What is VirtualBox?
VirtualBox is a virtualization software that enables users to install and run multiple operating systems on the same computer. With virtualization software, you can create and run virtual machines, which are similar to standalone computers. VirtualBox is free to download and use for personal and educational purposes.

Section 2: What is Windows 8 Developer Preview?
Windows 8 Developer Preview is a pre-release version of the Windows 8 operating system. It was first released in September of 2011 and is designed for developers to test and develop apps for the Windows 8 platform. Unlike other Windows versions, Windows 8 features a more advanced graphical user interface, which makes it easier to navigate and interact with.

Section 3: Preparing for Installation
Before installing Windows 8 on VirtualBox, you need to ensure that you have the following prerequisites:

• A computer that meets the minimum hardware requirements for VirtualBox
• VirtualBox software installed on your computer
• The Windows 8 Developer Preview ISO image
• At least 2GB of RAM and 20 GB of free hard drive space

Section 4: Installing Windows 8 on VirtualBox
To install Windows 8 on VirtualBox, follow the steps below:

1. Open VirtualBox and click on the “New” button to create a new virtual machine.
2. Follow the setup wizard and enter a name for your virtual machine, select Windows 8 as the operating system, and allocate at least 2GB of RAM.
3. Click on “Create” to create your virtual machine.
4. Select your virtual machine and click on “Settings,” then navigate to “Storage.”
5. Add the Windows 8 ISO image to your virtual machine by clicking on “Add Attachment” and selecting the ISO image.
6. Click “OK” to save the settings.
7. Start the virtual machine and follow the Windows 8 installation process.

Section 5: Conclusion
In conclusion, learning how to install and run Windows 8 Developer Preview on VirtualBox is a great way to experience the latest features and improvements of this new operating system. With this tutorial, you now know how to install and set up a virtual machine to run Windows 8 Developer Preview. Enjoy exploring and understanding the potential of Windows 8!

{{< youtube wX75Z-4MEoM >}} 



If you are an early adopter and you want to install Windows 8 Developer Preview, the best way to do it is by creating a virtual machine, and you can use VMware Workstation — check this article to learn more –, you can also use VirtualBox (the one we are going to use today), which is a program from Oracle that works in the same way that VMware, or other type of virtualization software.
 
Alright, bad news first, I have been doing some testing and it appears to be that you need to have a CPU that supports hardware virtualization technology such as, VT-x/AMD-V to install this preview version of Windows. If you don’t have these settings enable, you’ll get some nasty errors and you are more than likely not to be able to run Windows 8 — but you can still try with VMware Workstation with the link I mentioned before.
 
Other than the support for hardware virtualization technology, after you crate the virtual machine, you’ll need to configure some custom settings, and you will hopefully be running Windows in not time.
 
## To install Windows 8 Developer Preview on VirtualBox follow this steps:
 
Before we start, you’ll need to download and install VirtualBox if you haven’t done so. When you done with this installation continue with the process:
 
1.  Open VirtualBox, to create a new virtual machine, click New and in the welcome wizard, click Next.
 

 
2.  In the VM Name and OS Type step: name your virtual machine with a descriptive name, and in the OS Type make sure that Operating System is on Microsoft Windows and the version to Windows 7. Then click Next.
 
3.  Set the amount of memory to at least 1024MB and click Next.
 
4.  In Virtual Hard Disk leave the default settings and click Next, a new dialog box (refer to the second image below) will appear, which will guide you in the creation of a virtual disk, select VDI (VirtualBox Disk IMage) and click Next.
 
5.  Now in Virtual disk storage details, leave the default setting Dynamically allocated and click Next.
 
6.  The next step is Virtual disk file location and size, there do just that: choose the location where to store the virtual machine and don’t forget to the name of the folder that will contain the VM. Windows 8 Developer Preview requires a minimum of 16GB of free space, so to be safe set the disk size to 20GB, then click Next.
 
7.  Then you’ll get a summary of your virtual machine in VirtualBox, click Create and Create one more time.
 
Up to here with some simple steps, you have created a new virtual machine. Next you’ll need to customize the settings in order to run the Windows 8 installation process successfully.
 
1.  Select the VM that you just created, click Settings and navigate to System.
 
2.  In System customize the settings this way:
 
Motherboard:
 
- Set Boot Order to use CD/DVD-ROM and Hard Disk
 - The Chipset should be at PIIX3
 - Extended Features should be selected

 
Processor:
 
- In Processors choose 1 or as many CPUs that is allowed
 - Extended Features Enable PAE/NX should be selected

 
Acceleration:
 
Here is where you need to pay close attention, if you CANNOT access this tab, it means that your CPU either doesn’t support hardware virtualization technology or it is disabled in which case you’ll need to get the motherboard manual and see how to enable this feature.
 
- Hardware Virtualization: Enable VT-x/AMD-V and Enable Nested Paging, both should be selected.

 
3.  Now navigate to Storage:
 
- Under IDE Controller, select Empty, and on the right, click the CD icon to browse and locate the Windows 8 Developer Preview ISO image, and click OK to finish with the settings customization.

 
4.  Next start the virtual machine and if everything went correctly to plan, you will see Windows 8 installation process.
 
After the installation is finished enjoy your Windows 8 Developer Preview on VirtualBox. 
 
That’s it!




