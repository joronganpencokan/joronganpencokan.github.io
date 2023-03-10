---
title: "You Won't Believe How Easy It Is To Make Your Own Chromecast With Raspberry Pi And Raspicast!"
ShowToc: true 
date: "2022-12-31"
author: "Willie Smith"
---
*****
Title: You Won't Believe How Easy It Is To Make Your Own Chromecast With Raspberry Pi And Raspicast!


Are you tired of paying the monthly subscription fee for your streaming device? Do you want to save some money and make your own Chromecast? If yes, then you are in the right place. In this article, we will show you how easy it is to make your own Chromecast with Raspberry Pi and Raspicast.

Before we begin, let's break down what a Chromecast is. As Google puts it, Chromecast is a smart TV dongle that plugs into the HDMI port on your television. It allows you to stream content from your smartphone, tablet, and computer to your TV. The device is affordable and simple to use, making it one of the most popular streaming devices in the world.

Now, let's move on to the fun part: making your own Chromecast. Raspberry Pi is a tiny computer that you can use for a variety of projects, and we will use it to create our Chromecast. Here are the things you will need:

- Raspberry Pi (any version will work)
- MicroSD card (at least 8 GB)
- Power adapter
- HDMI cable
- Ethernet cable or Wi-Fi dongle
- USB keyboard and mouse

Once you have all the necessary equipment, follow these steps:

Step 1: Install Raspbian

Raspbian is a free operating system based on Debian that is optimized for the Raspberry Pi. You can download the latest version of Raspbian from the official Raspberry Pi website. Install it on your MicroSD card using any SD card imaging software such as BalenaEtcher or Win32DiskImager.

Step 2: Establish Internet Connection

Once you have installed Raspbian, connect your Raspberry Pi to the internet. You can either use an Ethernet cable or connect it using a Wi-Fi dongle. Make sure the internet connection is stable, and you have a working browser.

Step 3: Install Raspicast

Raspicast is a free app that you can use to stream content to your TV. It is designed for the Raspberry Pi and supports multiple streaming services. To install Raspicast, open the Terminal and enter the following command:

```
sudo apt-get update
sudo apt-get install raspicast
```

Step 4: Start Streaming

Once you have installed Raspicast, you can start streaming content. Open Raspicast from the start menu, and you will see a QR code. Scan the code using your smartphone or tablet to establish a connection between your device and Raspicast.

Now, open any app that supports Chromecast streaming such as Netflix, YouTube, or Twitch. Look for the Chromecast icon, and you should see Raspicast listed. Click on it, and your content will start streaming on your TV.

Congratulations! You now have your own Chromecast, and you saved some money.

Conclusion

Making your own Chromecast is easy, and it won't cost you too much. Raspberry Pi is an affordable computer that is perfect for DIY projects. With Raspicast, you can stream content from your smartphone, tablet, or computer to your TV just like a real Chromecast. So, what are you waiting for? Give it a try and enjoy the benefits of streaming without paying the monthly subscription fee.

{{< youtube -VL1LDdJKuc >}} 



Google’s Chromecast is one of the most popular streaming devices on the market – and it’s easy to see why! Just plug your Chromecast dongle into an HDMI port on any compatible TV, monitor or projector, and you’re ready to start enjoying your content on the big screen.
 
But what if you don’t want to invest in a Chromecast? 
 
You can set up your Raspberry Pi to act as an inexpensive Chromecast-style streaming device. Although you can’t implement the same protocols as Chromecast, you can get very similar end-results.
 
You’ll learn in this tutorial how to turn your Raspberry Pi into a Chromecast alternative, using the free Raspicast software and the Raspicast for Android mobile app. 
 
## What you’ll need
 
To complete this tutorial, you’ll need:
 
- Raspberry Pi running Raspbian. If you don’t have it, grab the latest version and flash it to an SD card using Etcher Raspberry Pi-compatible power cableExternal keyboard and a way to attach it to your Raspberry PiHDMI or micro HDMI cable, depending on your model of Raspberry PiExternal monitorEthernet cable or Wi-Fi connection Android smartphone or tablet. Currently, the Raspicast mobile app isn’t available for iOS.

 
After completing this tutorial, you can attach your Raspberry Pi to a TV, projector, or any screen that has a compatible port, but this step is optional. 
 
