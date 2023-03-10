---
title: "Unlock the Full Potential of Your Raspberry Pi with Windows 10 - Step-by-Step Installation Guide Inside!"
ShowToc: true 
date: "2023-02-18"
author: "David Mooney"
---
*****
# Unlock the Full Potential of Your Raspberry Pi with Windows 10 - Step-by-Step Installation Guide Inside!

Are you looking for a way to unlock the full potential of your Raspberry Pi? Have you ever considered using Windows 10 as your operating system? With the help of this step-by-step installation guide, you can easily install Windows 10 on your Raspberry Pi and reap all the benefits it has to offer. 

## Why Windows 10?

Raspberry Pi is a great platform for experimenting and learning about computer programming and electronics. However, the default Raspbian operating system may not be suitable for all types of projects. Windows 10 is a popular choice because of its compatibility with various software and hardware components. It also offers a user-friendly interface that is familiar to millions of PC users around the world. 

## Requirements

Before you begin the installation process, make sure you have the following:

- A Raspberry Pi 3 Model B, 3 Model B+, or a Compute Module 3
- A 16GB or larger microSD card
- A computer running Windows 10, version 1703 or later
- A USB mouse and keyboard
- A micro-USB power adapter

## Step-by-Step Installation Guide

1. Download the Windows 10 IoT Core dashboard from the Microsoft website and install it on your computer. This dashboard is a tool for managing your Raspberry Pi and installing the operating system.

2. Connect your Raspberry Pi to your computer using an Ethernet cable.

3. Insert the microSD card into your computer and format it using FAT32.

4. Open the Windows 10 IoT Core dashboard and click the "Set up a new device" button.

5. Select "Raspberry Pi 3" from the list of available devices and click the "Download and install" button.

6. Choose the directory where you want to save the image and click "Download" to begin the download process.

7. Once the download is complete, click the "Customize" button to configure your device.

8. Enter a name for your device and choose a language and region.

9. If you want to connect your device to Wi-Fi, click the "Connectivity" tab and enter your Wi-Fi network name and password.

10. Click "Create" to create the image file.

11. Connect your microSD card to your computer and select it from the list of available devices in the "Flash" tab of the Windows 10 IoT Core dashboard.

12. Click "Flash" to write the Windows 10 image to the microSD card.

13. Once the flashing process is complete, insert the microSD card into your Raspberry Pi.

14. Connect your USB mouse and keyboard to your Raspberry Pi.

15. Connect your Raspberry Pi to a power source using a micro-USB power adapter.

16. Wait for the device to boot up with Windows 10 IoT Core.

17. Congratulations! You have successfully installed Windows 10 on your Raspberry Pi.

## Conclusion

Windows 10 is a powerful operating system that can unlock the full potential of your Raspberry Pi. With its user-friendly interface and wide compatibility with software and hardware components, it is a great choice for a variety of projects. By following this step-by-step installation guide, you can easily install Windows 10 on your Raspberry Pi and begin exploring all the possibilities it has to offer.

{{< youtube lPbFcM1GJDs >}} 



Though the Raspberry Pi has been around for a few years, you’ve only really been able to install Linux, BSD and other ARM-based operating systems, never Microsoft Windows. This has changed with the release of Windows 10. Microsoft has stepped up and created a bare-bones edition just for the Pi.
 
Mac and Linux users: Though it is possible to flash an SD card image with these operating systems, Windows 10 IoT core requires a specific file that can only be found on Windows.
 
Note: though the Raspberry Pi 3 is now out and support for Windows 10 is coming, there is no option as of yet to install it via the IoT dashboard. This guide will be updated to include instructions for the Pi 3 when the time comes.
 
## Install Windows 10 on Your Main PC
 
Make sure you’re running the latest version of Windows 10 on the computer you’re using to make the SD card. This method will not work if you’re running Windows 7, 8, or even Windows 8.1. You can quickly download an ISO from Microsoft’s official Windows 10 download page.
 

 
Once you have it downloaded, either put a DVD in your optical drive and double-click on the ISO file to burn it, or follow these instructions to make a USB installation disk (follow these links for the Mac and Linux tutorials). In this tutorial, we are using Rufus to create the USB installer.
 
Go to the Rufus site, and when you’re on the page, just scroll down. You should see a download button. Click it and get the program. Once you’ve downloaded the program, launch it. Plug in a USB drive (no smaller than 4 gigabytes), and click on the disc icon. This will open a file dialog and prompt you to provide an ISO. Using this open file dialog, browse to where the Windows 10 ISO file is on your system, and click open.
 
Click the Start button to create the installation USB stick. When the USB stick is created, just configure your BIOS to boot from it, and go through the standard Windows setup process. Be sure to follow all the instructions that Microsoft provides very carefully.
 
## Install Windows 10 IoT Dashboard
 
After installing Windows 10 on your PC, it’s time to install the IoT dashboard for Windows 10. This is the program needed to create the SD card for your Raspberry Pi 2. There is currently no other way to install Windows on this device. Get the dashboard by following this link. On the page, click the button “Get IoT core Dashboard” to download it. The installer for this program will have instructions. Be sure to follow them carefully.
 
Microsoft has a lot of information regarding the Windows 10 IoT dashboard and what it can do for your Raspberry Pi. If you’re looking to use your Pi for development in Windows 10, head to this page to learn everything Microsoft has to say about IoT core and Raspberry Pi development.
 
## Installing Windows 10 IoT on the Raspberry Pi 2
 
Now that all the programs required are installed on your system, the SD card can finally be made. Get out the SD card you’re planning on installing Windows 10 to and insert it into the SD card reader on your Windows 10 desktop. Keep in mind the SD card must be at least 8 gigabyte in size and rated class 10 or better.
 
Launch the IoT core dashboard. Once launched, you’ll see a few things on screen in the form of three drop-down menus. Select Raspberry Pi 2 in the first drop-down menu, Windows 10 IoT core for Raspberry Pi 2 in the second, and the SD card you plan on using in the third.
 
When everything has been selected, click the box saying that you accept Microsoft’s terms and conditions, and select the download and install button.
 
What follows is the flashing process. You’ll see a progress bar pop up on screen and tell you that your SD card is being flashed. This may take a bit of time. Be patient.
 
Once the flashing has completed, another window will open. This window will partition the SD card in the correct way.
 
When the partitioning process has completed, the IoT dashboard will notify you that the SD card is ready.
 
Finally, just insert your SD card into the raspberry Pi, connect your peripherals, network cable, display and power it on. That’s it! You’re now running Windows 10 IoT on your Pi!
 
## Conclusion
 
Windows 10 IoT Core for the Raspberry Pi is a is a good start to a market that is almost exclusively dominated by Linux. Since this is Windows 10, it doesn’t have the same amount of community surrounding it and thus has less enthusiasm for its deployment on these types of hobby boards.
 
We can only hope that as Windows 10 IoT gets more adoption, the Pi community will come together and realize what a useful tool it is and has the potential to become.
 
Would you use Windows 10 on your Pi 2? Tell us why or why not below!
 
Derrik Diener is a freelance technology blogger.
 
Our latest tutorials delivered straight to your inbox




