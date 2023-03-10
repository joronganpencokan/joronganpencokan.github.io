---
title: "Discover the Mind-Blowing Hack to Unlock Extreme Screen Resolution on Linux - Say Goodbye to Blurry Screens Forever!"
ShowToc: true 
date: "2023-07-06"
author: "Donald Tiger"
---
*****
Discover the Mind-Blowing Hack to Unlock Extreme Screen Resolution on Linux - Say Goodbye to Blurry Screens Forever!

If you are a Linux user and have ever experienced blurry screens and low resolution, this article is just for you. With the help of some simple hacks, you can unlock extreme screen resolution on Linux and get rid of those annoying blurry screens forever.

Firstly, you need to understand the reason behind the blurry screens. Linux systems, by default, use an open-source X server that controls the screen resolution. This server is usually set to a lower resolution to ensure that the system runs at optimal speed. However, this can result in blurry screens that can be frustrating for users who need high-quality displays for their work or leisure activities.

Fortunately, there is an easy way to change this. By installing a third-party X server, you can get access to higher screen resolutions, resulting in sharper and clearer displays.

One of the most popular third-party X servers is Xpra. This software comes with a host of features that enable you to customize your screen resolution to suit your preferences. You can use Xpra to customize the screen resolution to give you exactly what you need for your work or leisure activities.

To get started with Xpra, you need to install it on your Linux system. You can do this by running the following command:

sudo apt-get install xpra

Once Xpra is installed, you can configure your screen resolution by running the following command:

xpra start :100 --start-child=glxgears --dpi=96 --desktop-scaling=1.5 --html=on

In this command, you need to replace "glxgears" with the name of the application you want to run. You can also adjust the DPI and desktop scaling parameters to suit your preferences.

Once you have configured Xpra, you need to launch it by running the following command:

xpra attach

This will launch the application, and you can adjust your screen resolution to the desired level by using the resolution settings in the Xpra menu.

In conclusion, Linux users can now enjoy extreme screen resolution by using Xpra. By following the simple steps outlined in this article, you can unlock higher screen resolutions, resulting in sharper and clearer displays. Say goodbye to blurry screens forever and experience Linux at its best.

{{< youtube UTsRPk32Kjw >}} 



If you have a old desktop monitor, or are using a netbook with limited screen space, you know that you are stucked with the small screen size and there is practically nothing you can do about it (or do you?) Newrez is a simple application for Linux (Gnome to be more specific) that allows you to stretch your screen resolution beyond the monitor default. That means, if you are stuck at a 1024×768 resolution for your netbook, you can set it to run at 1280 or 1920 width.

Note: Newrez is not an elegant application and is not without problems. However it is one great solution to one annoying hardware limitation.   
 
1. Download newrez from gtk-apps.
 
2. Inside the zipped file, there should have two files – newresz and newresz-v. Extract the two files and place newresz in the “Home -> .gnome2 -> nautilus-scripts” folder. If the nautilus-scripts does not exist, create it. 
 
3. Next, kill your nautilus by typing “killall nautilus” in the terminal.
 
4. At your desktop, right-click your mouse and navigate to “Scripts -> newresz”. You should see the following:
 

 
5. Enter the resolution size that you want to set, say 1280, or 1920 and click OK. If everything go well, your screen should automatically resized to the new width. 
 
## Problems you might face
 
1. The script does not work
 
1. Check to see if you are using Gnome.
2. I have tested it with an integrated intel graphics and it works fine. However, since it requires XRandr and several AMD and Nvidia grpahics cards do not play well with XRandr, you might experience problem with the script.
 
2. There is no ways to restore back to the original settings
 
To restore, you just have to run the script again and set it to the original resolution. 
 
3. The resized screen shows a black border box and the mouse can’t move into the box
 
This happens when you are on Gnome 3.x and it is a known-bug that is yet to solve (as of this post). Try the alternative method listed below.
 
## Alternative to newresz
 
Remember there are two files in the zipped folder? The other file, newrez-v is an alternative to newrez and should work in all systems. The trick here is to create a vnc server at a higher resolution and then starts a vncviewer in scaled mode. 
 
1. Open a terminal and type:
 
2. Next, open the newrez-v file with a text editor. Scroll down to the end of the file (at around line 81), change the value behind the depth to ’24’ and the geometry to the screen size that you want to set (for example: 1920 x 1080)
 
Save and close the file.
 
3. Back to the terminal, run the newrez-v file (the one time need to be run from the command line. Subsequent launch can be done from Nautilus)
 
Remember to change the path to the exact location of the file. This will configure the vnc settings. Once it is done, it will run the default VNC viewer with the screen size you specified. If you have specified a larger screen size, everything will be shrink down and look smaller than the default. 
 
Image credit: several monitors with magnetic resonance images by Big Stock Photo
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




