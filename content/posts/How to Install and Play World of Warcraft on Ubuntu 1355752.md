---
title: "Unleash The Power: Discover The Ultimate Guide To Playing World Of Warcraft On Ubuntu!"
ShowToc: true 
date: "2022-12-01"
author: "Rose Hambleton"
---
*****
Introduction

World of Warcraft, also known as WoW, is a massively multiplayer online role-playing game (MMORPG) that has been popular among gamers since its release in 2004. Many people enjoy playing WoW on their Windows or Mac computers, but what about Ubuntu users? Is it possible to play WoW on Ubuntu? The answer is yes, and in this article, we will explore the ultimate guide to playing World of Warcraft on Ubuntu.

Step 1: Install Wine

Wine is a compatibility layer that allows Ubuntu users to run Windows applications, including games. To install Wine, open the terminal and type:

sudo apt-get install wine

This will download and install Wine on your Ubuntu system.

Step 2: Download the WoW client

To play WoW on Ubuntu, you need to have a copy of the game client. You can download the client from the official WoW website or from Blizzard's Battle.net app.

Step 3: Install the WoW client using Wine

Once you have downloaded the WoW client, you need to install it using Wine. To do this, right-click on the downloaded file and select Open With > Other Application. In the dialog box, choose Wine and click on the Open button.

This will start the installation process, and you need to follow the instructions provided by the installer. Make sure to select the correct language and region settings during the installation.

Step 4: Configure Wine for WoW

After installing the WoW client, you need to configure Wine for optimal performance. The first step is to install the necessary Windows DLL files. You can do this by running the following commands in the terminal:

winetricks corefonts vcrun2017

This will download and install the required DLL files.

Next, you need to configure Wine to use OpenGL instead of DirectX. To do this, open the Wine configuration tool by running the command:

winecfg

In the Graphics tab, select the "Emulate a virtual desktop" option and choose a resolution that matches your screen size. Then, select the "Automatically capture the mouse in the full-screen window" option.

In the Libraries tab, add the "d3d9" library and set it to "disabled".

Step 5: Launch WoW on Ubuntu

Now, you are ready to launch WoW on your Ubuntu system. To do this, navigate to the directory where you installed the WoW client and run the following command in the terminal:

wine Wow.exe

This will launch WoW, and you can start playing the game on your Ubuntu system.

Conclusion

Playing World of Warcraft on Ubuntu is possible, thanks to Wine. By following the steps outlined in this article, you can unleash the power of WoW on your Ubuntu system and enjoy the game alongside Windows and Mac users. So go ahead and discover the ultimate guide to playing World of Warcraft on Ubuntu!

{{< youtube QA9DJo9438g >}} 



As World of Warcraft’s seventh expansion draws nearer, interest in the venerable MMO is peaking again. For a long time WoW has been a game known to work well through the Wine compatibility layer on Linux, even though it’s never been officially supported. There was even a time when rumors were flying that Blizzard’s developers tested WoW for Wine compatibility.
 
Since World of Warcraft dropped OpenGL support and moved to DirectX 11, things haven’t been so simple. There’s been plenty of breakage and odd graphical glitches, and that doesn’t take into account the problematic Battle.net app or the decreased framerates. But it can still be just as easy as before.
 
Lutris and its scripted installs make playing World of Warcraft on Ubuntu about as easy as it is on Windows, and the performance is great, even on lower-powered systems.
 
## Make Sure Your Drivers Are Installed
 
Before you go any further, make sure that you have the latest drivers installed for your graphics card. Check out the Steam guide. It does a great job covering driver installation pretty. Once you have your drivers installed, reboot your computer to make sure that you’re using them.
 
## Install Lutris
 
Lutris isn’t in the default Ubuntu repositories, but the Lutris developers do maintain a convenient repository. Before you get that set up, though, you’ll need to create a Lutris account, if you don’t already have one.
 
### Create Your Lutris Account
 

 
Head over to the Lutris registration page and create your account. Lutris only uses the account to keep track of your downloads and your library. They don’t sell you anything or try to track you. You only need to give it a username, email, and password.
 
### Add the Lutris Repository
 
These repository instructions are straight form Lutris. They first look for which version of Ubuntu you’re running, then create a file in your Apt sources directory that points to the repository for your version of Ubuntu. Finally, they import the GPG signing key for the repository.
 
After you’ve run all three commands, you’re ready to update Apt and install Lutris. From now on, you’ll receive regular updates for Lutris on your system.
 
### Install Lutris
 
Update Apt and install Lutris like you normally would.
 
## Run the WoW Installer
 
Lutris has a page on its website for each game that it supports. WoW is no exception. Go to the Lutris WoW page, and click on the “Install” button below the main image. Your browser will ask you if you want to open the script with Lutris. Click “Agree.”
 
A new window will pop open. It’ll start off by asking if you do, in fact, want to begin installing WoW. Click to confirm. The Lutris install script will kick off and start setting up your Wine prefix for WoW. In the process, it’ll download a few Windows components and fonts to make everything go smoothly.
 
Next, the installer will start the regular Battle.net installer. Follow the steps for Battle.net. When it’s done, don’t sign in. Instead, close the Battle.net window to allow the installer to finish. After a couple of seconds, Lutris will show you a success message. Close the message window. There’s something else you need to do.
 
## Check For Wine Updates
 
Wine updates frequently, and those updates usually bring performance improvements with them. Before you start the game, it’s best to make sure that you’re using the latest version of Wine.
 
Click on the “Runners” icon at the top of the main Lutris window. It’s the second icon from the left, and it looks like gears by default.
 
A new window will pop open, displaying a list of available runners. The list is alphabetical, so Wine is towards the bottom. Scroll down and click on Wine. A new window will pop open listing the available Wine versions. There are a lot. Look for the latest version with the PBA patches. It’ll have “pba” in the name. Click on the checkbox next to the name to start downloading it. If it’s already checked, you have the latest one. Close both runner windows, and return to the main Lutris screen.
 
Right-click on the WoW banner image, and select “Configure” on the menu that pops open. Another window will open up with all the available options for your WoW install. Click on “Runner options,” and look for the Wine option. Select the Wine version, and choose the latest version of Wine-PBA.
 
Return to the main Lutris window.
 
## Play World of Warcraft
 
Click on the WoW banner image to launch the game. Actually, it’s not the game. The Lutris installer can only go so far, and it can’t script the Battle.net client. You’re going to need to sign in to your Battle.net account and click the “Install” button for WoW yourself. There’s nothing special that you need, though. This is just the standard procedure, like on Windows.
 
The game will take some time to download. World of Warcraft weighs in at around 50GB. After you have it, launch the game with “Play.”
 
It’s always a safe bet to turn your settings down at first to make sure that everything is working properly. Then, slowly dial it up to see what your computer can handle. Try exploring a capital city in the game to test it.
 
The latest patch for the expansion just launched. Don’t expect perfection. In testing this, there was a weird bug where textures didn’t load. It seems like a texture caching thing because it did stop, but just be prepared. That also means that you shouldn’t have any new problems when Battle for Azeroth does launch.
 
That said, there’s no reason you can’t enjoy the game to its fullest. And, of course, FOR THE HORDE!
 
Nick is a freelance tech. journalist, Linux enthusiast, and a long time PC gamer.
 
Our latest tutorials delivered straight to your inbox




