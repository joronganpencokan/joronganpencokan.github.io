---
title: "10 Easy Steps to Install Skype on Ubuntu - Join the Global Conversation Now!"
ShowToc: true 
date: "2023-06-13"
author: "Kay Wald"
---
*****
# 10 Easy Steps to Install Skype on Ubuntu - Join the Global Conversation Now!

If you are an Ubuntu user, and you want to join the millions of people around the world who use Skype for communication, you are just a few steps away from joining the global conversation. Despite being a Microsoft product, Skype can be easily installed on Ubuntu, and in this article, we will show you how to do it.

Before we get started, make sure you have a stable internet connection and an updated Ubuntu system.

1. Open the Terminal: Press "Ctrl + Alt + T" or find it in the applications menu.

2. Add the Skype repository: Type in the following command in the terminal and press Enter:

```bash
sudo add-apt-repository "deb http://archive.canonical.com/ $(lsb_release -sc) partner"
```
This will add Skype repository to your system.

3. Update the system: Type in the following command in the terminal to update the system:

```bash
sudo apt-get update
```

4. Install Skype: Type in the following command in the terminal and press Enter:

```bash
sudo apt-get install skype
```

5. Confirm the installation: Type "Y" and press Enter to confirm the installation of Skype.

6. Wait for the installation: The installation process might take a few minutes depending on your internet speed.

7. Launch Skype: Once the installation is completed, launch Skype from the applications menu.

8. Sign in or create an account: If you already have a Skype account, sign in with your credentials, or create a new account by following the on-screen instructions.

9. Allow access to your microphone and camera: Skype might ask for permission to access your microphone and camera. Allow it to proceed with video and audio calls.

10. Enjoy Skype: Congratulations, you have installed Skype and are now ready to connect with people all over the world.

In conclusion, installing Skype on Ubuntu is a straightforward process that can be completed in just a few minutes. Follow the above steps and join millions of people who use Skype for communication. Whether it's personal or professional, Skype is a great tool for staying connected with people. With Skype at your fingertips, the world is just a call away.

{{< youtube DNbzRW82rII >}} 



There are actually a couple of ways to get Skype installed and running on your Ubuntu system. Both are fairly easy. It’s probably more convenient to use a Snap package, but you can also download and install Skype directly from Microsoft’s site.
 
## With a Snap
 
Snaps are a relatively new universal packaging format for Linux. That means that Snap packages will work across all Linux distributions, making it an ideal format for applications like Skype.
 
Only recently, Skype started packaging in a Snap format, which is a big deal because Skype has historically been one of the more problematic packages to manage on Linux. Hopefully, this step forward will help make Skype more reliable for Linux users.
 
### Check Snapd
 

 
Canonical, Ubuntu’s parent company, is responsible for creating the Snap format. So support on Ubuntu is about as good as it gets. Just double-check that your Ubuntu install is running the snapd service, but it probably is.
 
On the off chance that it isn’t, install the package.
 
### Install Skype
 
Now you can install Skype. Snaps are like any other Linux packages, so you can just tell the package manager to install it.
 
The --classic flag is necessary for file sharing over Skype.
 
## The Classic Way
 
If you don’t want to get involved with Snap, you can download and install a classic “.deb” package directly from Microsoft.
 
### Get the Package
 
Go to Microsoft’s Skype download page, and select “Skype for Linux DEB.” Save the package when you’re asked.
 
### Install with DPKG
 
Open up a terminal, and change into your download directory.
 
Then, use dpkg to install Skype.
 
### The Easiest Way: Double-Click
 
An easier way (or perhaps the easiest) to install a .deb file in Ubuntu is to simply double-click on it, like how you double-click an .exe file in Windows. In the window that opens up, click “Install.”
 
## Using Skype
 
Skype for Linux is a lot like the web application version of Skype. That’s because it practically is the web application version. Microsoft got kind of lazy with that. Still, it’s better than the old buggy version of Skype that never got updates.
 
Once you start up Skype, sign in to your account, or create one. You’ll be dropped into the same interface that you’d expect, with your contacts to the left and a chat/status space on the right. Again, it’s almost identical to the web interface.
 
From here, you can use Skype the way you’re accustomed to. Skype will run on startup by default and move itself to the background when it’s closed. Make sure to modify this behavior if it’s not what you want.
 
Nick is a freelance tech. journalist, Linux enthusiast, and a long time PC gamer.
 
Our latest tutorials delivered straight to your inbox




