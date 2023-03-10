---
title: "Breaking News: The Ultimate Guide To Installing Windows In Virtualbox On Linux REVEALED! You Won't Believe How Easy It Is!"
ShowToc: true 
date: "2023-01-08"
author: "Andrea Spears"
---
*****
# Breaking News: The Ultimate Guide To Installing Windows In Virtualbox On Linux REVEALED! You Won't Believe How Easy It Is!

Are you tired of using only Linux on your computer? Do you want to try out Windows for some specific task but don't want to dual boot and risk messing up your system? Do you need to test applications in Windows without having to purchase a separate computer? If you answered yes to any of these questions, then this article is for you!

Virtualization has become increasingly popular over the years, as it allows individuals to run multiple operating systems on a single computer without affecting the host operating system. One of the most popular virtualization software is Virtualbox, which is available for free on Linux.

In this ultimate guide, we will walk you through the step-by-step process of installing Windows on Virtualbox on your Linux computer. You won't believe how easy it is!

**Step 1: Install Virtualbox**

The first step is to install Virtualbox on your Linux computer. You can download the latest version of Virtualbox from the official website or from your distribution's software repository.

**Step 2: Download Windows ISO**

The next step is to download a Windows ISO file. You can download a legal and free copy of Windows 10 from Microsoft's website. Make sure to choose the correct version and language for your needs.

**Step 3: Create a New Virtual Machine**

Open Virtualbox and click on "New" to create a new virtual machine. Give it a name and choose "Microsoft Windows" as the type and the version you downloaded.

**Step 4: Allocate Memory and Storage**

Allocate the amount of memory you want to allocate to the virtual machine. Keep in mind that you need a minimum of 2GB of RAM for Windows 10. Next, create a virtual hard disk file, either dynamically allocated or fixed size.

**Step 5: Configure Settings**

We need to tweak the virtual machine settings to ensure a smooth experience. In the "System" tab, enable "Enable EFI (special OSes only)" and select "Chipset" as "ICH9". In the "Display" tab, enable "3D Acceleration" and set "Video Memory" to 128MB.

**Step 6: Install Windows**

Now it's time to install Windows on the virtual machine. Click on "Start" and select the Windows ISO you downloaded. Follow the installation process just like you would on a physical computer.

**Step 7: Install Virtualbox Guest Additions**

Once Windows is installed, you may notice that the graphics are not up to par. You can install Virtualbox Guest Additions to enable features like full-screen mode, better graphics, and shared folders. To do this, click on "Devices" and select "Insert Guest Additions CD image". Follow the prompts to install the software.

Voila! You now have a fully functioning Windows installation running on your Linux computer. You can use Windows applications and test software without having to switch between two computers or affecting your host operating system.

In conclusion, Virtualbox is a great tool to have on your Linux computer, especially if you want to experiment with different operating systems without the risk of messing up your computer. Follow these simple steps, and you'll be on your way to successfully installing Windows on Virtualbox in no time!

{{< youtube OWmD8obq4eQ >}} 



There are several reasons why a Linux user would want to create a Windows virtual machine, and VirtualBox is easily one of the most popular hypervisors available for Linux. It’s simple to use, easily accessible, and extremely flexible in what it allows you to do with your virtual machines. In this guide, you’ll learn how to install Windows in VirtualBox in Linux.
 
## Installing VirtualBox
 
There are two primary ways to install VirtualBox in Linux. The first one is to go to the website and download whichever package works for your system. To do this, first go to the project website and click the big “Download VirtualBox 6.1” button.
 
After that, click “Linux distributions” on the Downloads page.
 
You’ll be brought to a list of compatible Linux distros on which you can install VirtualBox. Click whichever one you’re looking for, follow the download prompts, and the package installer should automatically install the package. 
 
However, there are some challenges with that. Generally, just installing the RPM or DEB will miss building the kernel modules necessary, which can bring up many errors. The way to get around that is to install VirtualBox from your distro’s repository. This is usually a simple command to install, depending on your distribution. 
 
For Ubuntu and its derivatives: 
 
## Downloading Windows 10
 
For those who may not be aware, Windows 10 is actually free to download and use. You can’t use it in a production environment without paying for it, but if it’s purely for personal purposes, it’s fair game. 
 
To download the ISO image file, go to this link and scroll down to where it says “Select edition.” Choose whichever is the latest edition and click “Confirm.” Choose your product language and click “Confirm” again. You’ll be brought to a page where you can choose between 64-bit and 32-bit downloads. I’d recommend 64-bit, as it’ll give you the most flexibility in terms of the actual virtual machine you create. 
 
Note: the download may take a while, especially on a slow network connection, as the ISO image is almost 5GB in size.
 
Once you click “64-bit Download” and save it to your machine, you’re ready to create your Windows 10 virtual machine in VirtualBox. 
 
## Creating the Windows 10 Virtual Machine
 
Once your download is finished, open up VirtualBox and click “New.” 
 
Type “Windows 10” in the “Name” section. That will automatically choose the “Version” to “Windows 10 (64-bit).” From there, name it anything you want. 
 
Go through the menu and set whatever you’d like for the configuration of the virtual machine. I’d recommend at least 4096MB Memory and creating a 75GB virtual disk. Don’t worry about it eating up all of your disk space; you can choose “Dynamically allocated” to save disk space. The type of disk doesn’t matter too much either, unless you plan to move this VM around from system to system. 
 
Once you finish creating your virtual machine, you’ll be left with a plain VM that needs some help to be configured. Depending on the specs of your host machine, you may be able to do more than this, but here’s what I would recommend as the minimum. 
 
You’ll want at least:
 
- 2 vCPUs
 - 3D acceleration turned on
 - Hyper-V for the paravirtualization interface

 
If you have more CPU cores or RAM to allocate, I’d absolutely recommend doing so. This will only get you so far. 
 
Additionally, you’ll have to attach the Windows 10 ISO file that you downloaded earlier. On the VM Settings page, click “Storage -> Optical Drive -> Empty” in the Storage section and click “Choose a disk file.” Navigate to your downloads folder and choose your Windows 10 ISO file.
 
Now, all you have to do is start up your virtual machine by clicking “Start” at the top and install Windows.
 
Once Windows is installed, you may notice that it’s complaining about inadequate video drivers and that you’re limited to a very small screen. To fix all that, you will need to install VirtualBox Guest Additions. 
 
## Installing VirtualBox Guest Additions in Windows 
 
Installing Guest Additions is quite simple. With the VM running, click “Devices -> Insert Guest Additions CDimage” and then “Insert.” Open the file explorer and click on “This PC.” You should see the icon for the Guest Additions CD Image on the bottom next to “Local Disk (C:).” Click on the Guest Additions CD Image icon. 
 
Click on “VBoxWindowsAdditions” and “Yes” on the UAC dialogue.
 
Click “Next” through the installer dialogue, accepting all defaults. Additionally, click “Install” when you get the dialogue asking to trust software from Oracle. 
 
Once the installation is finished, click “Finish,” and your VM will reboot. Once it reboots, the Guest Additions are installed, and you can now experience true 3D acceleration, screen size selection, and many of the other great benefits that come with using VirtualBox Guest Additions, like shared clipboards and file sharing from Host to Guest and back. 
 
Now that you know how to install Windows in VirtualBox, make sure to check out some of our other Linux virtualization articles, including this one about Virtual Machine Manager, and this one about creating a Linux virtualization workstation.
 
John is a young technical professional with a passion for educating users on the best ways to use their technology. He holds technical certifications covering topics ranging from computer hardware to cybersecurity to Linux system administration.
 
Our latest tutorials delivered straight to your inbox




