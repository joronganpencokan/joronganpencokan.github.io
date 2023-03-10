---
title: "Master the Ultimate Linux Setup Hack: Learn How to Install and Configure Bspwm for a Seamless User Experience!"
ShowToc: true 
date: "2023-03-04"
author: "Don Sonnier"
---
*****
Master the Ultimate Linux Setup Hack: Learn How to Install and Configure Bspwm for a Seamless User Experience!

Linux is an open-source operating system that is popular among developers, system administrators, and those who value security and privacy. One of the reasons why Linux is so popular is because of its customizability. With Linux, you can personalize your system to suit your unique needs and preferences. However, customizing Linux can also be a daunting task, especially for new users. That's where Bspwm comes in. Bspwm is a window manager that can help you organize your desktop and improve your Linux experience. In this article, we will show you how to install and configure Bspwm for a seamless user experience.

What is Bspwm? 

Bspwm (Binary Space Partitioning Window Manager) is a tiling window manager for Linux. Tiling window managers are different from traditional window managers in that they organize desktop windows in a tile-like pattern, allowing you to view multiple windows at the same time without overlapping. Bspwm is lightweight and fast, making it ideal for older or low-powered computers.

Installing Bspwm

Before you install Bspwm, you need to ensure that your system has the dependencies required to run Bspwm. Here are the dependencies:

• Xorg – A display server 

• Xterm – A terminal emulator

• Compton – A compositor manager

• Feh – A lightweight image viewer

• Rofi – A window switcher and application launcher

• Polybar – A customizable status bar

If you are using Ubuntu or Debian, you can install these dependencies by running the following command:

sudo apt-get install xorg xterm compton feh rofi polybar

Once you have installed the dependencies, you can install Bspwm. To install Bspwm, you need to clone the Bspwm GitHub repository. You can do this by running the following command:

git clone https://github.com/baskerville/bspwm.git

After cloning the repository, you need to compile and install Bspwm. You can do this by running the following commands:

cd bspwm

make

sudo make install

Configuring Bspwm

After installing Bspwm, you need to configure the window manager. Bspwm is configured using a configuration file called bspwmrc. The bspwmrc file is located in the ~/.config/bspwm directory. Here is an example of a basic bspwmrc file:

#! /bin/sh

bspc monitor -d I II III IV V VI VII VIII IX X

bspc config focused_border_color "#ff8800"

bspc config normal_border_color "#383c44"

bspc config border_width 2

polybar example &

feh --bg-scale ~/Pictures/wallpaper.jpg &

compton -b

In this example, we have set up the default desktops and configured the border color and width. We have also launched Polybar, and set a wallpaper using Feh. Finally, we have enabled a compositor using Compton.

Conclusion

Bspwm is an excellent window manager for Linux users who want to improve their desktop experience. It is lightweight and fast, and it allows you to customize your desktop to your liking. By following the above steps, you will be able to install and configure Bspwm on your Linux system. Once you get the hang of it, you'll be able to master the ultimate Linux setup hack!

{{< youtube _55HGnz422M >}} 



Binary Space Partitioning Window Manager (bspwm) is a powerful minimalist window manager for Linux. It is highly configurable and it proposes an innovative approach to window management. Bspwm is written in C and it can be configured using any language. Bspwm is the epitome of user customization in window managers. This makes it attractive to power users and tinkerers who are interested in learning to create their own unique workflow.
 
## Binary Space Partitioning, Explained
 
Binary Space Partitioning is the idea that windows in a desktop can be represented as leaves in a full binary tree. A full binary tree is a structure of ordering information using hierarchical nodes. Any information within that tree is sorted in twos with a root node always containing two nodes.
 
Bspwm works with nodes. In practice, when you create a window on an empty desktop, bspwm will create a single node for that window to be placed in. You can think of that node as a leaf node. But when you create an additional window in that desktop, that leaf node will become a root node and bspwm will create two new leaf nodes attached to it. It then places the current window and the newly created one into those leaf nodes.
 
Any new window that will be created after this will now be associated with either one of those leaf nodes, turning those into their own respective root nodes.
 
