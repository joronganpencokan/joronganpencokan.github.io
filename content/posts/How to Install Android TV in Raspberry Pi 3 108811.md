---
title: "Transform your Raspberry Pi 3 into an Android TV in minutes with this simple hack!"
ShowToc: true 
date: "2023-06-21"
author: "Stacy James"
---
*****
Transform Your Raspberry Pi 3 into an Android TV in Minutes with this Simple Hack!

Are you looking for a budget-friendly way to stream your favorite TV shows and movies without paying hefty subscription fees? If yes, then you are in the right place. The Raspberry Pi 3 is a small yet powerful single-board computer that has the ability to run a variety of operating systems. One of its most popular uses is as a media center or home theater PC (HTPC), thanks to its HDMI output and support for popular media center software like Kodi.

In this article, we will guide you through the steps to transform your Raspberry Pi 3 into an Android TV in minutes with this simple hack. By the end of the process, you will have a fully functioning Android TV that can stream your favorite TV shows, movies, and games right from your Raspberry Pi 3.

Here's what you'll need:

1. Raspberry Pi 3.
2. TV or monitor with HDMI input.
3. Micro-SD card (minimum 16GB).
4. Micro-SD card reader.
5. USB Keyboard and Mouse.
6. Power supply.
7. Android TV OS, like LineageOS.

Step 1: Download and Install the Required Software

The first thing you need to do is download the Android TV OS image file from a trusted source like LineageOS. Once downloaded, extract the compressed file and locate the Raspberry Pi 3 image. Next, you need to flash the image to your micro-SD card using a tool like BalenaEtcher. Once the image is flashed, insert the micro-SD card into your Raspberry Pi 3.

Step 2: Connect Your Hardware

Now you need to connect your Raspberry Pi 3 to your TV or monitor using an HDMI cable. Plug in your USB keyboard and mouse too. Finally, connect the power supply to your Raspberry Pi 3, and switch on your TV or monitor.

Step 3: Configure Your Android TV Setup

Once you have connected all the hardware, you will be greeted with the Android TV setup wizard. Follow the on-screen instructions to select your language, connect to Wi-Fi, and set up your Google account. After the setup is complete, you can tweak your Android TV settings like display resolution, audio output, and more.

Step 4: Install Your Favorite Apps

Now that you have set up your Android TV, it's time to install your favorite apps. You can download Android TV compatible apps from the Google Play Store, such as Netflix, Hulu, and Amazon Prime Video. You can also download games and other apps as needed.

Step 5: Enjoy Your Android TV

That's it! You have successfully transformed your Raspberry Pi 3 into an Android TV in minutes with this simple hack. Now you can enjoy your favorite TV shows, movies, games, and apps on your Raspberry Pi 3-powered Android TV.

Wrap-Up

In conclusion, the Raspberry Pi 3 is a versatile single-board computer that can be used for a variety of purposes, including as a media center or HTPC. By installing Android TV on your Raspberry Pi 3, you can enjoy all the benefits of an Android TV without having to spend a lot of money on expensive hardware. So, follow the above steps, and transform your Raspberry Pi 3 into a fully functioning Android TV in minutes.

{{< youtube K9fgJ5B9WGw >}} 



There are several Raspberry Pi models out there, and the latest Raspberry Pi 3 is the best of them all. It comes with a Wifi and Bluetooth adapter and a 64-bit CPU that makes it one of the best and affordable mini computers around. There are tons of things that you can do with a Raspberry Pi, but with a specs like this it is really great to be able to use it as a TV box. In this article we will show you how to install Android TV in Raspberry Pi 3.
 
Note: this article will show you the installation instructions in Linux, but the same steps are applicable for Windows and Mac OS X, too. Also, note that the Android TV build that we are using is not stable, and some of the apps might not work properly.
 
## Things you need
 
Obviously, you will need a Raspberry Pi 3. You will also need a micro SD card (preferably class 10) with a minimum 8 GB.
 
## Install Android TV in Raspberry Pi
 
