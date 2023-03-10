---
title: "Unlock Mind-Blowing Mac Dock Appearance Hacks: Control Your 2D or 3D Display Today!"
ShowToc: true 
date: "2022-12-01"
author: "Luann Cannon"
---
*****
There's no denying that a Mac Dock is a helpful tool to quickly launch apps, access folders, or switch between open windows. However, did you know that you can take the Dock's appearance to the next level by customizing it in various ways? Whether you prefer a minimalist approach or a flamboyant one, you can unlock mind-blowing Mac Dock appearance hacks to control your 2D or 3D display today. Here's how.

First, let's start with the obvious. To access the Dock, move your mouse to the bottom or sides of your screen, depending on where you've placed it. By default, the Dock appears in 3D, meaning that the icons have a slight shadow and reflection behind them. If you prefer a 2D appearance, go to the Apple menu, then System Preferences, and click on Dock. From there, select the "Scale effect" or "Genie effect" for the Dock animation and untick the "Magnification" option.

Now, let's delve into more advanced customization options. For instance, you can change the size of the Dock, its position, and its hiding behavior. To do so, right-click on the Dock's divider, select "Dock Preferences," and adjust the settings to your liking. You can also use Terminal commands to fine-tune these parameters or create keyboard shortcuts to show or hide the Dock quickly.

Another cool Mac Dock appearance hack involves changing the icons' size and style. By default, the Dock icons are small and squared, but you can make them bigger or smaller, circular, or even animated. One way to do this is by using third-party apps such as LiteIcon, CandyBar, or DockDesigner. These tools provide a user-friendly interface to browse and apply custom icon sets, as well as save and share your creations with others.

Moreover, you can add more functionality to the Dock by installing plugins or stacks. Stacks are folders that expand into a grid of items when clicked, allowing you to access multiple apps or files at once. To create a Stack, drag a folder to the right side of the Dock, and it will automatically transform into a fan or grid view, depending on your settings. You can also customize the Stack's appearance, title, and sorting method by right-clicking on it and selecting "Display as" and "View content as."

As for plugins, there are various options to choose from, depending on your workflow and preferences. For instance, you can add a weather widget that displays the current conditions and forecast for your location, a music player that integrates with iTunes or Spotify, or a clipboard manager that stores your copied items and lets you access them later. Some popular plugins include uBar, Dragthing, Bartender, or DockMate.

In conclusion, unlocking mind-blowing Mac Dock appearance hacks is a fun and creative endeavor that can enhance your productivity and enjoyment of your Mac. With a bit of experimentation and imagination, you can control your 2D or 3D display and make the Dock truly yours. Give it a try!

{{< youtube m2bF4U6EBZU >}} 




The Mac's Dock has undergone revisions over time. It started life as a basic 2D Dock that was flat and slightly translucent and then morphed into a 3D look with Leopard. With OS X Yosemite, the Dock reverted to a 2D look. If you became fond of the 3D look and want to experience it in OS X Yosemite or later, or if you have an OS with the 3D look and want the 2D appearance, it's possible to switch between the two Dock looks.

 

Here's a look at the evolution of the Dock and how to change back and forth between a 2D and 3D appearance using Terminal or the third-party cDock utility.

 
##   The Evolution of the Dock  
 

OS X Cheetah introduced the Dock, creating the Mac desktop's distinctive look. It was a basic 2D dock with the original Aqua pinstripe interface elements introduced in the first OS X version. The Dock morphed a bit through Puma, Jaguar, Panther, and Tiger, but remained 2D.

 
The information in this article applies OS X Leopard and later OS X and macOS versions as indicated.
 

With the advent of OS X Leopard, the Dock underwent a dramatic change with a three-dimensional, reflective look. The Dock icons looked like they were standing up on a ledge. The 3D look continued through Snow Leopard, Lion, Mountain Lion, and Mavericks. However, with OS X Yosemite came the return of the flat, two-dimensional Dock, which remained through subsequent releases.

 
##   Use Terminal to Apply a 2D Effect to the Dock  
 

Use Terminal with OS X Leopard, Snow Leopard, Lion, Mountain Lion, and Mavericks Docks that are currently sporting a 3D look.

 
- From the Utilities folder, launch Terminal or type Terminal into spotlight search.
 - Enter the following command line into Terminal. Copy and paste the command or type it in exactly as shown in a single line of text.
 - defaults write com.apple.dock no-glass -boolean YES
 - Press Return.
 - Enter the following text into Terminal. If you type the text rather than copy and paste it, be sure to match the case of the text.
 - killall Dock
 - Press Return.
 - The Dock disappears for a moment and then reappears.
 - Enter the following text into Terminal.
 - exit
 - Press Return. Terminal ends the current session.
 - Quit the Terminal application. Your Dock should now revert to a 2D look.

 
