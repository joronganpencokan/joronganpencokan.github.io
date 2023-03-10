---
title: "Unlock the Secrets to Running Windows 8 Developer Preview on Your Computer - Learn the Ultimate Guide to Installing a Virtual Machine with VMware Workstation 8!"
ShowToc: true 
date: "2023-06-08"
author: "Hazel Henson"
---
*****
Unlock the Secrets to Running Windows 8 Developer Preview on Your Computer - Learn the Ultimate Guide to Installing a Virtual Machine with VMware Workstation 8!

Are you excited about the new features in Windows 8 Developer Preview? Have you been dying to try it out on your computer, but don't want to risk damaging your current operating system? Well, fear not! There's a solution that enables you to have the best of both worlds: installing a virtual machine with VMware Workstation 8.

A virtual machine is a software emulator that allows you to run an operating system within your current one, without interfering with any of your existing files or programs. They're perfect for testing out new technology, and in this case, running Windows 8 Developer Preview. So, let's get started.

Step 1: Download VMware Workstation 8

The first step is to download a copy of VMware Workstation 8. You can download a free trial from the VMware website, or pay for the full version. Once you have it downloaded, install it on your computer.

Step 2: Create a new virtual machine

Now that VMware Workstation 8 is installed, open it up and click on 'Create a New Virtual Machine'. This will launch the New Virtual Machine Wizard. Follow the prompts, selecting the option for 'Typical', and then selecting the 'Installer disc image file' option. Browse for the Windows 8 Developer Preview ISO file that you downloaded.

Step 3: Choose your settings

You'll be prompted to select how much memory you want to allocate to the virtual machine. You can choose any amount, but it's recommended that you allocate at least 2GB. Click 'Next' and choose to create a new virtual disk. Again, you can choose any size, but it's recommended that you allocate at least 20GB. Click 'Next' again and choose the name and location for your virtual machine.

Step 4: Install Windows 8 Developer Preview

With your virtual machine created, you'll now need to install Windows 8 Developer Preview. Click 'Finish' and the installation process will begin. Follow the prompts, selecting 'Custom: Install Windows only (advanced)', and then selecting the virtual disk that you created earlier. The installation process will take a little while, but once it's done, you'll have Windows 8 Developer Preview up and running on your computer.

Step 5: Explore Windows 8 Developer Preview

Congratulations, you've now installed Windows 8 Developer Preview on your computer using VMware Workstation 8! Take some time to explore all the new features, such as the enhanced Start screen, the new App Store, and the updated File Explorer. You can even use the virtual machine to test out new programs or play games.

In conclusion, running Windows 8 Developer Preview on your computer is now easier than ever, thanks to the use of virtual machines with VMware Workstation 8. With just a few easy steps, you can be up and running in no time, exploring all the new features and functions of the latest operating system from Microsoft. So what are you waiting for? It's time to unlock the secrets of Windows 8 Developer Preview!

{{< youtube 3I64TeJ4iNI >}} 



Many users are excited with the release of Windows 8 Developers Preview, because it give us the change to get a first look of what is to come and an opportunity to get a head start to create new and unique Windows 8 applications. But you need to keep in mind that this is an unfinished product, there still a lot of work to be done and there is a good chance that things can go wrong, so the most effective way to test Windows 8 is by creating a virtual machine (VM). If you tried creating a virtual machine using VMware Workstation 7, VMware Player 3, VirtualBox, Virtual PC, or Windows 7 XP mode, chances are that you were unsuccessful to get to the Windows 8 installation process — I know because it happened to me as well.
 
After trying and trying, I was able to get my Windows 8 Developer Preview running. Many users may have found different ways to install this version of Windows, but I wanted to share the way it worked for me.
 
## To create a Windows 8 virtual machine on VMware follow these steps:
 
Before we start, I tried this installation process using just a regular laptop with a dual-core Intel CPU, which is also running Windows 7. And the image I used was the Windows 8 32-bit version 6.2.8102 a.k.a build 8102.
 
If you didn’t get the Windows 8 Developer Preview ISO image, just head over to this previous article and grab links to download a copy of your choice.
 
If you have tried VMware Workstation 7, you may have noticed that you get the new Blue Screen of Death (BSOB) — which now includes a sad smiling face –. So what do you do now? Well, what you need is to download and install VMware Workstation 8, keep in mind that you previous version of VMware Workstation will be uninstalled in order to install this new version. 
 

 
Alright, now that you have the appropriate environment to install Windows, let’s go through the creation of the actual virtual machine.
 
1.  Open VMware Workstation 8, go to File and select New Virtual Machine.
 
2.  In the welcome to the New Virtual Machine wizard, leave the defaults and click Next.
 
3.  In Guest Operating System Installation, select I will install the operating system later and click Next.
 
4.  Select the guest operating system, in this case what you want is: Microsoft Windows and version Windows 7. Then click Next.
 
5.  Name your Windows 8 virtual machine with a descriptive name, choose the storage location, and click Next.
 
6.  Specify the disk capacity, Windows 8 requires a minimum of 16GB of free space in disk, so to make it safe enter 20GB, select Store virtual disk as a single file, and click Next.
 
7.  Now click Finish in the VMware virtual machine wizard.
 
8.  This is the step where we make the magic happens and where many people seem to be having a little bit of problem using VMware Workstation. Click on Power on this virtual machine and if you come across any dialog box, just click OK.
 
9.  When the VMware virtual machine is running, go to VM (in the file menu), and navigate through Removable Devices, CD/DVD (IDE), and click Settings.
 
There tick Use ISO image file, click Browse and locate the Windows 8 Developer Preview ISO image file, and click OK.
 
If you don’t do this you are going to end up with: Windows cannot read the product key setting from the unattend answer file. message like in the image below.
 
10. Finally, click the Reset button.
 
If everything went accordingly you will have a functional Windows 8 Developer Preview virtual machine using VMware.
 
## Sept. 20, 2011 Update
 
### Other notes:
 
Windows 8 Developer Preview was only released several days ago, and there still a lot of work to be done from Microsoft itself, and from hardware manufactures and software vendors. At this stage there are many virtualization solutions on the market that do not support this new version of Windows and they need to be updated.
 
People around the web are being successful installing it with some products and others are failing. As you read in this article we are successful using VMware Workstation 8 for Windows, so here are other virtualization products that are known to be working:
 
- VirtualBox 4.1.2 for Windows
 - Hyper-V in Windows 8 Developer Preview
 - Hyper-V in Windows Server 2008 R2

 
These products will not work:
 
- VMWare Workstation 7.x or older
 - Windows 7 XP Mode
 - Microsoft Virtual PC (all versions)
 - Microsoft Virtual Server (all versions)

 
## Useful Links
 
- How to create a Windows To Go USB drive in Windows 8 [step-by-step]





