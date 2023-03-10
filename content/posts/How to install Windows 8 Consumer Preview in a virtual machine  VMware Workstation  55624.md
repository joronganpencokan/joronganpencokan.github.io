---
title: "Revolutionize Your Computer with Windows 8 Consumer Preview: Learn the Ultimate Installation Guide with VMware Workstation!"
ShowToc: true 
date: "2023-07-03"
author: "Gina Calogero"
---
*****
Revolutionize Your Computer with Windows 8 Consumer Preview: Learn the Ultimate Installation Guide with VMware Workstation!

Are you tired of using outdated operating systems on your computer? Do you want to experience the latest features and advancements in operating systems? Look no further than Windows 8 Consumer Preview. Windows 8 is a futuristic operating system that includes a redesigned user interface, touch screen capabilities, and improved performance. The Consumer preview version allows you to try out the latest interface and features before purchasing the final version. But before installing it, it is important to have a proper installation guide. In this guide, we will teach you how to install the Windows 8 Consumer Preview with VMware Workstation, which makes the installation process hassle-free!

VMware Workstation is a virtualization software that allows you to run multiple operating systems on one computer. This means that you can install Windows 8 Consumer Preview on a virtual machine without affecting your existing operating system. This is useful as it enables you to try out Windows 8 without worrying about it affecting your work or personal life. Let's dive into the installation process!

Step 1: Download Windows 8 Consumer Preview

The first step is to download the Windows 8 Consumer Preview ISO file. You can do this by visiting the official Microsoft website and downloading it for free. Once you have downloaded the file, make sure to save it in a location where you can easily access it.

Step 2: Install VMware Workstation

The second step is to install VMware Workstation on your computer. VMware Workstation is a paid software that you can purchase online. However, it also offers a free trial version for 30 days. You can download the trial version from the official VMware website. Once you have downloaded the software, run the installation file and follow the on-screen instructions to install VMware Workstation on your computer.

Step 3: Create a Virtual Machine

After installing VMware Workstation, it is time to create a virtual machine for Windows 8 Consumer Preview. To do this, open VMware Workstation and click on the Create a New Virtual Machine button. In the wizard, select the option to install an operating system later, as we will be using the ISO file instead. Then, select the Windows 8 Consumer Preview ISO file that you downloaded in Step 1 in the CD/DVD option.

Step 4: Configure Virtual Machine Settings

Next, you need to configure the virtual machine settings. This includes specifying the amount of RAM, hard disk space, and processor usage. VMware Workstation recommends assigning at least 2 GB of RAM and 20 GB of hard disk space to the virtual machine. Once you have configured the settings, click on the Finish button.

Step 5: Install Windows 8 Consumer Preview

Finally, it is time to install Windows 8 Consumer Preview on the virtual machine. Start the virtual machine and follow the instructions to install Windows 8. Make sure to select the custom installation option and choose the hard disk that you created in Step 4. The installation will take some time to complete, but once it is done, you will have access to the latest features of Windows 8 Consumer Preview.

Conclusion

In conclusion, Windows 8 Consumer Preview is a great operating system that can revolutionize your computer experience. By using VMware Workstation, you can try out Windows 8 without worrying about it affecting your existing operating system. Follow this installation guide to install Windows 8 Consumer Preview on a virtual machine and experience the latest features and advancements of this futuristic operating system.

{{< youtube ydGLx1Mn3u0 >}} 



Step-by-step how to install Windows 8 Consumer Preview using VMware Workstation 8.
 
So Windows 8 Consumer Preview has been released and now is ready for download. This new version of the upcoming operating system from Microsoft will give everyone a chance to get a glimpse of a more stable version. 
 
Will users who tested Windows 8 Developer Preview see major changes? Probably not, but they will notice tones of fixes and improvements under the hood and in the user interface (over 100,000 changes). The “wow!” is only to come to those users that are going to try Windows 8 for the first time.
 
But you need to keep in mind that this is an unfinished product, there still a lot of work to be done and there is a good chance that things can go wrong, so the most effective way to test Windows 8 is by creating a virtual machine (VM). Many people may have found different ways to install this version of Windows, but I wanted to share the way it worked for me.
 
## Instructions
 
Before getting our hands dirty, I tried this installation on a dual-core AMD CPU, with 4GB of RAM and with Windows 7 running as the main OS. For the virtual machine, I allocated two of the CPU’s cores and about 1.4GB of RAM. The ISO image I used was the Windows 8 32-bit version number 6.2.8250 (a.k.a build 8250).
 
If you didn’t get the Windows 8 Consumer Preview ISO image, just head over to this previous article and grab the link to download a copy of your choice — this time around Microsoft added some additional languages compare to the Developer Preview.
 
Alright, now that you have the appropriate environment to install Windows, let’s go through the creation of the actual virtual machine, we have many NEXT buttons to go through.
 
1.  Open VMware Workstation 8, go to File and select New Virtual Machine.
 

 
2.  In the welcome to the New Virtual Machine wizard, leave the defaults and click Next.
 
3.  In Guest Operating System Installation, select Installer disc image file (iso), click Browse, and locate the Windows 8 Consumer Preview ISO, then click Next.
 
4.  Select the guest operating system, in this case what you want is: Microsoft Windows and version Windows 7. Then click Next.
 
5.  You can enter the Windows product key and the Personalize Windows information now or later. For this example, I am just going to skip this step and click Next. Then name your Windows 8 virtual machine with a descriptive name, choose the storage location, and click Next.
 
6. Specify how many CPU cores you want to use for this installation (this option always is going to depend on your hardware configuration), and then click Next.
 
7. Specify the amount of RAM for the virtual machine, make it at least 1GB, and then click Next.
 
8. Choose how to connect to the network — I always use the option Use bridged networking —, then click Next.
 
9. In the following 3 steps Select I/) Controller Types, Select a Disk, and Select a Disk Type, leave the defaults and click Next.
 
10.  Specify the disk capacity, Windows 8 Consumer Preview requires a minimum of 16GB of free space for the 32-bit version, so to be safe set the disk size to 20GB, which is the minimum requirement for the 64-bit version,, select Store virtual disk as a single file, and click Next. — the final installation only used 7.9GB in my installation, this is insanely awesome!
 
11. Save the virtual machine in a new location — you may find that saving the virtual machine in another hard drive will boost performance –, and click Next.
 
12.  Now click Finish in the VMware virtual machine wizard. The new VM is created and should start.
 
If everything went accordingly, you will have a functional Windows 8 Consumer Preview installation virtual machine using VMware.
 
To finish the Windows Setup, head over: Walkthrough Windows 8 Consumer Preview installation (Windows Setup) step-by-step
 
## Other notes
 
Windows 8 Consumer Preview has just been released, remember that this is the beta version of the operating system, and there still a lot of work to be done from Microsoft and from hardware manufactures and software vendors. 
 
Be the first and let us know if you had any issues installing ‘Consumer Preview’ in the comments below or just tell us what you think about Windows 8.
 
## Useful Links
 
- How to create a Windows To Go USB drive in Windows 8 [step-by-step]





