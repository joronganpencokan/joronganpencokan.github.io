---
title: "Discover the Secret to Stream Your Favorite Videos on Android with VLC Shares in Ubuntu - Easy Step-by-Step Guide!"
ShowToc: true 
date: "2023-01-16"
author: "William Knight"
---
*****
Title: Discover the Secret to Stream Your Favorite Videos on Android with VLC Shares in Ubuntu - Easy Step-by-Step Guide!

Are you tired of missing out on your favorite movies or TV shows because your Android device doesn't support the format? Have you been looking for an easy way to stream your favorite videos directly from your Ubuntu system to your Android device? If so, you're in luck! With VLC Shares in Ubuntu, you can easily stream videos from your computer to your Android device, no matter the format. In this article, we'll show you how to do it step-by-step.

Step 1: Install VLC Media Player on Ubuntu
First, you'll need to install VLC Media Player on your Ubuntu system. To do this, open the terminal and type the following command:

sudo apt-get install vlc

Press Enter and wait for the installation process to complete.

Step 2: Set Up VLC Shares in Ubuntu
Once you have VLC installed, you need to set up the VLC Shares feature on your Ubuntu system. To do this, follow these steps:

1. Open VLC media player and navigate to the "View" menu.
2. Select "Add Interface" and then "Web".
3. Select "Show Settings" under the "Web" interface option.
4. You'll see an option for "Lua HTTP". Check it and set a password.
5. Go to the "General" tab and select "All" under "Interfaces".
6. Select "HTTP" and click on "Save".

Step 3: Share a Folder on Ubuntu
Now that you have the VLC Shares feature set up, it's time to share a folder or directory on your Ubuntu system. Follow these steps:

1. Create a folder that you want to share (e.g., ~/Videos).
2. Right-click on the folder and select "Properties".
3. Go to the "Local Network Share" tab and check the "Share this folder" box.
4. Click on the "Install Service" button to install the Samba service.

Step 4: Access the Shared Folder from Android
Now, it's time to access the shared folder from your Android device. To do this, follow these steps:

1. Download and install the VLC app on your Android device from the Google Play Store.
2. Open VLC and tap on the "Menu" icon.
3. Tap on "Local Network".
4. Tap on "Enter URL".
5. Type in the following: http://[IP address of Ubuntu system]:8080.
6. Enter the password that you set up earlier.
7. Tap "OK".

That's it! You can now select your shared folder from the VLC app on your Android device and start streaming your favorite videos from your Ubuntu system.

In conclusion, VLC Shares is a great feature that allows you to stream videos from your Ubuntu system to your Android device. With this step-by-step guide, you can set it up quickly and easily. So, what are you waiting for? Try it out and start enjoying your favorite videos on your Android device today!

{{< youtube r3Rq-1OIX4k >}} 



VLC, without a doubt, is the best media player around. Not only is it able to play almost any file format, it is also able to stream audio/video from the Web and transcode on the fly. VLC-share is a web implementation of VLC streaming and transcoding that allows you to stream (and transcode) your videos to your WII Media Center (WIIMC) or Android phone. Just think of airplay for Android and you get VLC-Shares.
 
In this tutorial, we will show you how to get VLC-shares up and running in your Ubuntu machine. VLC-shares is available for Windows as well and the installation and configuration instruction is pretty easy and straightforward, so we will not touch on that.

 
### Installing VLC-shares in Ubuntu
 
First of all, go to the VLC-shares website and download the “vlc-shares_0.5.*.zip” file. The latest version (as of this post) is version 0.5.3.
 
Extract the zip file to your Home folder. You should see a folder “vlc-shares”.
 
Open a terminal. We are going to install the necessary software.
 
Next, we are going to enable apache mod_rewrite
 
It will prompt you to restart apache. Ignore that for a moment. We will do that later.
 
Open Zend Framework config file:
 
Remove the “;” in front of the second sentence.
 

 
Save and close the file.
 
Back to your terminal, we are going to change the apache config file.
 
Scroll down the file until you see the part “<Directory /var/www/>“. Underneath that line of code, change AllowOverride None to AllowOverride All.
 
(Assuming you have earlier unpacked the vlc-shares.zip file to your Home folder) We are going to move the VLC-shares folder to the apache folder.
 
Lastly, we are going to restart the apache.
 
We are almost there. Now, open up a browser and navigate to “http://localhost/vlc-shares/public” (without the quote). You should see the installation dashboard. Go ahead to select all the plugins and click the “Start Installation” button.
 
The installation shouldn’t take more than a minute. Once it is done, you will see the configuration page. Ignore that (the default configuration should work fine). At the top, click the first Home icon. This will bring you to the Home page.
 
We are done with your Ubuntu installation. The next step is to configure your Android phone.
 
### Accessing VLC-shares from Android
 
Before we start the streaming, we need to install a media player app capable of playing stream video. I have tried out RockPlayer and MVideo Player and they failed. VPlayer is the one that works.
 
Install VPlayer from the market.
 
Note: If you have firewall installed, remember to configure it to allow incoming connection before proceeding.
 
If your Android phone is connected to the same WIFI network as your Ubuntu computer
 
Open the browser and enter the URL: http://your-ubuntu-lan-address/vlc-share/public. Replace “your-ubuntu-lan-address” with the physical LAN address of your computer. In this case, my computer has the address 192.168.0.131, so on my Android browser, I enter “http://192.168.0.131/vlc-shares/public”
 
Note: On Ubuntu machine, you can find out the IP address of your computer by right-clicking the network manager applet and select Connection Information
 
If your Android phone is connected via remote network
 
You have to enable the port forwarding feature in your router. We won’t touch on that in this tutorial. Refer to your router’s user manual for the instruction (or get more detail here).
 
On your Android browser, you should see the same dashboard interface.
 
Tap on the “Browse” button.
 
If you want to stream video from the Ubuntu computer, select the “Shared Folder” option and navigate to the folder where you store your videos. Select the video you want to stream and tap “Start VLC Stream”.
 
Select “Go to Stream”. When prompted, select “VPlayer”.
 
That’s it. Enjoy your video.
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




