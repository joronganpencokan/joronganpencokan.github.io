---
title: "You Won't Believe How Easy It Is To Install And Use Snapcraft On Linux - Learn Now!"
ShowToc: true 
date: "2023-06-30"
author: "Louie Bent"
---
*****
Title: You Won't Believe How Easy It Is To Install And Use Snapcraft On Linux - Learn Now!

Introduction: 

Snapcraft is the modern package manager for Linux that offers a better way to install, manage and upgrade applications on your Linux distribution. It simplifies the packaging process for developers while providing users with quick and easy access to a growing library of software applications. In this article, we'll show you how easy it is to install and use Snapcraft on Linux so that you can start exploring this exciting platform.

Body: 

Step 1: Installing Snapcraft on Linux
To install Snapcraft on Linux, you need to open the terminal and execute the following command:

$ sudo apt install snapd snapcraft

This will install both snapd and snapcraft on your system, and you'll be able to create and access snaps, the universal Linux package format.

Step 2: Creating a Snap
Creating a snap is a straightforward process using Snapcraft. You must first create a snapcraft.yaml file that defines your application's dependencies, building process, and other information needed to package your app into a snap. You can use any text editor to create this file.

We will go through the process of creating a snap for a simple Python application named 'hello-world' using the following steps.

- Create a directory named 'hello-world-snap' and navigate to it.

$ mkdir hello-world-snap && cd hello-world-snap

- Create a file named 'hello.py' that contains a simple Python program:

print("Hello World!")

- Create a file named 'snapcraft.yaml' in the same directory and paste the following code:

name: hello-world
version: '1.0'
summary: A simple 'Hello World' Python application
description: This is a simple Python application that prints 'Hello World!'

parts:
  hello:
    plugin: python
    python-version: python3
    source: .
          
- Build the Snap package with Snapcraft.
 
$ snapcraft
 
- Install the Snap package using the following command:

$ sudo snap install hello-world_1.0_amd64.snap --devmode

Here's what we did:

- Created and navigated to a directory for the package called 'hello-world-snap'
- Created a simple Python program
- Wrote a 'snapcraft.yaml' file to provide information about your app to Snapcraft
- Created a snap by running the 'snapcraft' command
- Installed the 'hello-world' snap in devmode using the 'sudo snap install' command.

Step 3: Managing Snap packages
Now that you have installed a Snap, you can use the following commands to manage it:

List installed snaps:

$ snap list

Remove a snap:

$ sudo snap remove hello-world

Update a snap to the latest version:

$ sudo snap refresh hello-world

Conclusion:

Snapcraft is an easy-to-use tool that simplifies the process of creating, sharing, and installing snaps for Linux distributions. It provides a modern, efficient way for developers to package their applications and for users to access a vast selection of software packages. With the steps above, you have learned how to install and use Snapcraft on Linux. Now, you're ready to explore this exciting platform and develop your own Snap packages.

{{< youtube pK4TKT3OaNQ >}} 



Have you ever wondered how some Linux distributions make it so easy to install software while others can be quite difficult? The difference is in the package format that they use. Some distributions use .deb files while others use .rpm.
 
But what if there was a package format that could be used on any distribution? That’s where Snapcraft comes in. In this tutorial, you will learn how to install and use Snapcraft to create and install snap packages in Linux.
 
## What Is a Snap Package?
 
A snap package is a self-contained application package that includes all the necessary dependencies and libraries, making it easy to install and update applications without having to worry about dependency issues.
 
## Why Use Snap Packages?
 
There are several advantages to using snap packages:
 
- Snaps are easy to install and update. You can install a snap package with a single command, and snaps are automatically updated in the background.Snaps are safe and secure. Since all the dependencies are included in the snap package, there is no risk of a dependency conflict. Also, snaps are isolated from the rest of the system, so they cannot access your data or other applications on your system.

 
- You can install your favorite app on any Linux distribution that supports snaps.

 
## Installing Snapd in Linux
 
Snapd is a daemon that enables the installation and use of snaps and needs to be installed before you can use Snapcraft. When you install Snapd, it also installs a command line interface (CLI) tool called snap. You can use this tool to manage your snaps.
 
To install Snapd on Ubuntu, open a terminal and enter the following command, entering your user password when prompted.
 
On CentOS, you’ll need to enable the EPEL repository before you can install Snapd. To do this, first enter the following command in your terminal:
 
Then, install Snapd with the below command. Enter the password for the sudo user when prompted.
 
In Fedora, install with the command:
 
In Arch Linux, install snapd from AUR. Check out these AUR helpers to help you install third-party packages easily.
 
Once the installation completes, run the below command to enable the snapd.socket systemd unit. This ensures that the Snapd daemon starts automatically when your system boots up.
 
Create a symbolic link between “/var/lib/snapd/snap” and “/snap” to enable the classic snap support.
 
Now that you have installed the Snapd on your Linux system, check the version of the Snapd with the below command. You will see an output similar to the following.
 
