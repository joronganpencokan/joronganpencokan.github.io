---
title: "Linux Users Rejoice! Learn How to Easily Install Handbrake and Rip Your Favorite DVDs Now!"
ShowToc: true 
date: "2023-04-13"
author: "Roxanne Cromwell"
---
*****
Linux Users Rejoice! Learn How to Easily Install Handbrake and Rip Your Favorite DVDs Now!

As a Linux user, you may have found it difficult to find the right software to do simple tasks like ripping DVDs. But rejoice, because Handbrake, the popular DVD-ripping tool, is now easily available for Linux users. Whether you want to backup your favorite movies or transfer them to your mobile device, Handbrake is a must-have tool. In this article, we’ll guide you through the process of installing Handbrake on your Linux machine so you can start ripping DVDs right away!

What is Handbrake?

Handbrake is a popular open-source software that allows users to easily rip DVDs and convert them to digital video files. It’s available for Windows, macOS, and Linux operating systems, making it a great choice for users who need to transfer DVD content to different devices. Handbrake is not only a free tool, but it’s also easy to use and offers a wide range of features like video conversion, DVD ripping, and options to optimize video quality.

How to Install Handbrake on Linux

Step 1: Open the Terminal

To install Handbrake on your Linux machine, you’ll need to open the terminal. This can be done by pressing the “Ctrl + Alt + T” keys together or by searching for “Terminal” in the Applications menu.

Step 2: Add Handbrake Repository

Once you have the terminal open, you’ll need to type in the following command:

$ sudo add-apt-repository ppa:stebbins/handbrake-releases

This command will add Handbrake’s repository to your system, allowing you to install the latest version.

Step 3: Update the System

After adding the repository, you’ll need to update your system with the following command:

$ sudo apt-get update

This will ensure that your system is updated with the latest changes and packages.

Step 4: Install Handbrake

Finally, to install Handbrake simply run the following command:

$ sudo apt-get install handbrake

That’s it! Once installation is complete, you can start using Handbrake to rip DVDs and convert video files.

Using Handbrake to Rip DVDs

Once you have Handbrake installed, ripping DVDs is a breeze. Here are the steps to follow:

Step 1: Open Handbrake

Firstly, open the Handbrake software by searching for it in the Applications menu.

Step 2: Insert DVD

Insert the DVD you want to rip into your computer. The software automatically detects the DVD and displays its details.

Step 3: Select Title

Select the title you want Handbrake to rip. You can choose the main movie or select individual episodes or chapters.

Step 4: Choose Settings

Next, you’ll need to choose the settings according to your preferences. You can select the output format, quality, and file size. Handbrake also offers advanced features like adding subtitles, cropping videos, and changing the aspect ratio.

Step 5: Start Ripping

Finally, click on the “Start” button and wait for the process to complete. Once Handbrake is done ripping your DVD, you can find the video file in your preferred location.

Conclusion

As you can see, installing Handbrake on your Linux machine is a simple process that can be completed in a few minutes. With Handbrake, you can easily rip and transfer DVDs to various devices, without any hassle. Linux users no longer need to be restricted to a limited selection of software. By using Handbrake, you can enjoy the freedom to backup and enjoy all your favorite movies and TV shows on your devices with ease.

{{< youtube 8R5CiR19xoE >}} 



Handbrake is a powerful open-source tool for encoding and editing video. It includes a graphical control panel to manage your encodes and even preview the result. Part of what makes Handbrake such a favorite in the Linux world is its ability to encode off of a DVD, effectively making it one of the best tools available for ripping DVDs.
 
The legality of ripping DVDs can be murky in some countries. The purpose of this article is to inform you how to make archival copies of DVDs that you legally own, but be sure to check the laws in your area before continuing.
 
Do note that Handbrake is also available for Windows and macOS.
 
## Install Handbrake
 
Everything here relies on Handbrake, but there’s another piece you’ll need too. The VLC developers created a library, libdvdcss, for decoding copyright-protected DVDs for playback. Handbrake relies on it to decode DVDs, too, so you’ll need it as well.
 
### Ubuntu
 
Ubuntu does have Handbrake in its repositories, but due to the legal grayness of libdvdcss, it’s not in the repositories. Instead, Ubuntu provides a script to build the package yourself. Don’t worry, it’s all automatic. Start by installing libdvd-pkg, the script package.
 

 
A menu will pop up in the terminal asking if you want to continue. Agree to everything and keep going. When it’s done, you’ll need to reconfigure the package to build and install libdvdcss.
 
