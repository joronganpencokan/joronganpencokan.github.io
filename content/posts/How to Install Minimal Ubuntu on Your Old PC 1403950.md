---
title: "Revive Your Old PC with This Secret Hack to Install Minimal Ubuntu - No Tech Skills Required!"
ShowToc: true 
date: "2023-04-27"
author: "John Raby"
---
*****
Revive Your Old PC with This Secret Hack to Install Minimal Ubuntu - No Tech Skills Required!

If you have an old computer that's just gathering dust in a corner, it's time to give it a new lease of life. Installing Ubuntu, one of the most popular Linux operating systems, is a great way to revive your old PC. But if you're worried about your tech skills not being up to par, worry not! Follow this secret hack and install the minimal version of Ubuntu on your old computer without any technical know-how.

Step 1: Download Ubuntu Minimal

The first step is to download the minimal version of Ubuntu. This version of Ubuntu is a stripped-down version of the original, which means it requires less power to operate. This will make it ideal for lighter and older hardware.

Visit the official Ubuntu site, and download the minimal version of Ubuntu. While you're there, ensure that you pick the right version that's compatible with the specifications of your old PC.

Step 2: Create a Bootable USB Drive

After downloading the Ubuntu Minimal image, the next thing is to create a bootable USB drive. This step is crucial, as you'll need to run Ubuntu from this USB drive during the installation process.

To create a bootable USB drive, you can use Rufus, a free and easy-to-use program, or any other similar software. Insert your USB drive, open Rufus, select the Ubuntu Minimal image, and let the program do its job.

Step 3: Boot From The USB Drive

Once you have the bootable USB drive, the next step is to boot the Ubuntu installation from the USB drive. You can do this by restarting your old PC and entering the BIOS settings (usually by pressing F2, F12, or Del while your computer boots).

Once you're in the BIOS settings, navigate to the boot order settings, and make sure that your USB drive is at the top of the list. Save your changes and reboot your PC with the USB drive still attached.

Step 4: Install Ubuntu Minimal

The Ubuntu Minimal installation process is straightforward and user-friendly. Follow the prompts as they appear, and you'll have a minimal installation of one of the best Linux operating systems. During the setup, remember to select the minimal installation option.

The installation process might take some time, depending on the specifications of your old PC, but once it's done, you'll have a functional operating system that's lightweight and capable of running on older hardware.

Conclusion

Reviving your old PC is easy and cheap with this simple Ubuntu hack. Ubuntu Minimal is an excellent choice for anyone looking to restore an older computer to usefulness. With this guide, you can easily install Ubuntu Minimal in no time, even if you have little to no technical know-how. So don't let your older computer gather dust, breathe new life into it with Ubuntu Minimal!

{{< youtube 21TFcUIPlS0 >}} 



What happens when an older PC with limited hardware is unsupported by Windows and can’t be upgraded? Users can turn to Linux for help, and in this case Ubuntu.
 
Ubuntu is a free open-source operating system that enables users to either break away from using Windows completely or have the option of dual booting to give more choice. It is easy to install, quick and will make your old PC more secure. In this tutorial we will show you how to install a minimal and lightweight version of Ubuntu on your old PC.
 
Tip: Did you know that installing Linux could increase your laptop battery life?
 
## Getting the ISO File
 
First, you will need to obtain a copy of the Ubuntu minimal ISO image file. This can be found by going to the Ubuntu website and selecting the appropriate image.
 

 
If you are using an older PC, then chances are you might need the 32-bit PC (i386, x86) image file. These are generally PCs that have less than 4GB of RAM and a much slower, older processor. They are also likely to work on slightly newer systems, as 64-bit processors can run 32-bit systems.
 
Click on your chosen image and save it to somewhere convenient, such as the Downloads or Desktop folder. Note the small size – this is because the ISO file is just the bare bones of what Ubuntu needs to boot. It will pull all the information and packages from the Ubuntu repositories as it installs.
 