We will make use of the Android TV image created by “Geek Till it Hertz.”
 
1. Go to the “Geek Till it Hertz” website, and download the ‘img.bz2″ file.
 

 
2. Extract the image. You should now have a “atvrpi320160530.img” file. (The filename might change if the developer updates the build, but it should still end with an .img extension.)
 
3. Insert your micro SD card into your computer. (You will need an SD card USB adaptor if your computer doesn’t come with a micro SD card slot.)
 
4. Open a terminal. Type the following command to find out the location of the micro SD card:
 
It should be in the “/dev/sdX” format. In this case my micro SD card is in the “/dev/sdc” slot.
 
Note: If your micro SD card is not in the FAT32 format, you will need to format it to FAT32 format. You can do that using the gParted tool. Also, back up the content in your SD card, as that will be wiped clean in the following step.
 
4. Run the following command to install the image to the SD card:
 
Replace “/location/to/androidtv-image-file.img” with the actual location of the Android TV image you downloaded earlier. Also replace “sdX” with the actual location of your micro SD card. In my case the command is as follows:
 
This will take some time. Sit back and enjoy your coffee.
 
5. Once it is done, unmount the SD card, plug it into the Raspberry Pi and boot it up. You should see your Android TV booting up.
 
## Available GUI tool to burn an img file to a USB drive
 
If you prefer not to deal with the command line or are a Windows user, here are some GUI tools you can use to burn the img file to a USB drive (micro SD card).
 
- Linux – Etcher
 - Windows – Win32 Disk Imager

 
## Android TV configuration
 
It is best to connect a keyboard and mouse to your Raspberry Pi so you can navigate around in the home screen. On the first boot up you will see that there is nothing on the home screen except for the “Settings” and “Network Settings” icons. The first thing you want to do is connect your Android TV to the Internet.
 
Using your keyboard arrow key (The mouse click doesn’t seem to work for me.), navigate to the “Network Settings” icon and press Enter.
 
From there select “Wifi” and turn it on. It will then scan for an existing Wifi network. Select your local network and connect to it.
 
Once it is connected, you will need to identify the IP address of your network connection (for sideloading apps).
 
Select your connected network, press Enter and select “status info.”
 
Write down the IP address. In my case it was 192.168.1.8.
 
You can continue to navigate around the different settings, but it is mostly empty for now. To install apps you will have to go to “Settings -> Security & restrictions” and enable “Unknown sources.”
 
## Sideloading apps to your Android TV from another Android phone/tablet
 
You will notice that there aren’t any apps installed on your Android TV, and there is no App Store for you to find and install new apps. For this we will need to sideload an App store app so that you can start installing other apps. In this instance Google Play store is not well supported in this Android TV build, so we will use Aptoide app store instead.
 
You will need to have another Android device to sideload apps to your Raspberry Pi.
 
1. On your Android phone go to the Aptoide site, and download the Aptoide TV apk. Alternatively, you can download the main Aptoide App Store apk instead of the Aptoide TV app.
 
2. Once the apk file is downloaded, go to Play Store and install the Apps2Fire app. (Any other apps that can sideload to Kindle Fire will work as well.)
 
3. Launch the Apps2Fire app. Slide the screen to the last “SETUP” page. Enter the IP address of the Raspberry Pi and press “Save.”
 
4. With your Raspberry Pi still running, press the “Upload” button on the Apps2Fire app on your Android phone.
 
Select the Aptoide apk file that you downloaded earlier. Select “Install” when prompted.
 
If everything went well, you should see the “Aptoide” app on your Raspberry Pi home screen after a while.
 
That’s it. You can now run the Aptoide app and start installing other apps. I do recommend installing Es File Explorer so that you can navigate the file system and install the apk file directly.
 
## Conclusion
 
This Android TV build for Raspberry Pi is buggy at the moment and not every app will work. I tried it with several games and TV apps, and some of them work fine, while others have graphic and display issues. Your experience might differ. With the instructions above you will have a working Android TV on your Raspberry Pi; just don’t expect everything to work. Enjoy!
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




