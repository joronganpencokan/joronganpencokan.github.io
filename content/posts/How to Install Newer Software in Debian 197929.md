---
title: "Revamp Your Debian System: Learn How To Install the Latest Software in Just a Few Clicks!"
ShowToc: true 
date: "2022-12-09"
author: "Kevin Rowe"
---
*****
# Revamp Your Debian System: Learn How To Install the Latest Software in Just a Few Clicks!

As a Debian user, are you tired of manually browsing through countless websites and repositories to install the latest software updates? Fortunately, you don't have to spend hours of effort and frustration when it comes to updating your Debian system. In this post, we'll show you how to install the latest software in just a few clicks using the apt-get package manager and the Synaptic Package Manager.

## Why should you update your Debian system?

Updating your Debian system is not only about receiving the latest features and bug fixes, but it also ensures your system's security. Failing to update your system leaves your computer vulnerable to cyber-attacks and malware infections. The latest software updates not only improve your system's performance but also increase its lifespan by ensuring compatibility with newer software and hardware.

## Using apt-get to update your Debian system.

Apt-get is the package manager for Debian and the other Debian-based systems. It is a terminal-based command-line utility tool that lets you manage software packages and update them. Here's how to update your Debian system using the apt-get package manager.

### Step 1: Open Terminal.

Head on to your Debian system's terminal application, which can be easily accessed from the applications menu.

### Step 2: Update your software repositories.

Before updating your Debian system, you need to update your software repositories. To do this, type the following command and hit Enter:

```
sudo apt-get update
```

### Step 3: Install the latest software.

Once you update your software repositories, you can proceed to install the latest software by typing the following command:

```
sudo apt-get upgrade
```

### Using Synaptic Package Manager to update your Debian system.

The Synaptic Package Manager is a graphical package management tool that can be used to manage, install, remove and upgrade software packages. It provides a user-friendly interface for managing software and repositories. Here's how to use Synaptic Package Manager to update your Debian system.

### Step 1: Install Synaptic Package Manager.

Open the terminal by pressing `Ctrl+Alt+T` and run the following command:

```
sudo apt-get install synaptic
```

### Step 2: Launch Synaptic Package Manager.

Once the installation is complete, open your Debian system's applications menu and search for Synaptic Package Manager. Click the application to launch it.

### Step 3: Update your system.

Once you open the Synaptic Package Manager, you'll notice that it already has a list of available updates. Select the packages that you want to update and click on the "Mark for Upgrade" button. After that, click on the "Apply" button to start the upgrading process.

## Conclusion.

Updating your Debian system is an essential process that ensures your system's stability, performance, and security. By installing the latest software updates, you can enjoy the latest features and bug fixes while keeping your system protected from cyber threats. Fortunately, the process of updating your Debian system is not only easy but also fast. With just a few clicks, you can update your Debian system using either the apt-get package manager or the Synaptic Package Manager.

{{< youtube ntdlZ60XoD4 >}} 



Debian is an excellent Linux distribution, especially for servers. It is also a great distribution to run on a regular desktop computer or laptop. You very rarely encounter a bug on this operating system, and packages integrate exceptionally well with one another.
 
For example, you can easily switch to a different display/login manager, add another desktop environment or change other key components of your software stack. In contrast, you might get weird conflicts on other distributions when trying to switch default packages.
 
## Why Debian Has Old Software
 
Here’s the short version, without too many technical details. Once most of the known bugs are removed, packages are frozen to a particular version. Most of them will never receive feature upgrades, only security fixes. This way, no new bugs get introduced, and the distribution can remain “stable.” To be stable means that what worked in a certain way one year ago will work exactly the same way next year on the same version of Debian. The advantage is that you get an operating system that (almost) never “breaks.” You can pull in the latest security fixes, and rest assured that your laptop or computer will work just fine the next day.
 

 
You don’t lose a lot by not having the latest version of everything. Most software doesn’t dramatically change in the course of two years. But some software does indeed change often and brings important improvements.
 
