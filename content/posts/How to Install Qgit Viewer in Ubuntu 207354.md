---
title: "Discover the Ultimate Guide to Installing Qgit Viewer in Ubuntu - A Game-Changer for Linux Enthusiasts!"
ShowToc: true 
date: "2023-02-09"
author: "Edith Chalepah"
---
*****
# Discover the Ultimate Guide to Installing Qgit Viewer in Ubuntu - A Game-Changer for Linux Enthusiasts!

For all Linux enthusiasts and developers, Qgit Viewer is a game-changer. It is an easy-to-use git repository viewer that simplifies tracking changes in your code repositories. Here we discuss how to install Qgit Viewer on Ubuntu, the ultimate guide to mastering Qgit Viewer.

## What is Qgit Viewer?

Before we dive into how to install Qgit Viewer, it is important to understand what it is and why you need it. Qgit Viewer is an open-source Git repository viewer that shows how the repository has evolved over time. It helps developers understand the history of their code and its changes over time. It is an essential tool for all developers working with Git repositories.

## Installing Qgit Viewer on Ubuntu

Now that you understand the importance of Qgit Viewer let's get started with the installation process. Here are the steps to install Qgit Viewer on Ubuntu.

### Step 1: Update your system

The first step in any installation process is to ensure that your system is up-to-date. Run the following command to update your Ubuntu system:

```
sudo apt-get update && sudo apt-get upgrade -y
```

### Step 2: Install Qgit Viewer

Once your system is up-to-date, you can start the installation process for Qgit Viewer. Run the following command to install Qgit Viewer:

```
sudo apt-get install qgit
```

### Step 3: Verify the installation

After the installation is complete, you can verify if Qgit Viewer has been installed successfully. Run the following command to check if Qgit Viewer is installed:

```
qgit --version
```

### Step 4: Launch Qgit Viewer

After verifying the installation, launch Qgit Viewer by running the following command:

```
qgit
```

## Using Qgit Viewer

Now that you have successfully installed Qgit Viewer on your Ubuntu system, let's learn how to use it.

### Step 1: Open a repository

To open a repository in Qgit Viewer, click on the File menu and then select Open. Navigate to the repository you want to open and click Open.

### Step 2: Navigate the repository

Once you have opened the repository, you can use the navigation panel on the left to browse through the repository history. You can view the commits, changes, and branches of the repository.

### Step 3: View commits

To view the commits of the repository, click on the Commits tab in the navigation panel. This will display all the commits in the repository.

### Step 4: View changes

To view the changes made in a commit, select the commit in the Commits tab, and then click on the Changes tab in the right panel.

### Step 5: View branches

To view the different branches in the repository, click on the Branches tab in the navigation panel.

## Conclusion

Qgit Viewer is an essential tool for all developers working with Git repositories. It simplifies the process of tracking changes in your code repositories. With this ultimate guide, you can install and master Qgit Viewer on your Ubuntu system. So go ahead and install Qgit Viewer today and take your Linux development game to the next level!

{{< youtube mCzJG-JG9ec >}} 



Git is a useful tool for developers, as it makes it very easy to control versions of software, issue patches, and contribute upstream. Though, for as helpful as Git is,  a lot of interaction with Git is done with the command line, and it is tedious.
 
For those that love to use Git but don’t want to deal with the command line on Linux, there is Qgit Viewer – a Qt-based Git-viewing tool for Linux. With it, users can access Git repos to contribute code, patches and everything that the command line version of Git can do!
 
Let’s discuss how to install it.
 
## Preparing Qgit
 
Various Qt4 libraries and components are needed before the program builds. The program will not build correctly without these tools. The developer has failed to really list the exact components the user needs (in extreme detail). It is because of this that the best course of action is to use a wildcard in the terminal and use it to install everything Qt4 related.
 
When the command completes, Qgit Viewer will be able to compile correctly. Get the source code for Qgit Viewer.
 

 
Extract the source code. Open a terminal and enter the source code directory.
 
## Compiling Qgit Viewer
 
First, run the qmake command. This command will create the makefile. A makefile is key in the compiling process.
 
Qmake has created a Makefile. Run the make command to start the compilation of Qgit Viewer.
 
Finally, to finish the compilation process, run the make command again but with the install command to finish the compiling process.
 
After the qmake, make and make install commands have run through, a new folder in the “qmake” directory will appear labeled “bin.” This folder contains the fully compiled Linux binary for use on Ubuntu.
 
## Running Qgit viewer
 
To run Qgit Viewer, double-click on it (or right-click, then execute). The compiler should automatically set the correct permissions to allow the binary to run and execute as a program, so there’s no need to fiddle with it.
 
Another way (and perhaps the best way) to run Qgit the first time is to run it from the terminal window itself. This is because the Linux terminal can output any errors directly, let the user know of missing dependencies, etc. To run Qgit from the terminal, enter the following:
 
## Making a desktop icon
 
Creating a desktop icon for Qgit Viewer will help the program open more easily. To start, enter the Qgit bin directory with the terminal.
 
Move the binary file to the /usr/bin/ directory.
 
The Qgit binary is in the right place. Now, let’s make the desktop icon. Open Gedit and paste the following into it.
 
Save the file as “qgit-viewer.desktop.” Then, locate the saved desktop file. Right-click the file, select “Properties,” then the permissions tab. Check the box “allow executing file as a program,” and close the window.
 
Place the desktop file in the application directory with:
 
## Conclusion
 
With the Desktop icon made and everything taken care of, Qgit Viewer is installed on the Ubuntu desktop. From here, code patches, code contributions, and everything in-between can now be done with a nice GUI tool. So long as Git is configured on the system, everything should run smoothly!
 
Derrik Diener is a freelance technology blogger.
 
Our latest tutorials delivered straight to your inbox




