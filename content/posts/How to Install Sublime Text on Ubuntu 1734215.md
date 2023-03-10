---
title: "Unlock the Power of Coding: Install Sublime Text on Ubuntu with These Simple Steps!"
ShowToc: true 
date: "2023-06-17"
author: "Tom Dillon"
---
*****
# Unlock the Power of Coding: Install Sublime Text on Ubuntu with These Simple Steps!

Are you a seasoned programmer or a newbie who's eager to dive into the world of coding? Regardless of your experience level, your choice of code editor is critical. In today's fast-paced programming world, a programmer requires a code editor that's powerful, speedy, and has an easy-to-use interface. Sublime Text is one such code editor that's widely used by programmers worldwide. In this article, we'll show you how to install Sublime Text on Ubuntu.

## What is Sublime Text?

Sublime Text is a sophisticated yet easy-to-use code editor that supports multiple programming languages. Sublime Text is available for Windows, Linux, and macOS platforms. The editor comes equipped with various features such as syntax highlighting, auto-completion, powerful search and replace features, and a built-in package manager that makes installing plugins and add-ons a breeze. With Sublime Text, you can improve your coding productivity, whether you're programming in Python, C++, JavaScript, or HTML.

## Pre-requisites for Installing Sublime Text

Before we dive into the installation process for Sublime Text, ensure that you have a few things in place:

1. You need to have Ubuntu installed on your computer.
2. You should have an active internet connection.
3. You need to have administrative privileges to install software on your system.

## Steps for Installing Sublime Text on Ubuntu

1. Update the Package Index:

Open the terminal and type the following command to update the package index:

```sudo apt-get update```

2. Install Sublime Text:

Type the following command in the terminal to download the Sublime Text package:

```wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -```

3. Once you have downloaded the package, add the Sublime Text repository to Ubuntu:

```echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list```

4. Update the package index again:

```sudo apt-get update```

5. Finally, install Sublime Text:

```sudo apt-get install sublime-text```

6. Confirm that the installation was successful by launching Sublime Text:

```subl```

That's it! You've successfully installed Sublime Text on your Ubuntu system!

## Conclusion

In summary, Sublime Text is a powerful and easy-to-use editor that can help you enhance your coding productivity. By following the simple steps outlined in this article, you can quickly install Sublime Text on your Ubuntu system. Get started with coding today, and unlock the power of coding with Sublime Text!

{{< youtube 4rxgdxB6ySE >}} 



Sublime Text is one of the most popular text/code editors, and for good reason: you can extend its functionality by using hundreds of plug-ins. Let’s see how you can install Sublime Text on your Ubuntu-based distribution, enable Package Control, and install packages for your development needs.
 
## Install Sublime Text on Ubuntu
 
In the past, to install Sublime Text, you had to download its package from its official site and install it the manual way. Unfortunately, this meant that whenever there was an update available, you had to repeat the process.
 
Today, installing Sublime Text on any Ubuntu-based distribution is much easier. The easiest way is through the Software Center, where you only have to click on the “Install” button.
 
You might notice that this uses snap instead of apt. If you prefer to use the terminal, just enter the following command to install the Sublime Text snap package.
 
If you prefer “apt,” you will first have to add its repositories and security key:
 
The next step is to make sure apt can work with HTTPS sources:
 
Sublime Text offers two channels you can use for its updates: a “stable” and a “developer” one. You can choose the first by using:
 
We don’t suggest you use the developer version unless A) you are a developer, and, probably most importantly, B) you have paid for it. Yes, you can use Sublime Text for free, but officially you are supposed to pay for a license if you keep using it.
 
The developer version demands this license from the get-go, so, as we said, don’t choose it if you neither have a specific need for it nor have bought a license for the application.
 
If you have paid for it and have no problem with unforeseen consequences, due to the somewhat unstable nature of the developer version, choose it with:
 
For the contents of the repository to be accessible by apt, you first have to run an update:
 
Finally, install the program itself with:
 
After its installation completes, you can now find Sublime Text in your Applications menu.
 
## Installing Packages in Sublime Text
 
Before you start installing packages on Sublime Text, you have to install the main one, with which you will control them: Package Control. This is much easier than it sounds since you only have to select “Tools -> Install Package Control …”
 
After it’s installed, visit Sublime Text’s “Command Palette.” To do that, use the Ctrl + Shift + P shortcut on your keyboard.
 
Now you’re ready to start installing extra packages to extend Sublime Text’s functionality. Start by typing “install” in the command palette.
 
Choose “Package Control: Install Package” from the list of available options. After that, select the package you wish from the hundreds available and press Enter.
 
The Command Palette allows you to filter down the package list as well to help in pinpointing the ones you want. For example, if you type “HTML,” the package list will show only packages with that term in their name.
 
After a package is installed, if it needs to inform you about something or allows you to tweak some options, a new “Package Control Messages” document might pop up in Sublime Text’s main interface. In most cases, if you don’t care about being informed of every aspect of the software you use and don’t want to get too granular with its configuration, you can safely ignore them.
 
There are so many packages available that we couldn’t realistically list all of them. This also means that whatever you need, it will be there available for you to install and use. This is what makes Sublime Text so useful.
 
Are you using Sublime Text? If not, what alternative did you choose and why? Do you have any suggestions for other plug-ins we missed?
 
OK's real life started at around 10, when he got his first computer - a Commodore 128. Since then, he's been melting keycaps by typing 24/7, trying to spread The Word Of Tech to anyone interested enough to listen. Or, rather, read.
 
Our latest tutorials delivered straight to your inbox