Finally, install Handbrake.
 
### Debian
 
Debian has an excellent multimedia repository that’s maintained by one of the Debian developers. You can add it to your system and install both Handbrake and libdvdcss. Start by downloading the repository’s key. It comes in a .deb package.
 
Install the package to import the key.
 
Use your favorite text editor to create a new file at “/etc/apt/sources.list.d/multimedia.list.” Open it and add the following line. Enter either “stretch,” “testing,” or “sid” to match your version of Debian.
 
Update Apt and install both packages.
 
### Fedora
 
Both packages are available on Fedora through the RPM Fusion repository. Start by enabling it on your system.
 
libdvdcss is found in the separate “tainted” RPM Fusion repo. You’ll need to add that too via a package from the regular RPM Fusion.
 
Now you can install Handbrake and libdvdcss.
 
### Arch Linux
 
Arch Linux has both packages in its regular repositories. Just install them.
 
## Rip a DVD
 
Open Handbrake. You can find it under the “Multimedia” category on your application menu. When Handbrake opens, it might look overwhelming at first, but it’s actually fairly simple, when you break it down.
 
### Load the Source
 
Begin by selecting your source. This could be a source file, but in this case, it’s your DVD drive. You’ll see an “Open Source” button in the upper-left corner of the screen. Click it.
 
A new window will open for you to browse to your source. There are a couple shortcuts to your DVD drive. First, if you already have your DVD in the drive, it should appear with the DVD’s title on the left of the window. Click on it and select “VIDEO_TS” to open.
 
You can also use the “Detected DVD devices” drop-down at the bottom of the window. It’ll probably have your drive selected already, so you can just open it right from there. If not, you can usually find your drive under the drop-down. It’s usually a drive letter like “/dev/sr0.”
 
After you select it, your drive will spin and start reading your DVD. A progress bar will pop up at the top of the Handbrake window as it loads your DVD. When it’s done, you’ll see your DVD’s title listed as the source in the upper-left.
 
### Select the Preset
 
Handbrake has presets with common aspect ratios, frame rates, and support for certain devices. You’ll find the preset list in the upper-right corner of the Handbrake window.
 
Scroll through and see what looks best for your use. If you’re just looking to make a copy of your DVD, you can select the “Fast 1080p30” preset as a good default. It will produce a quality 1080p copy of your DVD. If your DVD is an older standard definition DVD, Handbrake will use the native dimensions of the DVD and copy it as is.
 
### Add Titles to the Queue
 
Turn your attention back to the upper-left corner of the screen. Take a look at the “Title” drop-down directly under the “Source” label with your DVD’s title.
 
DVDs are broken up into titles. These are the individual videos on the DVD, and most of them are just garbage from the menus. It’s up to you to pick out the titles that contain the actual content that you want. The easiest way to do so is with the duration of the title. If your DVD is a movie, you can find the title with the same run time as the full film. If you’re looking for the episodes of a TV show, find titles that last about as long as one. They should all be fairly uniform. When you have your title, select it.
 
Below the title drop-down, take a look under the “Destination” header. There you can name your file. Under that, you can choose the destination for your video. You can place it anywhere with enough free space.
 
After everything looks good, press the “Add To Queue” button in the menu across the top of your window. It’s right next to the “Open Source” one. If you’re doing TV episodes, repeat these steps for each episode, adding each one to the queue.
 
### Rip!
 
Now that you have all of the titles that you want to back up in your queue, you can start ripping. If you’d like to double-check your queue, click the “Show Queue” button in the top menu. It’ll display all of your enqueued titles and the output file names.
 
Click “Start Encoding” in the top menu to start ripping your DVD. Handbrake will take a decent amount of time, depending on your CPU and DVD drive speeds, to work its way through your selected titles. When it’s done, it’ll show you a success message. At that point you’re free to eject your DVD and/or close Handbrake.
 
Congrats! You’re now ready to back up your DVDs or view them digitally on your devices. Remember to check the laws in your area before doing this, and never illegally distribute duplicated DVDs.
 
Nick is a freelance tech. journalist, Linux enthusiast, and a long time PC gamer.
 
Our latest tutorials delivered straight to your inbox




