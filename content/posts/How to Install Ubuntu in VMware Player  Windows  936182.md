---
title: "Unlock the Secrets of Installing Ubuntu on Windows! Learn the Easiest Way with VMware Player Now!"
ShowToc: true 
date: "2022-11-29"
author: "James Haverstock"
---
*****
Title: Unlock the Secrets of Installing Ubuntu on Windows! Learn the Easiest Way with VMware Player Now!

Introduction:

Have you ever felt curious about using Linux on your Windows PC but are afraid to take the plunge and install it as a dual-boot or run it on a virtual machine? Fear not! With VMware Player, you can easily run Ubuntu on your Windows PC without affecting your existing operating system.

In this article, we will go through the step-by-step process of installing Ubuntu on Windows using VMware Player. So, let's get started and unlock the secrets of using Ubuntu on your Windows PC!

Step 1: Download and Install VMware Player

The first step is to download and install VMware Player on your Windows PC. You can do this by visiting the VMware website and downloading the latest version of VMware Player.

Once the download is complete, run the installer and follow the on-screen instructions to install VMware Player on your computer.

Step 2: Download an ISO file of Ubuntu

After installing VMware Player, the next step is to download an ISO file of Ubuntu. You can do this by visiting the official website of Ubuntu and downloading the ISO file of the latest version of Ubuntu.

Step 3: Create a New Virtual Machine

To create a new virtual machine in VMware Player, click on the "Create a New Virtual Machine" option. In the wizard, you will be asked to select the ISO file of Ubuntu that you downloaded in Step 2.

Once you have selected the ISO file, follow the instructions to create a new virtual machine. You will be asked to allocate a certain amount of memory and hard disk space for the virtual machine.

Step 4: Install Ubuntu on the Virtual Machine

After creating the virtual machine, it's time to install Ubuntu on it. To do this, select the virtual machine and click on the "Play virtual machine" option.

This will start the Ubuntu installation process. Follow the on-screen instructions to install Ubuntu on the virtual machine. You will be asked to select the language, time zone, keyboard layout, and create a user account.

After the installation is complete, Ubuntu will be ready to use on your Windows PC!

Conclusion:

With VMware Player, installing Ubuntu on Windows is easy and straightforward. By following the step-by-step process outlined in this article, you can easily unlock the secrets of using Linux on your Windows PC.

So, what are you waiting for? Download VMware Player today and start using Ubuntu on your Windows PC!

{{< youtube wX75Z-4MEoM >}} 



So you have been following the Linux community for a while and wanted to install a Linux based OS like Ubuntu while having the known surroundings and convenience of Windows. There are lots of ways to test Ubuntu without making permanent changes to your computer. Running Ubuntu from USB or CD/DVD drives is one of the ways. Here we are showing you another way to test Ubuntu via VMWare Player.
 
We have previously shown you how to install Ubuntu in a Virtualbox. VMWare Player is another virtualization software that allows you to run a virtualized OS in your current system.
 
Note: This tutorial shows you how to install Ubuntu, but it will work for most Linux distro as well.
 
## Things You Need To Download
 
- Download VMware Player (free) – Once you have downloaded the software, just install it like any other software.
 - Ubuntu ISO – download it from Ubuntu’s official website. Personally, I recommend you to download the 32-bit version of Ubuntu unless you have tons of memory to spare. I really stress this because the 32-bit version of Ubuntu tends to run more smoothly on less memory (less than 2 GB) which is ideal for virtual machine.

 
## Install Ubuntu In VMware Player
 
1. Once you have downloaded VMware Player, install it in your Windows machine. Launch it via the desktop shortcut or by going to the Start menu. To create a new virtual machine, click on “Create a New Virtual Machine” link.
 

 
2. The above action will open virtual machine wizard. Select the radio button “Installer disc image file (iso)” and click on the “Browse” button and point it to the Ubuntu ISO file. As you can see from the below image, VMware automatically detects the OS and makes all the arrangements for easy installation. Click the “Next” button to continue.
 
3. In the next screen, fill in all the details like your full name, user name and a good password. After filling in all the necessary data, click the “Next” button to continue.
 
4. Now you have to name your Ubuntu virtual machine. As you can see, I have named it “UbuntuMTE” and I’ve also changed the default location to a folder named “UbuntuMTE” in G drive because most of us won’t have enough space to spare in our C drive (OS installation drive). Of course, there is no need for you to change the default location if you have enough space.
 
5. Here in this screen just leave the settings to default, e.g., “20 gigs” of virtual hard disk space and “split virtual disk into multiple files.” The default installation of Ubuntu takes around 4.5GB to 5GB, and the remaining free space can be used to install software, upgrades, etc. Click the “Next” button to continue.
 
6. This is the best part of VMware because it will automatically adjust all the required hardware specs. If you want to customize things like the amount of RAM (memory) you want to dedicate or number of processor cores you want to use, just click on the “Customize Hardware” button to customize a whole bunch of virtual hardware settings.
 
7. When you click the “customize hardware” button, it will open a window where you can tweak different hardware specs like…
 
- RAM (Memory) – The amount of memory you want to dedicate to the virtual machine. As you can see, 1GB of RAM is enough for Ubuntu 32-bit version.
 - Processors – Here you can select how many processor cores you want to dedicate to the virtual machine. That said, the default setting is just good and don’t touch it unless you know what you are doing.
 - CD/DVD – Here you can select a different ISO or you can even point it to your physical CD/DVD drive. Of course, we’ve already pointed it to use Ubuntu ISO that we just downloaded, so there is no need for any changes.
 - NAT – Here you can change the networking settings of your virtual machine. By default VMware uses NAT (Network Address Translation) but if you want to change your network connection to Bridged or Host-Only, this is the place to do so.
 - USB Controller – Here you can change the USB compatibility mode from 2.0 to 3.0 or vice-versa. You can even customize stuff like whether you want to connect new USB drives automatically or to share your Bluetooth device (if you have one on your physical machine) with the virtual machine, etc.
 - Sound Card – By default, VMware uses your default host sound card, but if you want to change it to another sound card, then you can change those settings here.
 - Printer – If you have a printer connected to your physical machine, VMware can use it to print out your stuff.
 - Display – By default, VMware uses host display settings. But you can change those display settings according to your needs under this section.

 
Note: If you are trying to install Ubuntu 64-bit version, I would recommend you dedicate at least 2GB RAM, otherwise you may not get a good smooth experience.
 
8. Once you have finished configuring all the virtual hardware specs, make sure the check box “Power on this virtual machine after creation” is checked and click the “Finish” button to start installing Ubuntu in VMware player.
 
9. As you can see from the below image, VMware automatically installs the Ubuntu OS. The installation will take a while, so just sit back and relax while VMware does the work for you.
 
Once the installation is complete, your virtual machine will be rebooted automatically and you will be greeted with a gorgeous Ubuntu login screen.
 
Enter your account password (the one you used in step #3) and hit the Enter button to start using and testing Ubuntu.
 
So, last but not least – Welcome to Ubuntu desktop. Hope that helps and do comment below if you face any problems while installing Ubuntu in VMware player.
 
Vamsi is a tech and WordPress geek who enjoys writing how-to guides and messing with his computer and software in general. When not writing for MTE, he writes for he shares tips, tricks, and lifehacks on his own blog Stugon.
 
Our latest tutorials delivered straight to your inbox