##   Use Terminal to Switch Back to a 3D Dock Effect  
 

Use this Terminal trick with OS X Leopard, Snow Leopard, Lion, Mountain Lion, and Mavericks Docks that currently sport a 2D look.

 

From the Utilities folder, launch Terminal or type Terminal into spotlight search.

 

Enter the following command line into Terminal. Copy and paste the command or type it in exactly as shown in a single line of text.

 

defaults write com.apple.dock no-glass -boolean YES

 

Press Return.

 

Enter the following text into Terminal. If you type the text rather than copy and paste it, be sure to match the case of the text.

 

killall Dock

 

The Dock disappears for a moment and then reappears.

 

Enter the following text into Terminal.

 

exit

 

Press Return. Terminal ends the current session.

 

Quit the Terminal application. Your Dock should now revert to a 2D look.

 
- From the Utilities folder, launch Terminal or type Terminal into Spotlight Search.
 - Enter the following command line into Terminal. Copy and paste the command or type it in exactly as shown in a single line of text.
 - defaults write com.apple.dock no-glass -boolean NO
 - Press Return.
 - Enter the following text into Terminal. If you type the text rather than copy and paste it, be sure to match the case of the text.
 - killall Dock
 - Press Return.
 - The Dock disappears for a moment and then reappears.
 - Enter the following text into Terminal.
 - exit
 - Press Return. Terminal ends the current session.
 - Quit the Terminal application. Your Dock should now revert to a 3D look.

 
##   Use cDock to Change the 2D or 3D Dock Aspect  
 

A third-party app called cDock changes the 2D or 3D aspect of your Dock and provides other customizations, including transparency controls, custom indicators, icon shadow, reflections, and more.

 

From the Utilities folder, launch Terminal or type Terminal into Spotlight Search.

 

defaults write com.apple.dock no-glass -boolean NO

 

Quit the Terminal application. Your Dock should now revert to a 3D look.

 

If you have OS X Yosemite, installing and using cDock is a simple process. For OS X El Capitan through macOS Big Sur, installing cDock requires an extra step that involves disabling your SIP (System Integrity Protection). This security measure prevents potentially malicious software from modifying protected resources on your Mac. While cDock is by no means malicious, the SIP security system prevents cDock's Dock-modification methods.

 

Disabling the SIP system isn't recommended just to perform cosmetic Dock changes. If you choose to go ahead with the process, cDock includes instructions for how to disable SIP.

 
###   How to Use cDock  
 

Here's how to change your Dock's appearance using cDock:

 
- Download cDock. The most recent version is cDock 4, which is compatible with Macs running macOS Mojave (10.14) or higher. Earlier versions are available at the cDock website for older operating systems.
 - Open the downloaded Zip file.
 - Open cDock.
 - Allow cDock to move itself to the Applications folder.
 - If you're using a version later than Yosemite, disable System Integrity Protection.
 - Apple doesn't recommend disabling System Integrity Protection. Do so at your own risk.
 - cDock installs its system components.
 - Re-enable System Integrity Protection. To do this, start your Mac using the Recovery partition. Launch Terminal and enter this command:
 - csrutil enable
 - Press Return, quit Terminal, and restart your Mac.
 - Use the cDock menus to change the Dock's appearance, including switching to a 3D Dock.

 

Download cDock. The most recent version is cDock 4, which is compatible with Macs running macOS Mojave (10.14) or higher. Earlier versions are available at the cDock website for older operating systems.

 

Open the downloaded Zip file.

 

Open cDock.

 

Allow cDock to move itself to the Applications folder.

 

If you're using a version later than Yosemite, disable System Integrity Protection.

 
Apple doesn't recommend disabling System Integrity Protection. Do so at your own risk.
 

cDock installs its system components.

 

Re-enable System Integrity Protection. To do this, start your Mac using the Recovery partition. Launch Terminal and enter this command:

 

csrutil enable

 

Press Return, quit Terminal, and restart your Mac.

 

Use the cDock menus to change the Dock's appearance, including switching to a 3D Dock.

 
The cDock app is not currently compatible with M1 Macs.
 

Get the Latest Tech News Delivered Every Day




