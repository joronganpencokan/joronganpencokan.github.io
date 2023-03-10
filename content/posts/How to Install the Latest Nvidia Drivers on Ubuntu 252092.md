---
title: "You won't believe how easy it is to install the latest Nvidia drivers on Ubuntu!"
ShowToc: true 
date: "2023-06-06"
author: "Shawn Gilson"
---
*****
# You Won't Believe How Easy it is to Install the Latest Nvidia Drivers on Ubuntu!

Are you tired of struggling with outdated Nvidia drivers on your Ubuntu system? Don't worry, you're not alone. Many Ubuntu users find it challenging to keep their graphics card drivers up to date. But the latest release of Nvidia drivers has made the installation process quick and straightforward, even for beginners!

In this article, we'll take you through the step-by-step process of how to install the latest Nvidia drivers on Ubuntu. Let's dive in!

## Step 1: Determine Your Graphics Card

Before installing the latest Nvidia drivers, you need to determine which graphics card you have in your system. To do this, open your terminal and type the following command:

```
lspci -nn | grep -E 'VGA|Display'
```

This command will list all the detected graphics cards in your system.

## Step 2: Add the Proprietary GPU Drivers PPA

The next step is to add the Proprietary GPU Drivers PPA to your system. This PPA provides the latest Nvidia graphics drivers. To add the PPA, enter the following commands in your terminal:

```
sudo add-apt-repository ppa:graphics-drivers/ppa
sudo apt update
```

## Step 3: Install the Latest Nvidia Drivers

After adding the PPA, you can now install the latest Nvidia drivers using the apt-get command. To install the latest Nvidia drivers, type the following command in your terminal:

```
sudo apt-get install nvidia-driver-450
```

This command will install the latest Nvidia drivers on your system.

## Step 4: Reboot Your System

After installing the Nvidia drivers, you need to reboot your system to activate the new drivers. To reboot your system, type the following command in your terminal:

```
sudo reboot
```

## Step 5: Verify the Installation

After rebooting your system, you can verify the installation of the Nvidia drivers using the following command:

```
nvidia-smi
```

If the Nvidia System Management Interface displays your graphics card's details, congratulations! You've successfully installed the latest Nvidia drivers on your Ubuntu system.

## Conclusion

Installing the latest Nvidia drivers on Ubuntu can be a challenging task, but it doesn't have to be. With the latest Nvidia drivers, the process has become more straightforward than ever before. By following the above steps, you can enjoy the latest Nvidia features on your Ubuntu system.

So, what are you waiting for? Give it a try and say goodbye to outdated graphics drivers on your Ubuntu system!

{{< youtube VP-R7LNSJXA >}} 



If you have an Nvidia video card you’re in luck. They perform exceptionally well on the Linux platform. However, most Linux-based operating systems come with the open-source driver preinstalled. The performance is poor, and 3D capabilities are usually non-existent. To get the most out of your video card, you need to install Nvidia’s proprietary driver.
 
## Install Recommended Nvidia Driver
 
This will install a fairly recent driver, but not the absolute latest. If you want bleeding edge software, skip to the next section.
 
The advantages of following the procedure in this section are:
 
- Older video cards (4+ years) may not work with the latest driver. The utility will automatically find and recommend an older driver (if necessary) that still works with your card.
 - These drivers are tested more and have fewer bugs than bleeding edge drivers.
 - It’s the easiest way to install a proprietary driver.
 - In most cases, performance is top notch.

 
If your card is already two years old or more, it’s better to go with the recommended driver. Developers already had a few years to improve software for your card. Newer releases usually deal with removing bugs and improving performance on newer cards.
 
On the flipside, if your card is extremely new, you may have a lot to gain by using the most recent driver.
 
To proceed, press the Super key. On most keyboards, this is the key with the Windows logo on it. Type “software” and click on the “Software & Updates” utility. Its icon is a cardboard box with a flat globe on it (the first icon in the next picture).
 

 
In the top bar go to the “Additional Drivers” tab. In most cases the Nouveau open-source driver is preselected here. Click on “Using NVIDIA driver metapackage …” to switch to the proprietary driver. Next, click “Apply Changes,” and wait for the driver to install.
 
Reboot and enjoy the high performance driver which will let you use the full capabilities of your card.
 
## Install the Latest Nvidia Driver
 
You have a very recent card, launched just a few months ago. In this case you don’t want to wait until Ubuntu includes a better driver in their main repositories. To get the most recent software for your card, you can use a third-party repository.
 
Open a terminal emulator and enter the following command:
 
Update the package repository information.
 
Upgrade all packages on your system. Even if you know you have your system up to date, don’t skip this step. It is important and helps avoid some scenarios where packages from the PPA can conflict with other packages.
 
Find out what proprietary driver packages are available.
 
Install the latest, the one with the highest version number at the end. For example, in the previous picture “nvidia-driver-415” is the latest. Replace the name of this package in the next command, with what is the latest in your case.
 
Reboot your computer so that the new driver is loaded.
 
## Upgrading Your Nvidia Driver
 
Periodically, new packages will be released with newer Nvidia drivers.
 
Important: before upgrading the driver, you should always perform a general system upgrade first with sudo apt update && sudo apt upgrade.
 
Without following this step, you may get conflicts between older and newer packages from the PPA.
 
It’s worth mentioning that you can also use “Software & Updates” to upgrade your driver. It’s easier to use a program with a graphical user interface. However, it does come at a price. If there is a problem with installing the driver, you can’t see what the error is.
 
To upgrade the driver from the terminal, first list available drivers:
 
If a newer driver is available than what you have installed, upgrade to it with:
 
Replace VERSION_NUMBER_HERE with the latest version number you saw in the output of the previous command.
 
## How to Purge Nvidia Driver
 
In some cases you may get package conflicts which may be hard to solve manually. You can purge all Nvidia packages (and related) from your system with:
 
Reboot and then try your preferred method of installing an Nvidia driver (recommended, latest, from terminal or from “Software & Updates”).
 
## Conclusion
 
Performance of the closed-source, proprietary driver is miles away from the open-source one. In fact, with most of the modern cards and drivers, you will usually get between 90% and 100% of the performance you have on Windows. And with Steam’s Proton compatibility layer, that lets you play Windows games on Linux, and there’s plenty to enjoy.
 
Fell in love with computers when he was four years old. 27 years later, the passion is still burning, fueling constant learning. Spends most of his time in terminal windows and SSH sessions, managing Linux desktops and servers.
 
Our latest tutorials delivered straight to your inbox