Note: there are two versions of the Ubuntu install media. The minimal one, as shown above, and the full installer that can be obtained from the Ubuntu website.
 
The main difference is that while you can perform a minimal install within the “full version” of Ubuntu, some older hardware may not be able to display the full graphical installer. Therefore, depending on your machine specifications, it is better to select this minimal installer as it is more likely to work on all machines.
 
## Verify the Downloaded ISO File (Optional)
 
As an optional step, you can verify the ISO file to ensure its integrity against the MD5SUM. An MD5SUM is a calculation (hash value) of the ISO file to ensure no files have been changed or altered. Details of how to check this can be found at the Ubuntu help pages.
 
## 2. Creating live media
 
Once you have the image saved, you will need to burn it onto either a CD or USB stick. Depending on how old the machine is, and if it has a CD/DVD drive, will determine which of these is better-suited to your hardware. Generally, all machines should be able to boot from the CD drive, whereas some older BIOS will not have the USB boot capability.
 
Ubuntu has provided a useful guide on burning the image to a CD on a variety of systems and also creating USB media. For creating a bootable USB drive, we highly recommend Etcher, as it is easy to use and cross-platform compatible.
 
## Installation of Minimal Ubuntu
 
With everything verified and your media created, you are now ready to install. Insert your CD or USB stick into the PC and switch it on. You may need to press F12 or F10 or F2 to access your BIOS menu to enable booting from your newly created media. (Please check with your manufacturer on how to do this.)
 
Once it boots up, you will be presented with the following menu screen.
 
Press Enter to start the install.
 
You will encounter a number of screens as Ubuntu guides you through the setup. Below are some of the screenshots to set Language, Keyboard, Hostname and Mirror. Take your time and read the instructions carefully. If you make a mistake, you can always use the Tab button and select “Go Back” to correct the problem.
 
Once you have selected the local mirror, which will make the download faster, Ubuntu will proceed to call all the packages and elements it needs to install itself on your PC. This may take a while depending on your connection, but just be patient.
 
With the download completed, you’ll be asked to set up a username and password.
 
You can pick anything you like as long as it is memorable. As an illustration, I picked the distro name which is “ubuntu.”
 
Choose a password – for this demo I selected “root.” For your own system, pick something strong and not easily guessed. The system will flag a password if it considers it weak as shown:
 
After this the system will set up the clock and time zone.
 
The system will then ask you to select how you want to partition your disk. If you want to use encryption, select the third option to allow guided setup. I would personally advocate encryption as a matter of course to keep your data secure, but the choice is yours. The installer will then run through some additional options, such as setting up passphrases for your encrypted disk.
 
If you have elected to not use encryption, you will immediately arrive at the following screenshot.
 
The system will select the amount of space automatically; however, you can follow the hint and use the word “max” to specify the maximum size available. There will be one last check of the partitioning you have selected, and then the system will start installing.
 
Just as with downloading the packages from the mirror, the install may take some time. Be patient.
 
Eventually the system will finish and ask you if you want to install updates automatically, so select the option that works for you.
 
The next screen will ask you to select what packages you want to install. Most people will want to select “Ubuntu desktop,” as this will give you the base desktop for you to fully boot into Ubuntu. In this case, Ubuntu desktop refers to GNOME 3 Desktop Manager, which is similar to the desktop in the full version. If you want a lighter weight version of Ubuntu, you can select “Lubuntu desktop” or “Ubuntu Mate.”
 
Finally, the system will ask to set up GRUB, which is the bootloader. GRUB stands for Grand Unified Bootloader. It is the small program that enables the kernel to load, which in turn starts the system loading.
 
Congratulations, your Ubuntu system is installed and ready to boot.
 
Image credit: A System76 laptop displays the Ubuntu Edgy login screen.
 
Matt has worked in the tech industry for many years and is now a freelance writer. His experience is within Windows, Linux, Privacy and Android.
 
Our latest tutorials delivered straight to your inbox




