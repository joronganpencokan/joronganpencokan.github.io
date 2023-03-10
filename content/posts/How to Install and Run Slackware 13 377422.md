---
title: "Unlock the Secrets of Slackware 13 Installation in Just a Few Steps! You Won't Believe How Easy It Is!"
ShowToc: true 
date: "2022-11-11"
author: "Timothy Brevig"
---
*****
+ Title: Unlock the Secrets of Slackware 13 Installation in Just a Few Steps! You Won't Believe How Easy It Is!

Introduction:
Slackware is a Linux-based operating system that is popular among technical enthusiasts and Linux veterans. It is famously known for its simplicity and stability, which is why it has a loyal fan base- It's said that once you start using Slackware, you won't look back! Slackware has been around for over 25 years and has established itself as a reliable and efficient operating system. If you're new to Slackware or Linux, you may feel intimidated by the installation process. But fear not, as we will show you a simple guide to install it.

Step 1: Download Slackware 13
The first step to installing any operating system is to download the installation image file. Visit the Slackware Download page and choose the appropriate version. Slackware 13 has three types of ISO images: full DVD, CD, and the minimal ISO. Choose the one that fits your needs and click on the appropriate link to begin the download.

Step 2: Burn Slackware to a CD or USB
Once the download is complete, you will have to burn the ISO image onto a CD or USB stick. You can use software like Rufus, Etcher, or BalenaEtcher to burn the ISO image to a USB stick or DVD. You can also use the command line to create a bootable USB stick.

Step 3: Boot from the CD or USB
Before you can install Slackware, you need to boot your computer from either the CD or USB flash disk you created. Insert your CD or USB boot drive into your computer's disc drive or USB port, and follow the instructions on the screen to boot your computer from it.

Step 4: Installation process
After booting up the Slackware installation media, you'll be presented with the installation menu. The installation menu lets you choose which components you want to install, such as the kernel, packages, and applications. Slackware's installation process is text-based, but it's very easy to follow.

The first few screens of the installation process will ask you to choose your keyboard and language preferences. Next, you will be prompted to set up your network connection, such as eth0 or wlan0. Once the network connection is established, you can proceed with the installation.

You can choose to install a full system or use the “expert” option to select only the specific packages that you require for your needs. The expert method lets you customize your Slackware installation to your liking.

Step 5: Set up the bootloader
Once the installation process is complete, you will be asked to set up your bootloader. The bootloader is responsible for loading Slackware when your computer boots up. You can choose to install either GRUB or LILO, which are the two most popular bootloaders used in Linux.

Final thoughts:
Slackware's installation process is relatively straightforward and easy to follow, even for beginners. This guide covers the essential steps of installing Slackware 13 on your computer, including burning the image to a CD or USB flash drive, booting from the installation media, and configuring your bootloader. With these few steps, you can enjoy the stability, reliability, and simplicity of Slackware 13.

{{< youtube L_T-HBQH2tI >}} 



A former co-worker once told me “If you want to learn Debian, install Debian.  If you want to learn Fedora, install Fedora. If you want to learn Linux, install Slackware.”  The philosophy behind Slackware is to keep the system as UNIX-like as possible. There’s not a lot of automatic configuration and you won’t find many bells and whistles, but you’d be hard set to find a more stable and mature distribution. In fact, Slackware is one of the few distros still in existence from Linux’s early days, right along with Debian, SuSE, and Red Hat. Because of this decision to keep things as UNIX-like as possible, Slackware has a reputation for being somewhat difficult to install and confusing to use. While this has been true for a long time, there have been some great improvements in the past few releases, and now seems like a great time to run a guide on this often misunderstood distribution.

 
### Getting Slackware
 
Torrent downloads for Slackware 13 can be found here. I’ll be using the full DVD ISO for this article as it includes all the packages necessary for a typical install.
 
### Booting the Installer
 
After burning the ISO to DVD and rebooting, you’ll be taken to the initial boot screen, pick a keymap, and log in.
 

 
### Setting up Disks
 
Chances are, before you can begin the install, you’ll need to set up some partitions. The Slackware Install DVD provides fdisk (purely text-based) and cfdisk (semi-graphical interface) to do the job. In general I’d recommend cfdisk, as I think it’s easier to navigate.
 
If you’re unsure how to set up the partitions, check out A Quick Guide to Linux Partition Schemes.
 
Once you’re finished with your partitioning, make sure you write the changes to disk and exit the partitioner. You’ll be taken back to the command line, and we can begin the install. Slackware has an installer built into the install DVD, which you can launch by typing
 
As long as the partitioning has been done correctly, you’ll be taken to the opening screen of the installer.
 