Arranging windows in this way creates a clear hierarchy within the desktop. It is clear which leaf nodes were spawned first and which are the ones that are from a particular group of root nodes. This is useful when creating custom behavior rules for specific windows and window layouts.
 
## Keybindings and Status Bars
 
It is important to note that bspwm only manages windows. This means that any other function that is not related to managing windows are not included in the bspwm package. This includes the ability to bind keys to functions and also the ability to display a status bar.
 
In order to use keybindings in bspwm, the developers created a separate program called the Simple X Hotkey Daemon (sxhkd) that only manages keybindings. For the status bar, however, the user can install a variety of third-party applications such as polybar and lemonbar.
 
## Installing bspwm and sxhkd
 
Installing bspwm and sxhkd is relatively straightforward. Both programs are also available in most Linux repositories. For example, to install those in Debian and Ubuntu you can do so using apt:
 
In Arch Linux, you can use pacman:
 
In Fedora, you can use dnf:
 
For Void Linux, you can use xbps:
 
In my case, I will be installing it in my Void Linux system so I will be using XBPS.
 
## bspc: The Universal Controller for bspwm
 
In order to use bspwm we only need to interact with one program: bspc. It is a powerful utility that can control and configure bspwm’s behavior. In fact, all of the commands that we will be using to manipulate windows and configure its behavior are just bspc commands.
 
### Preparing the Configuration File for bspwm
 
To start configuring bspwm, we need to first create a configuration file. This is where bspwm will look for the bspc commands that it will execute when it first runs. By default, bspwm will look for the “/home/$USER/.config/bspwm/bspwmrc” file. To create that file you can type:
 
This command will create the bspwm folder in “/home/$USER/.config/” and also create the bspwmrc file within that folder.
 
Now, the bspwmrc file can be written in any language that you want as long as it is executable. This means that we would first need to set its file properties to be such. We can do this by typing the following:
 
This will make sure that we and anyone in our usergroup can execute this file.
 
After that, we can now open the bspwmrc file. In my case, I will be using vim to edit my configuration file. To do that I will type the following:
 
This will open an empty file and we can now start writing our configuration.
 
### Configuring bspwm
 
A basic configuration for bspwm looks something like this:
 
As indicated by the shebang in the first line, this configuration is written in Bash. The first few commands are the programs that I wanted to run before setting any configurations for bspwm.
 
The first one, xsetroot, changes the default X cursor to the more familiar left pointer. The second one initializes our hotkey daemon in the background.
 
### bspc config and bspc rule
 
The following commands in the configuration are specific to bspc. bspc config deals with the general configuration of the window manager. It includes both aesthetic and functional settings.
 
- border_width determines the thickness, in pixels, of the border width of the windows.window_gap deals with the amount of gaps, in pixels, around windows.split_ratio determines the ratio between the two leaf nodes when split.focus_follows_pointer sets whether the mouse pointer can control which window gets focus.pointer_modifier determines the keyboard key to resize the windows using the mouse.automatic_scheme determines the layout of the windows when split in automatic mode.

 
bspc rule, on the other hand, deals with the behavior of programs when opened in bspwm.
 
- The first rule in our example configuration forces Chromium to run in the second desktop.The second rule in our example forces Gimp to run in the eighth desktop. It also forces Gimp to run in a floating state rather than the default tiled. Lastly, it forces the window focus on Gimp when it loads.

 
With that, we now have a basic configuration for bspwm. It is important to note, however, that the options for bspc config and bpsc rule is extensive. If you want to know more about fine tuning your bspwmrc, you can check the Github Github documentation to have a full list of all the possible settings.
 
## sxhkd: The Keybinding Utility for bspwm
 
sxhkd is a simple program. It listens for keyboard input events and executes commands based on the keys you have pressed. It can deal with multi-key inputs through chording and it has an intuitive configuration file that is simple and easy to understand.
 
### Preparing the Configuration File for sxhkd
 
Preparing the configuration file for sxhkd is similar to setting up the bspwmrc file. First, we need to create the configuration folder and file for sxhkd. We can do this by typing the following command:
 
