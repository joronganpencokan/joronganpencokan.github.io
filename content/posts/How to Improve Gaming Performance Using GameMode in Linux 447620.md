---
title: "Unlock The Ultimate Gaming Experience in Linux: Boost Your FPS With Gamemode!"
ShowToc: true 
date: "2023-02-24"
author: "Jeff Dearing"
---
*****
# Unlock The Ultimate Gaming Experience in Linux: Boost Your FPS With Gamemode! 

If you are a Linux gamer, you might have faced the problem of low FPS while playing your favorite games. This issue can be frustrating as it can ruin your gaming experience.

Gamemode is a solution to this problem. It is a tool that optimizes your Linux system for gaming and boosts the FPS in games. In this article, we will discuss why Gamemode is important and how to use it. 

## The Importance of Gamemode 

Gamemode is a system daemon that sets the CPU governor and I/O scheduler to performance mode when a game is launched. This means that your system will prioritize the game and give it more resources to improve performance. 

The default governor and I/O scheduler settings are usually set to power-saving mode, which is good for regular use but not ideal for gaming. Gamemode makes sure that your system is optimized for gaming and that you get the best possible performance while playing games. 

Gamemode is compatible with most Linux distributions, including Ubuntu, Arch, Manjaro, Fedora, and more. 

## How to Install Gamemode 

Gamemode is available in most Linux repositories, which means that you can simply install it using your distribution's package manager. 

### For Ubuntu-based distributions: 

```
sudo apt install gamemode
```

### For Arch-based distributions: 

```
pacman -S gamemode
```

### For Fedora-based distributions: 

```
sudo dnf install gamemode
```

Once you have installed Gamemode, you can proceed to the next step. 

## How to Use Gamemode 

Using Gamemode is as simple as running a command in the terminal. 

To enable Gamemode for a game, simply prefix the game's command with "gamemoderun." For example, if you want to launch "Counter-Strike: Global Offensive," you would use the following command: 

```
gamemoderun ./csgo_linux64
```

This will launch the game with Gamemode enabled. You can also create a shell script that enables Gamemode for all your games automatically. 

```
#!/bin/bash 
gamemoderun "$1"
```

Save this script as "gamerun" and make it executable using the following command: 

```
chmod +x gamerun
```

Now, whenever you want to launch a game, simply use the following command: 

```
./gamerun <game command>
```

## Conclusion 

Gamemode is a powerful tool that can help you unlock the ultimate gaming experience in Linux. It is easy to install and use and can significantly boost your FPS in games. If you are a Linux gamer, we highly recommend that you give Gamemode a try. 

We hope that you found this article helpful. If you have any questions or suggestions, please feel free to leave a comment below. 

Happy gaming!

{{< youtube foCFdb9BAJI >}} 



Linux is a great platform for gaming, but it can sometimes be challenging to get the best performance out of your games. This is where GameMode, a tool that allows you to optimize your system for gaming, comes in. Here we show you how to install and use GameMode to improve gaming performance in Linux.
 
Also check out some of the best games for Linux.
 
## What Is GameMode?
 
GameMode is a command line utility that improves gaming performance on Linux. It is developed and maintained by Feral Interactive.
 
GameMode works by optimizing your system for gaming. It sets your CPU governor to “performance” mode and your system’s I/O priority to real time. This ensures that your games have the best chance of running smoothly without hiccups.
 
Additionally, GameMode can disable or reduce the effects of CPU frequency scaling and process scheduler latency adjustments. This further improves game performance, especially in multiplayer games where every second matters.
 
On the other hand, if you are having high CPU usage issue in Linux, we have the fixes here.
 
## How to Install GameMode on Your Linux System
 
- Update and upgrade all your packages:

 
- Before we install the GameMode package, we need to install a couple of dependencies that GameMode will use. GameMode depends on systemd  for internal communication and meson for building. Install the dependencies with this command:

 

 
You may be asked whether you want to continue with the installation. If so, press Y to proceed.
 
- Clone the latest version of GameMode from Github.

 
This downloads the package to the folder from which you are running the terminal.
 