## Raspbian: check for the latest version
 
Before starting, make sure you’re running the latest version of Raspbian.
 
Connect your Raspberry Pi to a power supply to boot it up. Once it’s booted, click the “Terminal” icon in the toolbar.
 
Type the following into the Terminal window, then hit Enter.
 
If Raspbian installs any updates, then you’ll need to reboot your Raspberry Pi using the following Terminal command:
 
Once your Raspberry Pi has rebooted, you’re ready to move on to the next stage. 
 
## Install Git, Make, OMXPlayer and OpenMax
 
This tutorial uses GIT and Make. These packages should be bundled with Raspbian, but since they’re essential for Raspicast, you need to make sure they’re installed:
 
Next, check that OMXPlayer is installed, as this command line player will be responsible for processing all the audio or video content casted to Raspicast:
 
OMXPlayer can only process audio and video content; it cannot process static images. Next, install the OpenMax Image Viewer, which is a GPU-accelerated image viewer designed specifically for Raspberry Pi.
 
To start, clone OpenMax’s GitHub repository:
 
Next, download libjpeg8-dev and libpng12-dev, which are development libraries for images in PNG and JPEG format:
 
Switch to the folder where the OpenMax GitHub repository was cloned using the “change directory” (cd) command: 
 
Build the OpenMax source code into an executable program:
 
Once Make has finished compiling the OpenMax code, you’re ready to install it: 
 
The OpenMax Image Viewer is now running on your Raspberry Pi.
 
## Allow remote connections: enabling SSH 
 
You can use Raspicast to project any image, video or audio file from your Android device to your Raspberry Pi. This casting happens wirelessly, so you need to ensure your Raspberry Pi is set up to receive remote connections.
 
For security purposes, SSH (Secure Shell) is disabled by default on Raspbian. If you’re ever going to cast to your Raspberry Pi, then you need to enable SSH:
 
1. In the toolbar, select the Raspberry Pi icon.
 
2. Navigate to “Preferences -> Raspberry Pi Configuration.”
 
3. Select the “Interfaces” tab. 
 
4. Find “SSH” and then select its accompanying “Enabled” radio button. 
 
5. Save your changes by clicking “OK.” 
 
6. Reboot by selecting the Raspberry Pi logo in the toolbar and then navigating to “Shutdown -> Reboot.”
 
When your Raspberry Pi reboots, SSH will be enabled. 
 
## Cast from your Android device to your Raspberry Pi 
 
Next, you need to install the Raspicast mobile app on your Android smartphone or table. After installing this app, you’ll be able to cast any compatible image, video or audio file from your Android smartphone or tablet to your Raspberry Pi.
 
1. Download the free Raspicast app to your Android device. 
 
2. Launch the application.
 
3. When prompted for a “hostname,” enter your Raspberry Pi’s IP address. If you don’t already have this information, then you can retrieve it by opening a Terminal on your Raspberry Pi and running the following command: hostname -I
 
4. Enter your Raspberry Pi’s username and password. Raspbian’s default username is “pi,” and the default password is “raspberry.”
 
5. Tap “ OK.”
 
6. To cast any video, image or audio file, simply tap “Cast.” 
 
7. This file will now be cast to your Raspberry Pi.
 
Your chosen content will appear on any monitor or screen that’s attached to your Raspberry Pi, so now that you have Raspicast set up, you’re free to attach your Raspberry Pi to any compatible screen. Many apps and websites also support Raspicast, so if there’s a piece of media that you want to cast, then it’s always worth tapping “Share” and checking whether Raspicast is listed as an option.
 
Hopefully, you can now enjoy your favorite videos and photos on your widescreen TV. You can add more to the fun by installing Kodi and Netflix to Raspberry Pi or even a Plex server. With Raspberry Pi, you are spoilt for choices.
 
Jessica Thornsby is a technical writer based in Derbyshire, UK. When she isn’t obsessing over all things tech, she enjoys researching her family tree, and spending far too much time with her house rabbits.
 
Our latest tutorials delivered straight to your inbox