We, then, need to set the sxhkdrc file to be executable:
 
Once done, we now have our sxhkd configuration file to insert all of our keybindings.
 
### Configuring sxhkd
 
sxhkd recognizes keybindings in a specific pattern. It first asks for a modifier key. This can either be Alt, Super, Hyper or Control. After that, you need to provide a normal key to complement your modifier key. It can, then, be combined to be a keybinding by adding a “+” sign in between those two keys.
 
Therefore, the general form for an sxhkd keybinding looks like this:
 
Once done, you need to press Enter and Tab to create an indented line beneath the keybinding. After that, you need to specify the command that you want to execute when the keybinding is pressed.
 
An example configuration file for sxhkd looks something like this:
 
### Explaining the Keybinding Syntax
 
As we have discussed above, the keybinding syntax for sxhkd is relatively simple. Further, sxhkd can group keybindings together and it can execute branching commands through the use of key chording.
 
For example, a number of commands in this configuration makes use of the curly braces. This allows us to assign multiple functions on similar keybinds. Consider this command in the configuration:
 
This command deals with the closing and restarting of bspwm. The curly braces in the keybinding matches the curly braces that we have in the command line. Therefore, when we press Alt + Shift + Q in the keyboard the command: bspc quit gets executed. However, pressing Alt + Shift + R will execute bspc wm -r.
 
We can also bypass the need to provide additional keys when branching. Consider this example:
 
This command deals with the spawning of the terminal. It also swaps windows in the desktop. I can do the first command by pressing Alt + Enter and I can do the second command by pressing Alt + Shift + Enter. 
 
This is because the underscore character acts as a pass-through for keybindings. This allows us to have a default keybinding for a command but also have a “modified” keybinding for other commands.
 
Lastly, sxhkd is not limited to a single branching. Consider this example:
 
This command deals with the switching of the desktops. It also manages the movement of the windows within those desktops. The first command is executed when you press Alt + 1–0 while the second one is done with the Shift modifier key. 
 
In this, we used two curly braces to set the pass-through key and the numbers for the desktops. These two options then correspond to the two curly braces in the command below it.
 
## Finalizing the Installation
 
With that, we now have a basic understanding of configuring bspwm and sxhkd. The last thing that we need to do is to enable bspwm as our window manager. You can do this directly through Xorg or through your display manager.
 
### Running bspwm using xinitrc
 
The easiest way to initialize bspwm is to append it in your .xinitrc file. If you are using a minimal Linux distribution this is probably the method that you are already using to load a window manager.
 
To do this, you only need to append the following on the last line of your .xinitrc:
 
### Running bspwm using a Display Manager
 
However, if you are using a full-featured desktop such as Linux Mint or Ubuntu you might need to select bspwm in your login screen.
 
For example, in my Ubuntu installation I have to click on the gear icon on the login screen and select bspwm from the context menu to load it.
 
Congratulations! You now have a working installation of bspwm. You can now further customize your desktop by tweaking your configuration files and installing third-party docks. Here are some customized desktops to inspire you.
 
## Frequently Asked Questions
 
### 1. Why is my screen black when I logged in for the first time?
 
It is probably because you have not set a desktop background yet. This is often the case if you are running a minimal installation. You can change your background theme by using an image viewer program such as feh.
 
### 2. Why are my keybindings not working?
 
This is most probably due to two things:
 
- The keybindings did not load because sxhkd is not running.There was a syntax error with sxhkdrc. The most common mistake made with configuring sxhkd is with the indents. To initialize the commands properly, you must insert Tab-spaces in the indented lines.

 
### 3. When I logged in to my system it just returned me to the system prompt.
 
This can be due to a number of things. However, the most common cause is with an issue with the .xinitrc file. You need to make sure that bspwm is the last program that Xorg loads and that it is not running as a background process.
 
Ramces is a technology writer that lived with computers all his life. A prolific reader and a student of Anthropology, he is an eccentric character that writes articles about Linux and anything *nix.
 
Our latest tutorials delivered straight to your inbox




