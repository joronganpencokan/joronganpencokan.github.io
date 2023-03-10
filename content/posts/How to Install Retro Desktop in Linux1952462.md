---
title: "Transform Your Linux Into a Vintage Powerhouse With This Simple Retro Desktop Installation Tutorial!"
ShowToc: true 
date: "2023-07-02"
author: "Frances Lasky"
---
*****
Transform Your Linux Into a Vintage Powerhouse With This Simple Retro Desktop Installation Tutorial!

Linux is the most widely used operating system among developers, engineers, and system administrators. It has gained popularity over time due to its open-source philosophy, flexibility, and customizability. With these benefits, Linux has become the go-to option for developers and seasoned tech enthusiasts searching for alternative operating systems.

If you're a fan of classic and vintage aesthetics, the Retro desktop installation is the best option for you. Retro, which is a desktop environment, gives users an experience of using an old classic computer even with modern hardware. In this tutorial, we'll go over the steps required to install and set up the Retro desktop on your Linux machine.

Installation of the Retro Desktop

To start with, ensure that your system is updated to the latest version. Once you're done with that, open the Terminal using the keyboard shortcut, or search for it from your applications menu. Then analyze the system dependencies required for the Retro desktop. To do this, copy & paste this command and press the enter key: 

sudo apt-get update
sudo apt-get install build-essential autoconf automake libtool

After running this command, wait for a few minutes for the installation to complete. Once that's done, you can proceed to download the Retro desktop packages. To get the desktop package, you need to add the Retro desktop repository to your system. Run the following command:

sudo add-apt-repository ppa:headsnet/retroarch

This adds the Retro desktop repository to your apt sources list. After that is complete, run the update command again with the command:

sudo apt-get update

Next, install the Retro desktop packages with the command:

sudo apt-get install retroarch retroarch-assets

This command installs the necessary packages for the Retro desktop environment to work correctly.

Setting up the Retro Desktop

Once installation is complete, it's time to set up the desktop environment. To access the Retro desktop, log out of your current account and select the Retro option from the menu that appears on the login screen.

The first time you log in to the Retro desktop, you'll be presented with a setup wizard. Follow the instructions to configure the desktop environment according to your preferences.

After completing the setup, you can customize the desktop environment further by installing Retro-themed icons, fonts, and wallpapers. For example, you can install the Retro GTK theme using the command:

sudo apt-get install retro-gtk-theme

Once the theme is installed, you can then select it from your system's preferences to give your desktop a vintage feel.

In conclusion, installing the Retro desktop on your Linux machine is a simple and straightforward process. If you're a fan of classic aesthetics, this desktop environment provides a nostalgic experience while providing you with modern features and functionality. With this tutorial, transforming your Linux machine into a vintage powerhouse has never been easier.

{{< youtube j5UeSj2F-yc >}} 



Linux users have an almost infinite number of UI’s to from which to choose. Arguments over which is best among mainstays like KDE, GNOME, Unity, and XFCE can (and have) go on for days on Internet boards. Purists can still just use the command line. There are even desktops designed to give users the “retro” feeling by emulating earlier desktops on Linux or other operating systems. Here’s how to install some old-school desktops.

 
## Do you miss KDE3?
 
The switch to KDE4 caused some problems in the community when it was first released. For those who miss the old style of KDE, the Trinity Desktop Environment project has you covered.
 
To install this retro KDE desktop, take the following steps:
 
Add the following lines to your “/etc/apt/sources.list” file:
 
Note: The latest stable Trinity Desktop supports up to Precise in Ubuntu. To install on Quantal, you’ll need to try the Nightly builds.
 
Also add the Trinity GPG key:
 
Next, update your package lists
 
Lastly, install from the repository:
 

 
Then you can select it from your Display Manager next time you log in. I installed this on my old (PIII) Gateway notebook, and was pleasantly surprised (and more than a little nostalgic). Which brings us even further back in time…
 
## Nostalgic for Windows XP?
 
Regardless of how you feel about Microsoft, the Windows interface (starting with Windows 95) set a standard for UI’s that many systems (including Linux) still follow today. If you’re looking for a WinXP-like experience on Linux, icewm uses a similar layout with a “Start”-style menu in the lower-left corner, a system tray in the lower right, and a list of running tasks between the two. The window manager even provides a theme for window decorations that looks like the old blue-and-green.
 
To install icewm on your Ubuntu system, select it from the Software Centre, or use the following command:
 
Note that there are configuration utilities for icewm (iceconf and icemc), but they’ve been removed from the repositories, so you may be required to manage this through configuration files found in the “~/.icewm/” directory. Fortunately, there’s a nice explanation of how to do so on the Ubuntu Help site.
 
## Pining for Amiga?
 
Lastly, if you’re an Amiga fan from back in the day, you’re not alone among Linux users. The community has worked to bring the Workbench UI from the old Amiga machines to Linux in the form of amiwm. This window manager is decidedly minimalist, but Amiga users will feel right at home.
 
amiwm runs very light, as it consists of a single package (the dependencies of which should be installed out of the box on most Ubuntu systems), which can be installed with the following command:
 
Like icewm above, configuration of amiwm is done through a configuration file, specifically “~/.amiwmrc”. And while there are no utilities to help with configuration, some guidance and sample config files can be found around the Web.
 
To get an appreciation for how far the Linux desktop has really come, give some of these a try sometime. Or if you have a low-powered machine, one of these can be a fine alternative to the more robust (and more resource-hungry) options of GNOME, Unity, and KDE.
 
Aaron is an interactive business analyst, information architect, and project manager who has been using Linux since the days of Caldera.  A KDE and Android fanboy, he'll sit down and install anything at any time, just to see if he can make it work.  He has a special interest in integration of Linux desktops with other systems, such as Android, small business applications and webapps, and even paper.
 
Our latest tutorials delivered straight to your inbox




