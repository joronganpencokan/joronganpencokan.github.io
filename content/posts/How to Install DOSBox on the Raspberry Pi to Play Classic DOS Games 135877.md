---
title: "Unleash Nostalgia with Dosbox on Your Raspberry Pi: Relive Classic Dos Games in Minutes!"
ShowToc: true 
date: "2023-01-21"
author: "Eleanor Cortinas"
---
*****
# Unleash Nostalgia with Dosbox on Your Raspberry Pi: Relive Classic Dos Games in Minutes!

Do you miss playing classic DOS games from your childhood? Are you tired of feeling nostalgic but not being able to experience those games again? Well, we have good news for you! With the help of Raspberry Pi and DOSBox, you can relive your memories and enjoy your favorite games once again.

DOSBox is an emulator that allows you to run DOS-based games and software on modern systems like Raspberry Pi. It is easy to install and use, and it provides an authentic experience of using MS-DOS on your Raspberry Pi. DOSBox is free and open-source software, which means you can use it for personal and commercial purposes without any restrictions.

In this article, we will guide you through the process of installing DOSBox on Raspberry Pi and playing classic DOS games. So, let's get started.

## Step 1: Install Raspbian OS

Raspbian is the official operating system for Raspberry Pi. You can download it from the Raspberry Pi Foundation's website and install it on your Pi using an SD card. Follow the instructions on the website to download and install Raspbian. Once you have installed Raspbian, connect your Raspberry Pi to a keyboard, mouse, and monitor.

## Step 2: Install DOSBox

DOSBox is available in the Raspbian repository, so it is easy to install. Open the terminal on your Raspberry Pi and type the following command:

```
sudo apt-get install dosbox
```

This command will download and install DOSBox on your Raspberry Pi. Once the installation is complete, you can launch DOSBox by typing the following command in the terminal:

```
dosbox
```

## Step 3: Mount C Drive

DOSBox emulates a virtual drive, which means you need to mount the C drive before you can run any DOS-based software. To do this, type the following command in the DOSBox terminal:

```
mount c ~/dos
```

This command will mount the default C drive to the "dos" folder in your home directory. You can change the path to any other directory you prefer.

## Step 4: Install DOS Games

Now that you have installed DOSBox and mounted the C drive, it's time to install DOS games. You can find many classic DOS games online that you can download and install on your Raspberry Pi.

Once you have downloaded a DOS game, extract the files to a folder on your Raspberry Pi. In this example, we will use the classic game "Duke Nukem 3D." We will extract it to the "dos" folder in our home directory.

## Step 5: Run DOS Games

To run a DOS game, you need to navigate to the game's directory in the DOSBox terminal and type the executable file's name. In our example, we will navigate to the "dos" folder in our home directory and type the following command:

```
cd ~/dos
duke3d.exe
```

This command will launch Duke Nukem 3D in DOSBox, and you can start playing the game. You can use the keyboard and mouse to control the game, just like you did back in the day.

## Conclusion

In this article, we have shown you how to install DOSBox on Raspberry Pi and run classic DOS games. With the help of DOSBox, you can unleash your nostalgia and relive the memories of your childhood. Raspberry Pi is an affordable and easy-to-use platform that allows you to run old software and games that you thought were lost forever. We hope you enjoyed this article and found it informative. Happy gaming!


Do you remember the original SimCity games? How about Golden Axe, The Oregon Trail, or Wolfenstein? Debuting in 1981, MS-DOS (Microsoft Disk Operating System) saw thousands of games released across every genre. If you miss the games in the DOS era, you’ll learn here how to install DOSBox on Raspberry Pi to enjoy all of those classic DOS games.
 
By the end of this tutorial, you’ll have transformed your Raspberry Pi into a retro gaming rig.
 
Once your MS-DOS emulator is up and running, you’ll need some games, so you’ll learn how to access thousands of free MS-DOS games, including classics such as Lemmings, Street Fighter, and the 90s Aladdin and Lion King games.
 
## What you’ll need
 
To complete this tutorial, you’ll need:
 
