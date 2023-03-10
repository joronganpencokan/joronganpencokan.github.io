---
title: "Transform Your Ugly Gtk3 Apps Into Sleek Masterpieces in Kde4 with This One Simple Trick!"
ShowToc: true 
date: "2023-05-07"
author: "Rhonda Baumann"
---
*****
Transform Your Ugly Gtk3 Apps Into Sleek Masterpieces in Kde4 with This One Simple Trick!

Are you sick and tired of looking at those ugly, unpolished Gtk3 applications in your Kde4 desktop? Do you wish there was a way to give them a makeover and turn them into sleek, masterpieces that blend seamlessly with your desktop environment?

Well, you're in luck because there is actually one simple trick that can help you achieve this without having to spend countless hours tweaking and customizing your desktop. And the best part is that it's easy enough even for beginners to follow.

The trick is to install a Kde4 widget called "gtk3-nocsd," which essentially disables client-side decorations (CSD) in Gtk3 applications and replaces them with the standard Kde4 window decorations. This makes the applications look much more polished and integrated with the overall look and feel of your desktop.

So, how do you install this widget? It's actually quite simple. All you need to do is follow these few steps:

Step 1: Open your terminal and enter the following command to add the corresponding PPA to your system:

sudo add-apt-repository ppa:no1wantdthisname/ppa

Step 2: Update your system package list by running the following command:

sudo apt-get update

Step 3: Install the widget by typing the following command:

sudo apt-get install gtk3-nocsd

That's it! Once the installation process is complete, you can now launch any Gtk3 application and see the transformation for yourself. The windows of the application will now have the same window decoration as your Kde4 applications, making them blend in seamlessly with your desktop. No need for any further tweaking or customization.

Of course, you may still want to customize the colors and fonts to your liking, but that's entirely up to you. The important thing is that the application now looks much better and feels more at home in your Kde4 environment.

In conclusion, if you're looking to transform those ugly Gtk3 applications into sleek masterpieces in Kde4, then look no further than the gtk3-nocsd widget. It's a simple and easy trick that can make a world of difference in how your desktop looks and feels. So why not give it a try today? Your eyes (and your desktop) will thank you!


With the release of Gnome 3, many developers of GTK apps have begun to port their programs from GTK2 to GTK3. If you have used Ubuntu 11.04, you will notice that many of the popular GTK2 themes did not yet have GTK3 equivalents, which left the few GTK3 applications looking awful.

The latest versions of Fedora, Ubuntu, and other Linux distributions have better support for GTK3 for Gnome, XFCE and other GTK-based desktops, but if you are a KDE user, you might have noticed that the default Oxygen theme works for GTK2 apps but not for GTK3. The following brief guide will explain how to get your GTK3 apps looking good in KDE. Nothing you do here will affect your GTK2 applications or your KDE installation.
 

 
## Oxygen-GTK3
 
The solution to this problem is a package called oxygen-gtk3, which has made its way into some Linux distributions. If it is not in your distribution’s default repository (and it probably is not unless you have the most bleeding edge release), you can likely get the package from a third party.
 
For Kubuntu and other Ubuntu-based distributions, add the following repository:
 
Then, install the package called gtk3-engines-oxygen:
 
For OpenSUSE, you need to add the swyear repository:
 
Then, install the oxygen-gtk3 package:
 
Other distribution installation procedures will vary. I did find Fedora packages available from this user, but did not find any distribution-specific installation instructions.
 
For Archlinux, you need to install oxygen-gtk3-git from AUR.
 
## Completing the Installation
 
If you have come this far, you might have noticed that your GTK3 applications still look awful, even after you restarted your desktop environment. That is because GTK3 requires its own configuration file called settings.ini, which may remind you of your old Windows days. Fortunately, this settings.ini is not quite so aggravating, and you will only need to add a single configuration line.
 
If one does not already exist, create a folder at this location “~/.config/gtk-3.0“. In Archlinux, you can apparently just link to the default file:
 
Next, create a file inside the gtk-3.0 folder called settings.ini. Using the text editor of your choice, add this line:
 
Save and close your text editor, and the settings should take effect immediately. If not, restart your desktop environment. When you open applications like Gufw, you should now see your Oxygen theme rather than the ugly , un-themed GTK3 default that it previously displayed. There have been some reports of certain apps crashing on some distributions. I have not experienced this, but if you do, you should definitely report it to the appropriate developers.
 
## Keeping it Seamless
 
KDE users tend to like everything to flow nicely together. Oxygen-gtk3 allows you to keep your desktop looking seamless even when you need to use a GTK program. With the next major releases of most Linux distributions, you will probably see this package added by default, requiring no further action on your part. Until then, the above instructions should remain valid and usable.
 
Tavis J. Hampton is a  freelance writer from Indianapolis.  He is an avid user of free and open source software and strongly believes that software and knowledge should be free and accessible to all people. He enjoys reading, writing, teaching, spending time with his family, and playing with gadgets.
 
Our latest tutorials delivered straight to your inbox




