---
title: "Unlock the Ultimate Hack: Access Your Raspberry Pi Remotely with Windows SSH!"
ShowToc: true 
date: "2023-04-01"
author: "Arlene Ford"
---
*****
# Unlock the Ultimate Hack: Access Your Raspberry Pi Remotely with Windows SSH!

The Raspberry Pi, a small and affordable computer board, has been a favorite among tech enthusiasts for years. With its versatility, it's used for all kinds of projects, from homemade game consoles to DIY surveillance systems.

But there's one thing that can make using a Raspberry Pi even better: remote access. By using the Secure Shell (SSH) protocol, you can control your Raspberry Pi from your Windows computer, even if you're not in the same room.

And the best part? It's easy to set up. All you need is a Raspberry Pi, a Windows computer, and an internet connection.

## Step 1: Enable SSH on Your Raspberry Pi

Before you can access your Raspberry Pi remotely, you need to enable the SSH server on it. You can do this by following these steps:

1. Open the Terminal on your Raspberry Pi.
2. Type in `sudo raspi-config` and hit Enter.
3. Use the arrow keys on your keyboard to navigate to "Interfacing Options" and press Enter.
4. Use the arrow keys to navigate to "SSH" and press Enter.
5. Select "Yes" to enable SSH.
6. Press Enter to save your changes.

## Step 2: Find Your Raspberry Pi's IP Address

To access your Raspberry Pi remotely, you'll need to know its IP address. You can find this by following these steps:

1. Open the Terminal on your Raspberry Pi.
2. Type in `hostname -I` and hit Enter.
3. Your Raspberry Pi's IP address should be displayed.

Make sure to write down your IP address for later use.

## Step 3: Download an SSH Client on Your Windows Computer

To access your Raspberry Pi remotely, you'll need an SSH client on your Windows computer. One of the most popular options is PuTTY, which you can download for free from the official website.

## Step 4: Connect to Your Raspberry Pi from Your Windows Computer

Now that you have enabled SSH on your Raspberry Pi and have the IP address and an SSH client on your Windows computer, it's time to connect to your Raspberry Pi. Follow these steps to do so:

1. Open PuTTY on your Windows computer.
2. Enter your Raspberry Pi's IP address in the "Host Name" field.
3. Make sure the "SSH" radio button is selected.
4. Click "Open" to start the connection.
5. When prompted, enter your Raspberry Pi's username and password.

And voila! You're now connected to your Raspberry Pi remotely from your Windows computer.

## Conclusion

Accessing your Raspberry Pi remotely unlocks a whole new world of possibilities. By using the SSH protocol, you can control your Raspberry Pi from anywhere, making it more versatile and convenient than ever before. And with just a few easy steps, you can get started on this ultimate hack.

{{< youtube gsvS2M5knOw >}} 



Maybe you’ve gotten bored of repeatedly jamming a cable on that HDMI port. Or perhaps you’ve broken the port already. Either way, you can use the Raspberry Pi even without a monitor, thanks to SSH. That’s called a “headless computer,” and it’s a lifesaver that makes many things easier.
 
## What’s a Headless Computer?
 
A headless computer is a computer without a monitor. The computer can be anything – it doesn’t even have to be a Raspberry Pi. To give an example, the web server that lets you access this webpage from any part of the world is probably a headless computer from some data facility.
 
Headless computers can be controlled through different means. Some listen to a webpage to receive commands, while others let you remotely connect and control them via commands on a console. This time, we are doing the latter.
 
## Turn Your Raspberry Pi into a Headless Computer
 
We are splitting this up into three parts. The first one is for downloading PuTTY for Windows, the second for preparing the Raspberry Pi for SSH, and the last for logging in to the Raspberry Pi through Windows via SSH.
 
### Download PuTTY for Windows
 
- Download the x86 version of PuTTY. If you are unsure of your Windows PC’s architecture, the safe bet is to download the 32-bit version, as it can run on both 32- and 64-bit systems. Download the 64-bit version only if you’re sure that you’re using a 64-bit system.

 
- Run the installer and finish the installation wizard.

 
- After finishing the wizard, set that aside and configure the Raspberry Pi to allow SSH.

 
### Prepare Your Raspberry Pi
 