- Raspberry Pi that’s running Raspberry Pi OSPower cable that’s compatible with your Raspberry PiExternal keyboard and a way to attach it to your Raspberry PiHDMI or micro HDMI cable, depending on model of Raspberry PiExternal monitorGaming controller, preferably

 
Once you’ve assembled your tools, you’re ready to build your gaming rig.
 
## Update your Pi
 
If you haven’t already, attach your external keyboard, monitor, controller and any other peripherals to your Raspberry Pi, and then attach your Pi to a power source.
 
Before you build your rig, check that your Raspberry Pi is fully up to date. Open a terminal and type the following command:
 
## DOSBox: installing MS-DOS emulator
 
DOSBox is an emulator that mimics a computer running the DOS operating system, which makes it possible to run DOS games on your Raspberry Pi.
 
DOSBox is popular with retro-gaming enthusiasts and video game publishers alike, with a number of big names using DOSBox to re-release classic titles, such as Bethesda Softworks, who used DOSBox to re-release some of its Elder Scrolls games.
 
Note: also, check out the DOSBox Installation guide for Linux, macOS, and Windows.
 
To install DOSBox, run the following command on your Raspberry Pi:
 
And that’s it! DOSBox is now installed on your Pi.
 
### Configuring DOSBox
 
Before you can enjoy any DOS games on the Raspberry Pi, you need to configure your DOSBox setup.
 
To start, create a directory where all of your DOS games will be stored. A directory named “dos-games” was created fr this tutorial in the Raspberry Pi’s home directory.
 
To create a directory, run the following command:
 
DOSBox’s configuration file isn’t created until DOSBox runs for the first time, so do this now. In the Terminal, simply type the following:
 
Don’t forget to press the Enter key on your keyboard.
 
### Playing DOSBox games with a controller
 
Now that DOSBox is up and running, the next step is configuring your gaming controller. If you haven’t already, attach the controller that you want to use.
 
Next, press the Ctrl + F1 keys on your keyboard, and the keymapper window should appear onscreen.
 
Note that if the keymapper doesn’t launch, then DOSBox may not be running. You should be able to solve this problem by entering dosbox into the Terminal, pressing Enter and then repeating the keyboard shortcut.
 
Depending on your model of gaming controller, DOSBox may detect and map your controller automatically. If DOSBox doesn’t recognize your controller, you’ll need to configure it manually by following the onscreen instructions.
 
Once you’ve set up your controller, DOSBox is ready to go. You just need to decide which game you want to play.
 
## Finding free DOS games: SimCity, Golden Axe, Street Fighter
 
There’s a few places where you can download DOSBox games. Abandonia has thousands of free DOS games for you to choose from.
 
Abandonia is an abandonware website that specializes in software and games that are unsupported by the original owner, publisher, developer or manufacturer and aren’t currently available on the retail market. Unsurprisingly, lots of DOS games meet this criteria!
 
To download one or more games for your DOSBox rig, open your Raspberry Pi’s web browser and spend some time browsing Abandonia’s selection of free DOS games.
 
When you find a game that you want to try, simply click “Get it” to download that game as a zip file. The free Apollo 18 game is included in all of this tutorial’s screenshots.
 
### Create a directory of DOS games
 
Once you’ve downloaded one or more games, you’ll need to extract the compressed files into the “dos-games” directory you created in the previous step.
 
Once done, your DOS games are now ready to play!
 
## Enjoy your DOSBox gaming rig
 
To play a game, open the unzipped game file and look for the game’s executable .exe file. The exact file will vary between games. for example, the Apollo 18 game this file was “apollo.exe.”
 
Right-click the “.exe” file and select “Open With … “
 
In the subsequent window, select “Games -> DOSBox Emulator.”
 
This game will now launch in DOSBox, ready for you to enjoy.
 
After installing the DOSBox on Raspberry Pi, you should now have a gaming rig that’s capable of playing all of the classic DOS games.
 
If you are more into retro gaming, you can also turn your Raspberry Pi into a Retro Gaming Console or a simple Minecraft server on Raspberry Pi. What are your favorite DOS games?
 
Jessica Thornsby is a technical writer based in Derbyshire, UK. When she isn’t obsessing over all things tech, she enjoys researching her family tree, and spending far too much time with her house rabbits.
 
Our latest tutorials delivered straight to your inbox




