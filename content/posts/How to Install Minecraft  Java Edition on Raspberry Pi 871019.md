---
title: "You Won't Believe How Easy it is to Install Minecraft Java Edition on Your Raspberry Pi!"
ShowToc: true 
date: "2022-12-29"
author: "Pamela Mcreynolds"
---
*****
# You Won't Believe How Easy it is to Install Minecraft Java Edition on Your Raspberry Pi!

If you're looking for a fun way to pass the time, Minecraft is an excellent option. It's a game that's been around for over a decade, but its charm hasn't diminished even a bit.

If you're a Raspberry Pi user, you might be wondering if you can install Minecraft on your device. The good news is, yes, you can! In this article, we'll walk you through the simple steps to install Minecraft Java Edition on your Raspberry Pi.

## Requirements

Before jumping into the installation process, you need to ensure you have the following:

1. Raspberry Pi with Raspbian or Raspberry Pi OS installed.
2. A monitor, keyboard, and mouse for your Raspberry Pi.
3. A stable internet connection.
4. An official Minecraft account.

If you don't have a Minecraft account, you can buy one on the official website. Once you have these items, you're ready to install Minecraft Java Edition on your Raspberry Pi.

## Installation Steps

1. Open the terminal window on your Raspberry Pi by click the "terminal" icon on the taskbar.

2. Run the following command: `sudo apt-get update`.

3. Once the update is complete, run this command: `sudo apt-get install openjdk-8-jdk`.

4. After successful installation, download Minecraft from the official website.

5. Once the download is complete, go to the directory where the downloaded file is saved.

6. Unzip the file by running this command: `unzip minecraft.zip`.

7. Change the directory to the Minecraft directory by running this command: `cd minecraft-launcher*`.

8. Finally, run the Minecraft launcher by running this command: `./minecraft-launcher` .

9. Enter your Minecraft login credentials to access the game.

Congratulations! You have successfully installed Minecraft Java Edition on your Raspberry Pi. You can now enjoy endless hours of entertainment on your device.

## Conclusion

Installing Minecraft on your Raspberry Pi is easy and straightforward. With a little bit of technical know-how, you can enjoy the game on your device in just a few simple steps. So what are you waiting for? Go ahead and start playing!

{{< youtube oqNWJ52DLes >}} 



Today, there’s a version of Minecraft for pretty much every major platform – Java Edition for Windows, Education Edition for the iPad, Bedrock Edition for gaming consoles such as Nintendo Switch and PlayStation 4, and Pi Edition for the Raspberry Pi.
 
Minecraft: Pi Edition is based on an old version of Pocket Edition, with a few features removed to help it run more smoothly on the Raspberry Pi. Pi Edition is free to download and easy to install, but it doesn’t provide the complete Minecraft experience.
 
Wouldn’t you prefer to have the “full” version of Minecraft on your Raspberry Pi? You’ll learn in this article how to get Minecraft: Java Edition 1.14.4 running on Raspberry Pi 4. By following along, you can turn your Raspberry Pi into a portable Minecraft game that you can attach to any compatible screen or monitor.
 
## What you’ll need
 
To complete this tutorial, you’ll need:
 
- Raspberry Pi 4SD cardLaptop or computer to download the Gentoo operating systemRaspberry Pi 4-compatible power cableExternal keyboard and way to attach it to your Raspberry PiMicro HDMI cableExternal monitorEthernet cable or Wi-Fi connectionMinecraft Java Edition

 
Now that you’ve assembled your tools, let’s install Minecraft: Java Edition on the Raspberry Pi.
 
## Install the Gentoo operating system
 
This tutorial uses the Gentoo operating system, though the instructions should work for any Linux distro.
 
1. Gentoo will be flashed using Etcher, so if you haven’t already installed Etcher, download the latest version now.
 
2. On your computer or laptop, head over to Gentoo’s GitHub repository.
 
3. Scroll to “Raspberry Pi 4B, 3B/B+ 64-bit Full” and download the “genpi64.img.xz” file.
 
4. Insert your SD card.
 
5. Launch the Etcher application.
 
6. In Etcher, click “Select image” and then select the Gentoo file you just downloaded.
 
7. Click “Select target” and then choose your target boot medium, which in this instance is our SD card.
 
Etcher will now flash the system image to your SD card.
 
### Start up your Raspberry Pi: booting into Gentoo
 
You’re now ready to start your Raspberry Pi:
 
8. Remove the SD card from your laptop or computer and insert it into your Raspberry Pi.
 