These instructions assume that your Raspberry Pi has already been set up with Raspberry Pi OS.
 
- Power up your Raspberry Pi (with a monitor, of course), then click the Raspberry Pi Icon, followed by “Preferences -> Raspberry Pi Configuration.”

 
- When a new window opens, move to the “Interfaces” tab, then enable the “SSH” option.

 
- Check whether your Raspberry Pi is connected to your Wi-Fi router. If not, click on the Network icon, followed by your Wi-Fi network name.

 
- If you click on your Wi-Fi network name, a new window will pop up. This will ask you for your Wi-Fi password. Skip this step if you’re already connected to your Wi-Fi network.

 
- Open the terminal and type ifconfig. You’ll find a list of information about your Raspberry Pi’s network connections. Look for “wlan0,” then copy the IP address next to “inet” for the next step.

 
### Log in via SSH
 
- Open the PuTTY app in Windows, then type the IP address into the box that says “Host Name (or IP address).” Keep the port at 22. Make sure that the “Connection type” is set to SSH, then click “Open.”

 
- You will be greeted with a security alert, warning you about connecting to an unknown host. Click “Accept.”

 
- You will see a login prompt. By default, your Raspberry Pi should have “pi” as its username. The default password is “raspberry.”

 
- With all of that done, you are ready to use PuTTY to control your Raspberry Pi via SSH!

 
## What Can You Do with Your Headless Raspberry Pi
 
Now that you know how to access the terminal on your Raspberry Pi through Windows via SSH, you need to know how to do stuff with it.
 
You have to remember that the Raspberry Pi OS is based on the Debian distro for Linux, so you can use Linux terminal commands on the PuTTY terminal when doing most actions.
 
However, that only works if you have the Raspberry Pi OS on your Raspberry Pi. It won’t work if you have something else on your system, like Windows 11.
 
## Important Linux Terminal Commands
 
Given all that, there are some commands you have to know if you’re not used to doing stuff on the Linux terminal yet. The following are a few codes you might want to know.
 
- Turn off computer: sudo shutdown -h now Reboot computer: sudo reboot -h nowChange directories: cd <path> List files and directories: dir or ls

 
Without a file explorer to click on, you’re left to type where you want to go on the terminal window. Use cd to change directories and dir to show what’s inside the current directory.
 
Reading a little bit deeper into the Linux virtual directory structure might help you better understand how cd works.
 
- Making new folders: mkdir <folder name>Using a text editor: nano <filename>

 
nanois perhaps the simplest text editor out there and lets you write text files and programming scripts on the go. While it’s not an IDE that can compile code for you, it’s good enough when you’re just doodling with coding ideas.
 
- Deleting files and folders: rm <file or folder name>

 
Check out this article for more details on deleting files in Linux.
 
- Installing packages: sudo apt <install or uninstall> <package 1> <package 2>

 
Typically, this command is used to install or uninstall one or more packages. For instance, you can install the Python 3 package for controlling the Raspberry Pi’s GPIO pins by typing sudo apt-get install python3-rpi.gpio.
 
You may want to learn more about apt if you want to do more software-related things on the Raspberry Pi.
 
## Frequently Asked Questions
 
Image credit: close-up of raspberry pi pico by 123RF 
 
### What happens if I cd into a nonexisting directory?
 
If you try using the cd command to go to a non-existing directory, the terminal will return “No such file or directory” and not do anything else.
 
### What should I do when I make a typo while typing the password?
 
If you make a typo, use backspace to delete the last character you typed. Alternatively, use <- and -> along with Home and End to navigate between characters or  Ctrl + A to select everything, then press Delete or Backspace to remove it all, which is useful if you don’t know which character was wrong.
 
### Why is there a warning message when I shut off my Raspberry Pi?
 
When you shut it down, PuTTY only knows that it suddenly lost its connection with the Raspberry Pi. It doesn’t know if it shut itself down or got disconnected from the network. Hence, a “Fatal Error” warning message should show up after you enter sudo shutdown -h now on the terminal. The same should also work for all of its other variants, like the commands for rebooting.
 
Terenz is a hobbyist roboticist trying to build the most awesome robot the world has ever seen. He could have done that already if he wasn't so busy burning through LEDs as a second hobby.
 
Our latest tutorials delivered straight to your inbox




