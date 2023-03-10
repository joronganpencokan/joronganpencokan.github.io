---
title: "Unlock the Secret to Hacking like a Pro with this Step-by-Step Guide to Installing Metasploit on Ubuntu Linux!"
ShowToc: true 
date: "2023-05-25"
author: "Robert Brown"
---
*****
Introduction

Hacking is a highly popular topic in the tech world, and many individuals are interested in learning how to do it. However, that can be quite difficult if you don't know where to start or you're overwhelmed by the multitude of available tools. If you're interested in becoming a professional hacker or simply want to learn how to hack for fun, you'll need to start by installing a powerful tool known as Metasploit.

In this article, we'll guide you through the process of installing Metasploit on Ubuntu Linux in just a few simple steps.

What is Metasploit?

Metasploit is a powerful tool that allows you to perform penetration testing (pen-testing), vulnerability assessment, and exploit development. It's open-source software that contains a vast array of tools that make it easier for users to hack into systems and exploit vulnerabilities. Metasploit is one of the most popular hacking tools, and the tool of choice for many professionals in the industry.

Getting Started with Installing Metasploit

Before you begin installing Metasploit on your Ubuntu Linux machine, you'll need to ensure that your Ubuntu system is up-to-date. You can do this by running the following command:

$ sudo apt-get update && sudo apt-get upgrade

Once you've run the above command, you're ready to start installing Metasploit on your Ubuntu Linux machine. Let's get started!

Step 1: Install PostgreSQL Database

Metasploit requires a PostgreSQL database to run. To install PostgreSQL on your Ubuntu machine, run the following command:

$ sudo apt-get install postgresql postgresql-contrib libpq-dev

Once PostgreSQL is installed, you'll need to configure it. Run the following command to create a new user for Metasploit:

$ sudo -u postgres createuser msf -P -S -R -D

After executing the above command, you'll be asked for a password. Enter a strong password and remember it as you'll need it later.

Step 2: Install Metasploit Framework

Now that you've installed PostgreSQL on your Ubuntu machine and configured it to work with Metasploit, it's time to install Metasploit itself.

To install Metasploit Framework, run the following command:

$ sudo apt-get install metasploit-framework

This command will install Metasploit Framework along with all the necessary dependencies. It may take a while for the installation process to complete, so be patient.

Step 3: Start Metasploit Framework

After the installation of Metasploit Framework is complete, you're ready to start using it. To start Metasploit Framework, run the following command:

$ sudo msfconsole

This command will launch the Metasploit console, which is where you'll be able to start using the tool.

Congratulations! You've successfully installed Metasploit Framework on your Ubuntu Linux machine!

Conclusion

Installing Metasploit Framework on Ubuntu Linux is a simple process that only requires a few steps. Once you've installed it, you'll have access to a powerful tool that will allow you to perform pen-testing, vulnerability assessments, and exploit development. With Metasploit Framework, you can become a pro hacker and impress your friends and colleagues.

So, what are you waiting for? Start using Metasploit Framework today and unlock the secrets to hacking like a pro!

{{< youtube K7y_-JtpZ7I >}} 



Metasploit is a collection of exploits, payloads and virtual environments for the Linux operating system. Among other things, it allows you to create your own toolkit for security auditing and penetration testing.
 
This tutorial shows how to install it in Ubuntu Linux, how it works, and what you can do with this powerful security auditing tool.
 
## What Is Metasploit?
 
Metasploit is a free open-source tool for developing and executing exploit code. It comes with a large database of exploits for a variety of platforms and can be used to test the security of systems and look for vulnerabilities.
 
It is a framework rather than a single tool and includes a wide range of tools for conducting penetration tests and security research.
 
Features of Metasploit:
 
- Develops exploit code
 - Automated security testing
 - Reverse engineering
 - Password cracking
 - Social engineering

 
Note: you can’t just learn penetration testing without knowing what Kali Linux is. Learn all about Kali Linux and its full suite of penetration tools.
 
## Why Use the Metasploit Framework
 
One of the biggest advantages of Metasploit is that it is a single, cohesive software suite. Similar to an integrated development environment, the Metasploit Framework links together different tools and allows you to use them through a common interface.
 
Metasploit also categorizes each tool depending on its use case, making it useful not only to security experts but also to novice users.
 
The developers of the Metasploit Framework designed the software suite to be completely modular and extensible. You can create and design a highly custom toolkit for any specific target.
 
## Requirements
 
Before you can install Metasploit, make sure that you have the following resources:
 
- Good amount of hard disk space. For the most part, you should allot between 10 to 20 GB of disk space for Metasploit, as the framework will create its own environment, along with its dependencies.
 - 4 to 8 GB of system memory
 - Machine that is capable of virtualization, allowing you to create isolated environments to test Metasploit.

 
## Installing the Metasploit Framework in Linux
 
- Make sure that you have the necessary dependencies, such as curl by running the following command:

 
- Create a temporary directory where you can download Metasploit’s installation script.

 
- Download the installation script by running the following command:

 
- Make sure that your installation script has the right execution bits by running the following command:

 
- Run the installation script to install metasploit:

 
For the most part, the script does three things in your machine. First, it imports the signing key from the Metasploit Frameworks developers.
 
