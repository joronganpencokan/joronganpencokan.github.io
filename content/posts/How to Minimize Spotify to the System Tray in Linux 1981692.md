---
title: "You Won't Believe How Easy It Is To Hide Spotify In Linux System Tray!"
ShowToc: true 
date: "2023-01-25"
author: "Brenda Patterson"
---
*****
Title: You Won't Believe How Easy It Is To Hide Spotify In Linux System Tray!

Are you a Linux user who loves using Spotify but hates having it take up space in your taskbar? Well, you're in luck because hiding Spotify in your system tray is incredibly easy! In this article, we'll show you how to do it using the Hugo writing format.

Step 1: Install the 'sni-qt' package

The first step is to install the 'sni-qt' package. This package is necessary for apps to integrate with the system tray on Linux. To install it, open up your terminal and type the following command:

sudo apt-get install sni-qt

Once the package has been installed, you'll need to log out and log back in for the changes to take effect.

Step 2: Download the 'SpotifyWM' script

The next step is to download the 'SpotifyWM' script. This script is what will enable you to hide Spotify in the system tray. You can download the script from Github by clicking on this link: https://github.com/faviouz/spotifywm

Once you have downloaded the script, save it to a convenient location on your computer.

Step 3: Make the script executable

Next, you'll need to make the script executable. To do this, open up your terminal and navigate to the directory where you saved the script. Once you're in the directory, type the following command:

chmod +x spotifywm

This command will make the script executable.

Step 4: Run the script

Finally, it's time to run the script! To do this, open up your terminal and navigate to the directory where you saved the script. Once you're in the directory, type the following command:

./spotifywm

This will launch Spotify and hide it in the system tray.

Conclusion:

Hiding Spotify in the system tray on Linux is incredibly easy, thanks to the 'sni-qt' package and the 'SpotifyWM' script. With just a few simple steps, you can free up space in your taskbar and keep Spotify running in the background. So give it a try and see how much more streamlined your desktop can be!

{{< youtube TTPjZUo44-k >}} 



Spotify isn’t what it used to be. The recent versions of the Spotify client for Linux have lost the ability to hide in the tray. Now they always take up a spot in your taskbar or dock, but thankfully, there is a way to minimize Spotify to the system tray in Linux. Let’s see how.
 
## Install KDocker
 
For this to work, we will use both the latest version of the Spotify client and KDocker. Although its name starts with a “k,” KDocker is not associated with the KDE desktop. It is a simple tool that allows you to move any application to the tray in most popular desktop environments. While it has not been updated for quite a while, it is still working fine for most desktop environments. It is probably the best current solution for docking Spotify’s client.
 
You can install KDocker in Ubuntu and compatible distributions with:
 
In Fedora, Red Hat, and their siblings, try:
 
## Use KDocker to Minimize Spotify to the System Tray
 
Launch KDocker from your Applications menu after installation.
 
Click on the Spotify window to minimize it to the tray.
 
Done! You’ll find your app in the tray instead of your taskbar.
 
For it to show Spotify again, click on the KDocker tray icon and select “Show Spotify.”
 
You can also right-click on the icon and select “Dock Another” to repeat the process for other apps.
 
## Integrate KDocker to Spotify
 
As you can see, the above method requires you to run Spotify and KDocker simultaneously. Another way to do it is to integrate KDocker to Spotify so it can minimize to the tray anytime. 
 
Note that the following instructions make use of the Ubuntu’s default desktop.
 
Also, keep in mind that these tweaks will apply only to the desktop icon. If you launch Spotify any other way, such as from your app list or the terminal, Spotify will behave normally and won’t hide to the tray.
 
Start by locating Spotify’s icons. Try:
 
You should see a list of spotify-related icons. Jot down the path to a specific one, such as “/usr/share/icons/Papirus/64×64/apps/spotify.svg”.
 
Copy the Spotify client’s desktop entry to your Home folder with the command:
 
Edit the copied file with your favorite text editor. We prefer nano, so our command was:
 
Locate the Exec=spotify %U line. 
 
Change it to:
 
What the above command does is let KDocker handle the opening of the Spotify app so that it can become minimizable. The path to the Spotify icon is for KDocker to display the Spotify icon on the system tray. Without it, it will just show a generic icon.
 
Save the changes with Ctrl + o and exit the file with Ctrl + X. 
 
Launch your Spotify, and you should see its icon on the system tray. 
 
Click on it to minimize Spotify to the system tray.
 
If you are tired of using the Spotify client, you can try the Spotify Web Player or use these tips to hide your Spotify listening activity.
 
OK's real life started at around 10, when he got his first computer - a Commodore 128. Since then, he's been melting keycaps by typing 24/7, trying to spread The Word Of Tech to anyone interested enough to listen. Or, rather, read.
 
Our latest tutorials delivered straight to your inbox