9. Attach your monitor to the Raspberry Pi using the micro HDMI cable.
 
10. Attach your keyboard to the Raspberry Pi device.
 
11. Plug your Raspberry Pi into a power source. The device should boot automatically into the standard Gentoo desktop.
 
12. If you’re connecting to Wi-Fi, select the “Network” icon in the Gentoo toolbar and then select your Wi-Fi network.
 
13. Enter your password.
 
Now that Gentoo is installed and you’re connected to your local network, you’re ready to install Minecraft: Java Edition.
 
## Fetch the setup script
 
The first step is retrieving the setup script and replacing it with the Minecraft launcher. Toward the bottom of the Gentoo desktop, find the “Terminal” icon and give it a click.
 
Next, create a new Minecraft directory:
 
Point the Terminal at this new directory:
 
We can now fetch the setup script, run it, and replace the Minecraft launcher by running each of the following commands in turn:
 
This process may take a while, so why not grab yourself a coffee or a snack while you’re waiting?
 
## Start the Minecraft Launcher
 
Once the Terminal has executed all of your commands, you can start the Minecraft Launcher:
 
Enter your Minecraft username and password and then click “Log in.”
 
On the subsequent screen, click the “Edit Profile” button.
 
Open the “Use version” drop-down and select “1.14.4.” Note that you must select this specific version for Minecraft to run correctly on your Raspberry Pi.
 
Click “Save profile,” which will take you back to the main Minecraft Launcher screen. Click the “Play” button.
 
The Launcher will download everything it needs to install Minecraft – and then promptly crash. Don’t panic! We can resolve this issue by installing OptiFine.
 
## Install the OptiFine Minecraft mod
 
OptiFine is a Minecraft utility mod that optimizes the game’s graphics. It can deliver a performance boost, which is essential when you’re trying to run Minecraft on the Raspberry Pi!
 
To install OptiFine, run the following Terminal command:
 
When prompted, click “Install.”
 
After a few moments, you should receive a notification that OptiFine has been installed successfully. Click “OK.”
 
## Enter your Minecraft login details
 
Next, the “runmc1_14_4_optifinef3.sh” file needs to be opened, and your Minecraft username and password needs to be entered, as well as the email address that’s associated with your Minecraft account.
 
To open this file, run the following Terminal command:
 
This file should now open in a new window, ready for you to edit. 
 
Scroll to the following section:
 
Replace these placeholder credentials with your own information, making sure to surround your email address, password and username with quotation marks. For example:
 
Save your changes by selecting “File -> Save.”
 
Since this file now contains your Minecraft credentials in plain text, you need to run “chmod 0700” so that other people cannot read, write or execute your login details. In the Terminal, run the following command:
 
Your Minecraft credentials will now be protected against prying eyes.
 
## Launch Minecraft: Java Edition
 
You’re now ready to run Minecraft! In the Terminal, enter:
 
Minecraft will now load.
 
Starting Minecraft for the first time can take a while, but after a few minutes you should see the login screen for Minecraft: Java Edition.
 
Before logging in to your account, you should tweak Minecraft’s settings to make the game easier for Raspberry Pi to process.
 
### Optimizing Minecraft for the Raspberry Pi
 
The Raspberry Pi doesn’t have the same firepower as a PC or computer, so running Minecraft: Java Edition on your Raspberry Pi can result in poor performance.
 
To avoid any potential lag, you should reduce the number of “chunks” that are visible at any one time. Less chunks means that your Raspberry Pi can render frames more quickly which will reduce lag and make Minecraft flow easier.
 
To reduce the render distance:
 
On the Minecraft login screen, select “Options … -> Video Settings … ”
 
Find “Render Distance” and reduce it to “3 chunks.”
 
Save your changes by clicking “Done.”
 
## Time to play Minecraft: Java Edition
 
You’re finally ready to play Minecraft: Java Edition on the Raspberry Pi! Navigate back to the main Minecraft launcher screen (if you aren’t there already) and click the “Singleplayer” button.
 
Now that you have completed this setup, you can launch Minecraft at any time by opening a Terminal and running the following commands:
 
There are many different ways you can use Raspberry Pi alongside Minecraft (including creating your own Minecraft server!). 
 
Have you created any interesting projects using Raspberry Pi and Minecraft? Let us know in the comments below!
 
Jessica Thornsby is a technical writer based in Derbyshire, UK. When she isn’t obsessing over all things tech, she enjoys researching her family tree, and spending far too much time with her house rabbits.
 
Our latest tutorials delivered straight to your inbox




