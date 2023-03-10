---
title: "You Won't Believe How Easy It Is To Install Spotify On Linux!"
ShowToc: true 
date: "2023-01-02"
author: "Michael Bullard"
---
*****
Title: You Won't Believe How Easy It Is To Install Spotify On Linux!

Linux is a popular open-source operating system used widely by software developers, enthusiasts, and tech-savvy users. While Linux has several advantages, one of its drawbacks is the difficulty in using some applications that are widely available on other platforms. Fortunately, Spotify has made it incredibly easy to install and use their music streaming service on Linux.

In this guide, we will walk you through the simple steps to install Spotify on Linux, so you can enjoy your favorite music on your Linux machine.

Step 1: Add Spotify Repository

The first step to install Spotify on Linux is to add the Spotify repository to your system. This is a simple process that will enable your Linux machine to access and download the latest version of the Spotify app.

To add the Spotify repository, open your terminal and type the following command:

sudo sh -c 'echo "deb http://repository.spotify.com stable non-free" >> /etc/apt/sources.list.d/spotify.list'

This command adds the Spotify repository to your system's sources list.

Step 2: Import Public Key

The next step is to import the public key used to sign the Spotify packages. This will enable your system to verify that the packages downloaded from the repository are authentic and safe to install.

To import the public key, type the following command in your terminal:

sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4773BD5E130D1D45

This command will import the public key used to sign the Spotify packages.

Step 3: Install Spotify

Now that you have added the Spotify repository and imported the public key, the final step is to install Spotify on your Linux machine.

To install Spotify, run the following command in your terminal:

sudo apt-get update && sudo apt-get install spotify-client

This command updates your system's package list and installs the Spotify client.

Once the installation is complete, you can launch Spotify by searching for it in your applications system or by typing the following command in your terminal:

spotify

Conclusion

Installing Spotify on Linux is incredibly easy, thanks to the simple steps outlined in this guide. With just a few commands in your terminal, you can now enjoy your favorite music on your Linux machine.

While most Linux distributions may not come pre-installed with Spotify, you can easily add the repository and public key to your system, and install the client just like any other Linux application.

So, what are you waiting for? Go ahead and install Spotify on your Linux machine today and enjoy your favorite music hassle-free!

{{< youtube gnucYb51QNo >}} 



Spotify is the most popular streaming music service in the world. Plenty of people rely on it for almost all of their music. While it’s totally possible to listen from your web browser, it’s much nicer to have an app directly on your desktop.
 
Spotify has actually been supporting Linux for quite some time, now. While most distributions don’t include it in their main repositories for licensing reasons, it’s really not hard to get the official player installed on your Linux PC.
 
## Install Spotify
 
Spotify technically only packages for Debian distributions and via a Snap, but other distributions have dedicated package maintainers that have taken up the task of packaging Spoitfy for their favorite distribution. Follow the set of instructions that best matches your version of Linux.
 
### Ubuntu/Debian
 

 
The Spotify developers actually maintain a package repository for Debian-based distributions like Ubuntu and Linux Mint. You can add the repository and automatically receive the latest updates direct from the source.
 
First, add the repository key to your system.
 
Create a new document “spotify.list” at “/etc/apt/sources.list.d/.”
 
sudo nano /etc/apt/sources.list.d/spotify.list
 
Place the following line inside.
 
Now, simply update Apt and install the Spotify client.
 
Alternatively, Ubuntu users can install Spotify via Snap.
 
### Fedora
 
Fedora doesn’t have an official Spotify package, but the RPM Fusion repository absolutely does. That said, in testing for this article the RPM Fusion method was a complete disaster. Don’t go that route. Instead, you can skip down to the Snap, or you can make use of Flatpak, which tends to be better supported on Fedora.
 
### Arch Linux
 
Spotify is available for Arch through the AUR. If you don’t have an AUR helper, you can clone the repository found on its AUR page and build with makepkg.
 
Otherwise, install it with your AUR helper.
 
Confirm and install.
 
### Snap
 
Of course, you can bypass all of this on any system that can install snaps. Install the official Spotify snap instead.
 
## Using Spotify
 
The client is a graphical application. You can find it under the “Sound and Video” or “Multimedia” section of your desktop environment. GNOME systems list it alphabetically under “Spotify.”
 
When you launch Spotify for the first time, it will prompt you to log in or sign up for Spotify. Enter your account info, and you’ll arrive at an interface similar to the one you’re used to online and on other platforms.
 
Congratulations! You’re ready to listen to your favorite streaming music on Linux!
 
Nick is a freelance tech. journalist, Linux enthusiast, and a long time PC gamer.
 
Our latest tutorials delivered straight to your inbox