The script, then, copies the repository address for Metasploit to your “/etc/apt.d/sources.list” directory. Lastly, it downloads the Metasploit package through apt and corrects the PATH variable for the package.
 
- Configure your Metasploit environment by running msfconsole.

 
The Metasploit console will ask a couple of questions about your setup. First, it will ask if you want to set up a database for your installation by pressing  Y, then Enter.
 
You will also be asked if you want to create a remote web service. This is useful if you want to create a headless instance for Metasploit. Press Enter here if you only want the program to run locally.
 
The console will create and configure the necessary files to run Metasploit. This process should take one to two minutes, and then the console will reload itself and load the Metasploit prompt.
 
## Installing the Metasploitable Virtual Machine
 
Once the Metasploit Framework is up and running, start installing the Metasploitable virtual machine, a basic Linux distribution designed to be as insecure as possible.
 
- Install VirtualBox: a virtual machine client that can be used to run the virtual machine.

 
- Download the Metasploitable distribution from the developer’s sourceforge webpage.

 
- Extract the distribution’s files to your home directory and convert the distribution’s hard disk format for it to work with VirtualBox. Metasploitable is a pre-built bundle that works similarly to importing an Open Virtual Appliance.

 
Accomplish this by running the following commands:
 
- Open VirtualBox by pressing Win, then typing “virtualbox.”

 
- Press the “New” button to open a dialog box where you provide the details of your virtual machine. Add the name and set the Type to “Linux” and the Version to “Other Linux (64-bit).”

 
- Specify the amount of memory for the Metasploitable virtual machine. In most cases, a memory size between 512MB and 1G is enough.

 
- Select the hard disk file for your virtual machine. For this, select the “Use an existing virtual hard disk file” option.

 
## Using Metasploit and Metasploitable in Linux
 
With the virtual machine in your system, you can now open Metasploitable 2 to test the Metasploit Framework. To do this, double-click the “metasploitable” entry in VirtualBox.
 
This will load the virtual machine and expose it to a local internal network.
 
Once it is done loading, log in to Metasploitable by typing msfadmin on both the username and the password prompts.
 
## Learning the Basics of Metasploit
 
While the Metasploit Framework is a brilliant security auditing toolkit, it is also a great learning tool for beginners, as the framework provides a good amount of documentation for every function.
 
To access this, run msfconsole again on your terminal window.
 
This will load a console prompt that can access both your system programs and the Metasploit toolkit. Run the help command to print a short guide on the various commands for the Metasploit Framework.
 
As discussed above, you can use the framework at every step of a penetration test. It gives you tools to conduct both information gathering through network scripts, machine access through exploits and system breach through payloads.
 
These tools also vary widely depending on the architecture that you are targeting, which makes Metasploit incredibly flexible and adaptable.
 
You can use the show -h command to create a brief list of every tool that is available to Metasploit. For example, you can run the following command to list all of the available exploits in the framework:
 
Further, Metasploit also provides tool-specific documentation through the info command. Running info exploit/android/adb/adb_server_exec will print a short write-up on how this particular Android ADB exploit works.
 
### Scanning Open Network Ports with Metasploit
 
One of the most basic actions that you can immediately do in Metasploit is to determine whether there are any insecure open ports in a target system.
 
- Reload Metasploit by running msfconsole on a new terminal.

 
- Check whether the Metasploit Framework detects the virtual machine. But first, determine the IP address of the Metasploitable installation:

 
- Use the nmap utility in your host machine to create a network-wide scan for active hosts:

 
- Once you see the virtual machine in the nmap result, you can use the tcp module in Metasploit. It’s a simple utility that checks for every open port from either a single IP address or a range of them.

 
To use the tcp module, run the following command:
 
- Provide the IP address that you want the module to scan by running the following command:

 
- Run the tcp module by entering run in the console, which will print every open port in the Metasploitable system.

 
## Frequently Asked Questions
 
Image credit: Unsplash. All alterations and screenshots by Ramces Red.
 
### Is it possible to check if an exploit is present in Metasploit Framework?
 
Yes! You can check all of the available exploits by using the “search” command in the Metasploit console. For example, you can run search android to load every available exploit for the Android platform in Linux.
 
### My Metasploitable virtual machine does not boot. Is my installation broken?
 
No! This issue is most likely due to a missing VirtualBox configuration. By default, VirtualBox automatically sets the necessary processor flags to boot a virtual machine. However, there can be instances where it does not enable these flags properly.
 
To fix this, go to the Settings menu for Metasploitable. Click on “System -> Processor,” then click the “Enable PAE/NX” checkbox and reload VirtualBox.
 
### My host machine cannot detect Metasploitable. Is my virtual machine broken?
 
No! This issue happens whenever VirtualBox uses a different network adapter with your host machine. You can easily fix this issue by going to the Settings menu and selecting the Network category, then changing the Network Adapter from NAT to Bridged Adapter.
 
Ramces is a technology writer that lived with computers all his life. A prolific reader and a student of Anthropology, he is an eccentric character that writes articles about Linux and anything *nix.
 
Our latest tutorials delivered straight to your inbox