- Change your directory to gamemode:

 
- Build GameMode using these commands:

 
- Test whether GameMode was installed correctly using this command:

 
The command will test the GameMode installation with a series of commands. If everything worked correctly, you will receive a success message stating that all tests passed. 
 
## Using GameMode to Improve Gaming Performance on Standalone Games
 
By default, GameMode does not detect your games. Therefore, you have to start it every time you want to play a game.
 
Although the game in this example, Kmines, does not use heavy graphics, we are starting it using GameMode to illustrate how to run games.
 
To start your game using GameMode, follow these steps:
 
- Launch your game from the terminal starting with the gamemoderun command. For KMines, the command is:

 
Your game should start with enhanced performance from GameMode. 
 
- To test whether GameMode is working correctly, run this command:

 
If your game uses GameMode, you should get a message saying “gamemode is active” on your terminal. If you close the game, GameMode will be deactivated automatically.
 
Alternative: if your computer only has a limited amount of RAM, use zswap to improve its performance.
 
## Using GameMode on Steam
 
You can also run your Steam games using GameMode to improve gaming performance. Assuming that you have Steam set up and your game downloaded, follow these steps to play games on Steam using GameMode:
 
- Under your library tab, right-click on the game you wish to launch and click “Properties.”

 
- Type in this command in the launch options textbox:

 
Exit the properties window.
 
- Launch the game by tapping on the “Play” option.

 
To confirm that your game launched correctly, open a new terminal window and type this command to check whether GameMode is active:
 
If all went well, you should get a message saying, “gamemode is active.”
 
Tip: learn how to track your Steam stats, deals, spending and play time.
 
## Using GameMode on Lutris
 
If you are an avid Linux gamer, you may be familiar with Lutris Lutris, an open-source gaming platform for Linux, that makes it easy to install and manage games from various sources, including Steam, GOG, and even your collection of Windows games.
 
Similar to Steam, setting GameMode on Lutris involves adding a command prefix to the game launch configurations. To improve gaming performance using GameMode on Lutris:
 
- On your Lutris home screen, right-click on the game you want to launch and click “Configure.”

 
- Click on the “Systems options” tab to set the configurations for the game.

 
- Scroll to the “Command Prefix” option and type in the following command in the textbox:

 
Click on “Save” to exit the configuration menu. 
 
- Right-click on the game you want to run and click “Play.” The game will launch using GameMode.

 
The best part about using GameMode on Lutris is that you only have to configure the game once. The game will automatically run when you launch it the next time with GameMode on. You can also run the gamemoded -s command to check whether GameMode is active.
 
## Using GameMode on Non-Games
 
While GameMode was designed to be used with games on Linux, you can also use it on non-games to improve performance. This feature is handy when running heavy apps, such as video- and photo-editing tools.
 
Using GameMode with non-games is pretty straightforward. Launch the app from the terminal using the gamemoderun prefix. For example, the following command will launch GIMP with enhanced performance from GameMode:
 
## Frequently Asked Questions
 
All screenshots by Allan Ngetich.
 
### How do I turn GameMode off?
 
GameMode automatically turns off once you close the game or the app you used. Regardless of the platform you are using, close the game, and GameMode will turn off automatically.
 
### Does Game Mode increase FPS?
 
Yes, GameMode can increase FPS for some games. Games that are particularly CPU-heavy may see the most benefit with GameMode. If you do not see a significant increase in FPS after enabling GameMode, your game may be more limited by your GPU than your CPU.
 
### Does GameMode use more battery?
 
Yes, GameMode will use more battery power when active, as it is designed to do. However, the effect on battery life will vary depending on the game. Games that are more demanding on system resources will significantly decrease battery life when GameMode is enabled. For less demanding games, the impact on battery life may be negligible.
 
For prolonged battery life, follow these tips to improve battery life on a Linux laptop.
 
Allan Ngetich is a writer at Make Tech Easier, a website that provides tips, tricks and tutorials on technology. He was born and raised in Kenya, and has always been interested in technology. He started his career as a blog writer, and has since written for several websites. He is a firm believer in hard work and team work, and is always striving to improve his skills.
 
Our latest tutorials delivered straight to your inbox