Sometimes, you may even require the latest version of something. This may be the case with a new video card you bought that doesn’t work without the latest driver. For such situations, Debian has a special repository where you can upgrade certain pieces of software that you absolutely need to have.
 
## What Are Debian Backports?
 
Here’s how Debian’s official backports webpage describes what back-porting means:
 
This repository is not enabled by default, but the steps to do so are fairly straightforward.
 
## How to Enable Backports Repository on Debian
 
Open a terminal emulator, and find the codename of your Debian installation:
 
Note: in this example the codename is “stretch.” If at the time you read this the codename is different, for example “buster,” replace every occurence where you see “stretch” with “buster.”
 
Debian’s APT package manager stores the list of repositories where it can download software in a file. View and edit this file with the following command:
 
At the end of the file, add the following line:
 
On Debian Buster the line would be: “deb http://deb.debian.org/debian buster-backports main contrib non-free.”
 
Your APT sources list might not include the words “contrib” and “non-free.” In this case it means you don’t have some packages available. Among other things, such as the RAR archiver or Steam game platform, you will find drivers for your video card, Wi-Fi adapter and other hardware in “non-free.” If you need these, for example to play 3D video games or if your Wi-Fi isn’t working, enable “contrib” and “non-free.” Simply add the words at the end of each line, after “main.” The following is some text you can copy and paste:
 
Your sources.list file might also contain different URLs instead of “deb.debian.org.” Use “deb.debian.org,” as it has some advantages. It dynamically redirects you to a server close to you. Since it won’t always redirect you to the same server, there’s another advantage. If you use a static address, such as ” ftp.uk.debian.org/debian/,” if the server goes down, you won’t be able to download packages for that time.
 
With “deb.debian.org” that should no longer be an issue. It helps a lot, especially if you enable automatic upgrades. With a static server you might notice that your computer hasn’t been automatically updating for days or weeks, while the server was offline.
 
## Empty Screen After Running “sudo apt edit-sources”
 
On some installations the default file “/etc/apt/sources.list” might be missing. In this case sudo apt edit-sources will show an empty screen. Repositories might be stored in a file at “/etc/apt/sources.list.d/base.list” instead. With the following commands, you can see files in that directory and their contents:
 
When you edit the default sources file with sudo apt edit-sources, don’t repeat the lines you see here. Only add what is missing. Copy the lines from those files, add them to “/etc/apt/sources.list” and then delete the files in “/etc/apt/sources.list.d/.”
 
## How to Install Software from Debian Backports
 
Make the package manager pick up on your recent changes and update its database:
 
On Debian 9, codenamed Stretch, to install a newer Nvidia driver from backports, you would use this command:
 
On Debian 10, codenamed Buster, the command would be:
 
It’s not required to use the -V parameter, but it is useful in this case. This makes APT show version strings of the packages that it will install. It makes it easier to spot which packages will be pulled from backports and which will be pulled from regular repositories. Packages that contain the string “bpo” are from backports.
 
## Find Versions Available for a Package
 
Not all packages have backports available. Only the ones which have important or necessary features in new versions are usually backported. You can quickly check if you can install a newer version for a package with the following command:
 
In this case you can see that Nvidia’s proprietary driver version 384 is available in Debian’s regular repository. A superior version, 390, is available in backports.
 
Debian’s list of backported packages can also help you check if a package has a backport available. Remember to adjust the URL in the future with the codename of your current Debian release. “https://packages.debian.org/stretch-backports/allpackages” will be “https://packages.debian.org/buster-backports/allpackages.”
 
## Conclusion
 
Consider upgrading an emergency method from backports. This means don’t overdo it. Install only the packages you really need, otherwise you might make your system unstable or generate conflicts between packages.
 
Fell in love with computers when he was four years old. 27 years later, the passion is still burning, fueling constant learning. Spends most of his time in terminal windows and SSH sessions, managing Linux desktops and servers.
 
Our latest tutorials delivered straight to your inbox




