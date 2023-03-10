---
title: "Unleash the Power of Ubuntu with This Simple Guide to Installing Gcc!"
ShowToc: true 
date: "2023-04-11"
author: "Frances Jackson"
---
*****
# Unleash the Power of Ubuntu with This Simple Guide to Installing Gcc!

If you're looking to harness the power and flexibility of the Ubuntu operating system, installing Gcc (GNU Compiler Collection) is an absolute must. Whether you're a seasoned programmer looking to develop complex software applications or a student just starting out with computer science, Gcc is an essential tool that you need to have in your toolbox.

In this guide, we'll walk you through the step-by-step process of installing Gcc on Ubuntu, from start to finish. Whether you're a complete beginner or an experienced Ubuntu user, we guarantee that this guide will help you get up and running with Gcc in no time at all.

## Before You Begin

Before you can install Gcc on Ubuntu, you'll first need to have the Ubuntu operating system installed on your machine. If you haven't installed Ubuntu yet, don't worry – it's a quick and easy process that you can complete in just a few minutes.

To install Ubuntu, simply visit the official Ubuntu website and follow the instructions to download and install the operating system onto your machine. Once you have Ubuntu installed, you're ready to move on to the next step.

## Step 1: Update Your System

Before you can install Gcc, you should make sure that your Ubuntu system is up to date. This will ensure that you have the latest security patches and bug fixes installed, which will help to prevent any potential conflicts or problems when you install Gcc.

To update your system, simply open the terminal and run the following command:

```
sudo apt-get update && sudo apt-get upgrade
```

This will update your system to the latest version of Ubuntu, including any security patches and bug fixes that have been released since your last update.

## Step 2: Install Gcc

Now that your system is up to date, it's time to install Gcc. To do this, open the terminal and run the following command:

```
sudo apt-get install build-essential
```

This command will install a package called 'build-essential', which includes Gcc along with several other essential development tools that you'll need if you're planning to code on Ubuntu.

Once the installation is complete, you'll have Gcc installed on your Ubuntu system and ready to use.

## Step 3: Verify Your Installation

To verify that Gcc has been installed correctly, open the terminal and run the following command:

```
gcc --version
```

This will display the version of Gcc that has been installed on your system, along with some other information about the compiler.

If Gcc is installed correctly, you should see a message that looks something like this:

```
gcc (Ubuntu 7.5.0-3ubuntu1~18.04) 7.5.0
Copyright (C) 2017 Free Software Foundation, Inc.
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
```

Congratulations – you've now successfully installed Gcc on your Ubuntu system!

## Conclusion

In this guide, we've shown you how to install Gcc on Ubuntu, from start to finish. By following these simple steps, you can quickly and easily set up Gcc on your Ubuntu system and start using it to create amazing software applications.

Whether you're a beginner or an experienced developer, Gcc is an essential tool that you need to have in your arsenal. So why wait? Install Gcc on your Ubuntu system today and start unleashing the full power of Ubuntu!

{{< youtube oNEwEQ0uU1Y >}} 



GCC is one of the favorite tools used by developers working on the Linux platform. It serves as an integration of several compilers for popular programming languages such as Java, C, C++, Fortran, and many more. If you are beginning your journey with Linux, what better option there is than Ubuntu. Ubuntu is the most famous of all Linux distribution out there. It is known to be easy to learn while not compromising on the features front of things. So, if you are in need to know how to install GCC on your Ubuntu system, this article is the perfect place to start. We will explore how to download and install GCC on Ubuntu in the sections below. But before that let’s know more about GCC.
 

 
## How to Install GCC on Ubuntu
 
GCC (GNU Compiler Collection) is a set of tools for compiling source code from various programming languages into binaries, executables, or libraries. GCC is a command-line compiler that may be installed on Ubuntu.
 
Contents
 
- How to Install GCC on Ubuntu
 - Method 1: Through Ubuntu Terminal
 - Option 1: Install a Particular GCC Version
 - Option 2: Install Multiple GCC Versions
 - Method 2: Through Synaptic Package Manager
 - Option 1: Install a Particular GCC Version
 - Option 2: Install Multiple GCC Versions

 
- The GCC compiler, as well as many libraries and other tools necessary for generating applications, is included in the default Ubuntu repository as build-essential.
 - C, C++, Java, Objective-C, Go, Fortran, Ada, and more programming languages are supported by GCC.
 - Many open-source projects, including the GNU utilities and the Linux kernel, require GCC to build their code.

 
This tutorial will show you how to set up the GCC compiler on Ubuntu 18.04. We’ll teach you how to install the stable version of the distribution as well as the most recent version of GCC. The steps are the same for Ubuntu 16.04 and any Ubuntu-based distribution, such as Kubuntu, Linux Mint, and Elementary OS.
 
Note: You must be logged in as root or a user with sudo privileges to create new repositories and install packages on your Ubuntu system.
 
### Method 1: Through Ubuntu Terminal
 
To set up GCC on Ubuntu, you’ll need to download and install the build-essential package. Open a terminal window to download gcc ubuntu. Follow the given steps to install GCC on Ubuntu through the Terminal.
 