You can also check the status of the Snapd service with the followng command.
 
## Installing Snapcraft
 
Before you can create snap packages, you need to install Snapcraft, the tool used for building snap packages.
 
To install Snapcraft on Linux, run the following command. The classic flag tells snap to use the classic confinement mode. This flag is required since Snapcraft doesn’t support the newer, more restrictive confinement mode yet.
 
Verify that Snapcraft is installed by checking the version number.
 
## Using Snapcraft to Build a Snap Package
 
Now for the interesting part: using Snapcraft to create a snap package for an application. In this tutorial, we are creating a basic hello-world snap, a simple snap that prints “Hello, world!” when you run it. After you complete this tutorial, apply the same process to create snaps for your own applications.
 
For the sake of simplicity, the steps below will guide you through the process of creating a snap in Ubuntu. The same steps can be applied on other Linux distros as well.
 
### Starting a Project for Your Snap
 
First create a project directory for your snap. It will be the working directory for your project and helps you keep your project files organized.
 
- Create a project directory named “hello” with the following command:

 
The -p flag tells the mkdir command to create any parent directories that don’t already exist. In this case, the mysnaps directory will be created if it doesn’t exist. You can put any future snaps inside this directory.
 
- Move into the newly created project directory and initialize the project with the init  command to create a file named “snapcraft.yaml” in your project directory. You can use the “snapcraft.yaml” file to configure your snap later.

 
- Check the structure of your project with the tree command, which prints a graphical representation of your project directory.

 
You will see an output similar to the following.
 
### Adding Top-Level Metadata
 
Snapcraft provides many metadata that you can use to describe your snap package. In this tutorial, we add some basic info that is required for every snap.
 
- Open the “snapcraft.yaml” file in your favorite text editor. We used nano in this tutorial.

 
- Delete the placeholder lines and replace them with the following content.

 
Here we changed the info of our snap. The core18 base tells Snapcraft that you want to build a snap based on Ubuntu Core 18. The confinement: devmode metadata tells Snapcraft that you want to build a snap that is not confined, which is useful for development and testing purposes.
 
### Exposing Your Application
 
- Add the following lines after the confinement field in your “snapcraft.yaml” file. Here we specify the application we want to package.

 
In this case, we only have one app, hello. The command line tells Snapcraft which binary to run when the snap is installed.
 
### Adding a Part
 
- In a new line, add the following parts command:

 
This tells Snapcraft which software you want to include in your snap package.
 
To build this hello-world snap, you need to download the source code of GNU Hello, then use the autotool plugin to build the application from source.
 
- At this point, your snapcraft.yaml file will look like the one below.  Save and close the snapcraft.yaml file before you move on to the next step.

 
### Building the Snap Package
 
Now that you have defined your snap, it’s time to build it. To build a snap package, run the following command.
 
You will be asked to install “multipass” if you don’t have it on your system. Snapcraft uses multipass to create an isolated environment for building snaps within a virtual machine. Type y and press Enter to continue.
 
The building process may take a while, depending on your Internet connection and computer specs. Once the building process is finished, you will see something similar to the following output.
 
In the end, you will find a “hello_2.10_amd64.snap” in the project directory.
 
### Testing the Snap Package
 
To test whether your snap package is working, run the following command:
 
The --devmode flag tells snap that you want to install the snap in devmode, which is useful for testing purposes.
 
Next, run the following command to run your hello-world application.
 
You will see the following output, which indicates that your hello-world snap is working as expected.
 
To see the version of your hello-world application, run the following command.
 
If you encounter an issue while testing the snap, get more information by using the --debug flag and running the following command.
 
## Frequently Asked Questions
 
Image credit: Freepik. All screenshots by Nicholas Xuan Nguyen.
 
### Is Snapcraft safe?
 
Absolutely! Snapcraft is the official tool for building snaps. It is developed and maintained by Canonical, the company behind Ubuntu. Rest assured that Snapcraft is safe and reliable.
 
### Is Snap like Docker?
 
Yes and no. Snap and Docker are both container technologies but serve different purposes. Think of Snap as a packaging format for your application and Docker as a runtime environment for your application. You can set up WordPress with Nginx and PHP in a Docker container using the official WordPress and Nginx images but can’t create a Snap package for your WordPress site.
 
### Is snap better than apt or apt-get?
 
It depends. Both systems have their own advantages and disadvantages. Apt and apt-get is the traditional package manager for Debian-based Linux distributions. It has been around for a long time and is very stable, yet it has a few drawbacks. For instance, apt does not support versioning and rollback. Snap, on the other hand, supports both versioning and rollback. So if you want to experiment with new versions of your application, Snap is the way to go. But if you want a stable system, apt and apt-get is the better choice.
 
I am a big fan of Linux and open source software. I have been using Linux for over a decade and I absolutely love it. I am also a big fan of writing. In my spare time, I enjoy reading, playing video games.
 
Our latest tutorials delivered straight to your inbox




