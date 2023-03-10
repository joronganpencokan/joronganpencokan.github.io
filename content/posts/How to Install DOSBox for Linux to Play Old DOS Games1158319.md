---
title: "Unlock a Whole New World of Vintage Gaming: Learn How to Install Dosbox on Linux Today!"
ShowToc: true 
date: "2023-02-07"
author: "Jessie Jones"
---
*****
Unlock a Whole New World of Vintage Gaming: Learn How to Install Dosbox on Linux Today!

If you're someone who loves vintage gaming classics like Doom, Prince of Persia, and Monkey Island, you'll be happy to know that you don't need to rely on ancient hardware to play these games. Instead, you can install the Dosbox emulator on your Linux system and run all your favorite DOS games like it's the 90s again.

Dosbox is an emulator program that allows you to run old DOS games and applications on modern hardware. It works by emulating the DOS environment on your system so that games and other applications run as they did on an old-school PC. So, if you're a fan of nostalgic gaming, this is your chance to unlock a whole new world of vintage gaming.

The good news is that installing Dosbox on Linux is pretty easy. Here's how you can do it:

Step 1: Open the Terminal

To install Dosbox on Linux, you'll need to use the Terminal. To open it, click on the Applications menu and select Terminal. Alternatively, you can use the shortcut keys Ctrl+Alt+T.

Step 2: Update the System

The next step is to update your Linux system to ensure that everything is up to date. To do this, enter the following commands in the terminal one by one:

sudo apt-get update
sudo apt-get upgrade

Step 3: Install Dosbox

Now that your system is up to date, you can move on to installing Dosbox. To do this, enter the following command:

sudo apt-get install dosbox

Step 4: Run Dosbox

With Dosbox installed, you can now start it by typing "dosbox" in the Terminal. Dosbox works like a command-line program, so you'll need to type in commands to run your games. For example, to mount the C:\ drive, you can use the following command:

mount c /mnt/mygame

Replace "/mnt/mygame" with the path where your game files are stored. Once you have mounted the drive, you can run your game by typing its executable file name. For example:

c:\
cd gamefolder
game.exe

And that’s it, you can now enjoy vintage games in all their old-school glory!

In conclusion, if you're a fan of vintage gaming and haven't yet tried Dosbox, you're missing out on a whole new world of fun. With Dosbox installed on your Linux system, you can revisit the classics of the past and reminisce about the good old days. So, what are you waiting for? Go ahead and install Dosbox on Linux today and let the nostalgia take over!

{{< youtube uMe4O5WhtJQ >}} 



If you own copies of old DOS games like DOOM, you can still play these retro games on your PC with the help of an emulator. DOSBox is the best DOS emulator around. Most guides for DOSBox focus simply on installing the application and providing a couple of commands to get you going. However, this is likely to scare off new users, and there’s a nasty surprise awaiting DOS veterans as well. 
 
This guide will not only cover how to install DOSBox for Linux but also how to automatically mount your C: drive. And for the newbies out there scared of DOS commands, it also lays out a recommendation for a classic piece of software to help you along!
 
## Installation of DOSBox for Linux
 
Installing DOSBox is easy as it’s in the repositories of almost every distribution and should be accessible under any package manager. If you prefer to install by command line:
 
Once installed, the program should be in your system menu or can be started by entering:
 
## Usage of DOSBox for Linux
 
Once inside DOSBox, it’s easy to feel lost. Rather than launching with a prompt at “C:”, DOSBox starts its prompt at Z: (DOSBox’s internal virtual drive) with a recommendation on how to mount a new C: drive manually. This will scare off new computer users as well as annoy DOS veterans who just want a prompt at C: ready and waiting. To get around this, you need to edit DOSBox’s startup files.
 
On a normal DOS installation this would just involve editing “autoexec.bat” on the root of your C: drive. However, DOSBox uses a local configuration file in a sub-directory of your home folder to organize its commands.
 
To access this file, first enable hidden files and folders in your file manager, then open the “.dosbox” directory in your home folder. This is presuming you have run DOSBox at least once. If not, run it and close it. There should be a file called “dosbox-0.74.conf.” (Your version number may differ.)
 
It’s worth scrolling through this text file to see all the available options for any future tweaking, but for now we’re only interested in the [autoexec] section at the end. As the comments will note, this is for any commands you want running automatically at startup. Any sane person will put their mount commands here. For now this area is blank, but you will enter new lines here in the steps to follow.
 
These steps presume anything you want on your C: drive will be stored in a directory called “dosbox” directly in your home folder. If you don’t already have such a directory, create it now and copy into it any DOS software you want to run. With the DOSBox configuration file, enter these two new lines under the [autoexec] section:
 
Save the file. When you open DOSBox now it will automatically open at C:, ready to access everything in your dosbox folder.
 
### DOS Basics for the Unafraid
 
Change directory:
 
Go back a directory:
 
Browse a directory and view long file lists page by page:
 
Start an executable program by entering the name of the file; the extension isn’t necessary. For instance, wolf3d.exe just needs:
 
## But I Just Want To Play Games, Not Learn DOS!
 
Although it’s worth learning some basic DOS commands, it’s not strictly necessary. There was an enormous selection of software designed to create a friendly interface for anyone who didn’t want to learn how to use a DOS terminal. My personal recommendation would be The Norton Commander: an all time classic file manager that popularized twin-pane file browsing. It spawned a countless number of imitation projects, including Midnight Commander on Linux.
 
Use the arrow keys to browse through files, pressing Enter on any file you want to launch or directory you want to enter. To change between the two panes, press Tab. The function keys perform tasks like copying, renaming, deleting, and so on. Sadly, Norton Commander is an abandonware. There is no official link, but you should still be able to find it with Google search. 
 
Assuming you have Norton Commander under the “NC” directory in your dosbox folder, you can start it with the commands:
 
Or to be more precise:
 
To make Norton Commander run automatically at startup, you can add this command to the [autoexec] section of the DOSBox config file so that it now looks like this:
 
You should now be able to run DOS games with ease and just copy any new games into your dosbox folder at will. If you would like to know more about DOS commands or where to find software, check out our excellent guide on DOSBox for Mac.
 
John Knight is a writer, most notably for Linux Format (UK), Linux Journal (US), and Maximum PC (US). Outside of open source and general computing material, John has also written for automotive publications, and is currently writing material on vintage gaming and drumming. Other areas of interest include Psychology, French, and Japanese.
 
Our latest tutorials delivered straight to your inbox