#### Option 1: Install a Particular GCC Version
 
1. Press Ctrl + Alt + T keys together to launch a terminal window on the Desktop.
 
Note: Alternatively, go to the app menu and search for Terminal.
 
2. Use the install command below to install the build-essential package on Ubuntu once the terminal window is open.
 
sudo apt install build-essential
 
Note: The Sudo command prompts you for your password. Users can use this command to run a single task as root.
 
3. Ubuntu will prompt you for your password. Enter your user password to continue.
 
4. The terminal prompt will gather all dependencies for the build-essential package once you’ve supplied your password. Ubuntu will next ask you whether or not you wish to install the package. To proceed, press the Y key. When you hit the Y key, Ubuntu will begin installing GCC on your machine.
 
5. This procedure should take no more than a few minutes. With the man gcc command, you may browse the GCC documentation after the procedure is complete.
 
Also Read: Top 14 Best Graphics Card for Linux
 
#### Option 2: Install Multiple GCC Versions
 
While most Ubuntu users will be satisfied with the build-essential package because it contains GCC 10, it is not the only version of GCC available. Support for additional languages, improved performance, and expanded functionality are all included in newer versions of the GCC compiler. You have the option of installing various versions of GCC on Ubuntu. Here’s how to download gcc ubuntu.
 
1. First, on the Ubuntu desktop, open a terminal window.
 
2. Once it’s open, use the following command to search the Ubuntu software repositories for available GCC packages:
 
apt search gcc
 
3. Search through the prompt for the GCC version you want to install on Ubuntu. GCC 7, GCC 8, 9, and 10 will be available for installation.
 
4. Install GCC using the apt install instructions below once you’ve found the version you want to install on your Ubuntu PC. gcc-7, gcc-8, gcc-9, and gcc-10 are GCC packages.
 
5. To install the GCC version 7 on Ubuntu.
 
sudo apt install gcc-7 g++-7
 
6. To install GCC version 8 on Ubuntu.
 
sudo apt install gcc-8 g++-8
 
7. To install the GCC version 9 on Ubuntu.
 
sudo apt install gcc-9 g++-9
 
8. While installing the build-essential package is strongly recommended for getting GCC 10 to operate on Ubuntu, it isn’t the only option to do it. Installing the gcc-10 and g++-10 packages will also install GCC 10.
 
sudo apt install gcc-10 g++-10 
 
Also Read: 20 Best Lightweight Linux Distros of 2022
 
### Method 2: Through Synaptic Package Manager
 
If you don’t want to use the console to install GCC on Ubuntu, you may use the Synaptic Package Manager instead to download GCC in ubuntu.
 
Follow these steps to install GCC through Synaptic Package Manager.
 
1. To begin, make sure Synaptic is installed. To get Synaptic, go to the Ubuntu Software program and search for Synaptic, then install it.
 
2. Open the Synaptic Package Manager by searching for it in the app menu once it has been installed.
 
3. Then, in the top-right corner of the screen, look for the search button.
 
4. To display the search results, pick the Synaptic search button and input build-essential followed by the Enter key.
 
5. Look through Synaptic search results for build-essential.
 
6. Once you’ve identified it, right-click on it and choose the Designate for installation option to mark the build-essential package for Synaptic installation.
 
7. In Synaptic, locate the Apply button and click it to begin the GCC installation on Ubuntu.
 
Also Read: How To Install Linux Bash Shell On Windows 10
 
#### Option 2: Install Multiple GCC Versions 
 
To install a GCC version other than the one supplied with the build-essential package in Ubuntu, perform the steps below.
 
1. First, open Synaptic Package Manager.
 
2. Once Synaptic is open, click on the search button.
 
3. Then select one of the products from the list below and enter it into the search box.
 
- GCC 7: gcc-7, g++-7
 - GCC 8: gcc-8, g++-8
 - GCC 9: gcc-9, g++-9
 - GCC 10: gcc-10, g++-10

 
4. To install the GCC package(s) you’ve found in Synaptic, right-click on it and pick the Apply button.
 
5. Repeat this procedure as needed to install as many versions of GCC as you like on Ubuntu.
 
Q1. Is GCC already installed on your Ubuntu?
 
Ans. On all Ubuntu desktop variants, the GCC package is installed by default.
 
Q2. Which command is used to install GCC?
 
Ans. Install GNI C/C++ (GCC) and needed libs using the up2date command, yum command, or apt-get command, depending on your Linux distro.
 
Q3. What is the purpose of Ubuntu?
 
Ans. Ubuntu has everything you’ll need to manage your company, school, house, or business. All of the main software, like an office suite, browsers, email, and media apps, are pre-installed, and the Ubuntu Software Centre has hundreds of additional games and applications.
 
Recommended:
 
- How to Find Sleep Button on Windows 10
 - How to Send GIFs in Slack
 - How to Keep Microsoft Teams Status Available
 - How to Send Skype Code with Proper Format

 
We hope this article will prove to be helpful in finding out how to install gcc Ubuntu. You can find many more articles related to tech on our website. If you have any suggestions or feedback regarding this article, you can reach out to us in the comment section below.