The first thing we’ll do is set the target partition. This will be whichever partition you created in fdisk or cfdisk that you intend to be root (/). In my example screenshots above, it would be /dev/hda1. Next you’ll choose your filesystem. There’s no right or wrong choice here, there are pros and cons to most of the filesystem options. If unsure, ext4 is a good choice.
 
### Installing the System
 
When asked to choose the installation source, pick Install from Slackware CD or DVD and let it scan for the drive. You’ll then be taken to the first package installation screen.
 
If you’re looking to save on space, some of those can be removed without negatively affecting your installation. Deselecting KDE, for example, would greatly reduce disk space needed.
 
The next step is choosing just how much detail you want to go into when choosing packages. The Full option will install everything, minus the items you deselected in the previous step and is by far the simplest option.  Menu and Expert give a good balance between ease and flexibility, allowing you to choose from groups of packages. If you choose one of those options, you’ll be given several screens, one group per screen. Choose this option only if you’re very familiar with what is and isn’t essential your system. We’ll be proceeding using the Full option.
 
Once you’ve chosen your packages, installation will truly begin. Chances are this will take a while. A long while. A nice feature of the Slackware installer is that it gives descriptions of each package as it installs.  You can learn quite a bit by simply watching the packages install and reading what they do.
 
### Installing the Boot Loader
 
Once the file copy is complete, you’ll be asked if you want to make a USB recovery key. Take your pick from the suggestions provided and you’ll be brought to the boot loader screen. The somewhat odd thing about this is that Slackware uses the lilo boot loader instead of GRUB. According to their website:
 
Our example partitions are quite simple so we’ll proceed with the automatic.
 
Reminder: Installing any boot loader overwrite whatever boot loader may already be in place.
 
Once you choose the screen resolution for startup and some other minor prompts, you’ll be taken to the screen asking where exactly lilo should be installed. If Slackware is the only operating system on this computer, it should be perfectly ok to install at the default location, the MBR. If you intend to use lilo with other operating systems or without overwriting the MBR, see a more detailed guide such as this.
 
After that you choose mouse type (default should be fine) and whether or not to include gpm (recommended).
 
### Network Config
 
Network configuration in most situations can be left automatic with DHCP. You’d probably know if you needed a special IP or anything. Hostname can be whatever you like, “slackware” is a good standby. When it comes to domain name, unless you have a specific reason, there’s no need to worry about whether or not it’s a “real” domain name, you can put in anything, like mynetwork.rox.
 
### Final Setup
 
At the Startup Services screen, you can choose… well… startup services. The defaults are all good choices but there are some you may wish to enable or disable, such as CUPS printing or SSH.
 
Next up is one of the nice little additions that made Slackware a little more endearing to me, a menu to test and set console fonts. Not much utility but a nice touch.
 
When you’ve finished picking a font and entering time settings, you’ll get to choose which of the desktop environments you’d like to run.
 
Once you set a new root password, you’re ready to reboot into your new Slackware system. Don’t forget to create a new user once you’ve rebooted so you won’t be running as root. Your desktop environment can be started from the console with the command
 
### Installing New Software
 
Even if you installed the full 4GB system, there will eventually be some things you want that Slackware doesn’t have preinstalled. This is where a lot of people give up on Slackware, because unlike most other modern Linux distributions, it has no automated online package manager with dependency resolution and such. That means nothing like apt-get or yum or other such tools by default.  This can make package management and upgrades a much more tedious process. There is an alternative, however, to get that functionality. To cover all the bases, here are the three main methods for software installation in Slackware:
 
Method 1: Slackware Packages
This is how it’s “supposed” to be done. Some software developers make Slackware packages (in .tgz format) available for download, and others can be found on sites such as LinuxPackages.net. Once downloaded, you just open a terminal and enter
 
Update – MTE readers have suggested SlackBuilds.org and Slacky.eu as better places to find Slackware packages and build scripts.  
 
Method 2: Compile From Source
As with all Linux, you almost always have the option of compiling programs directly from the source code.  If you need a refresher on that, check out How to Install Software from a Tarball in Linux.
 
Method 3: Slapt-get
As the name implies, slapt-get is an apt-like tool for Slackware. It can be used to install, remove, and upgrade packages.  The output is nearly identical to apt-get in many places so it should be familiar to most Debian/Ubuntu users.
 
Unlike apt-get, slapt-get parameters start with double dashes (–).  Some common ones include:
 
- –update  Refresh lists of packages
 - –upgrade  Perform system upgrade
 - –install  Install a specific package
 - –remove Remove a package
 - –search Find keyword in package lists

 
That should be enough to get you started. If you run into any trouble, check out the Revised Slackware Book Project. Happy Slacking!
 
Josh Price is a senior MakeTechEasier writer and owner of Rain Dog Software
 
Our latest tutorials delivered straight to your inbox




