---
title: "Revolutionize Your Ubuntu Linux Experience With This Incredible Webmin Installation Guide!"
ShowToc: true 
date: "2023-05-28"
author: "Denise Arreola"
---
*****
# Revolutionize Your Ubuntu Linux Experience With This Incredible Webmin Installation Guide!
---

Webmin is an open-source web-based management tool for Linux operating systems. It allows system administrators to manage Unix-like servers, including Ubuntu, using a web interface. In this article, we’ll guide you through the installation process of Webmin on Ubuntu Linux, so you can manage your server with ease.

## First things first: update your system
Before proceeding with the installation, you need to ensure that your Ubuntu system is up to date. This will help prevent any package conflicts that might arise during the installation of Webmin.

To update your system, open a terminal window and type the following command:

```
sudo apt update && sudo apt upgrade -y
```

This will update all the packages on your system and install any pending updates.

## Installing Webmin
Now that your system is up to date, you can proceed with the installation of Webmin. Follow the steps below to get started:

### Step 1: Add the Webmin repository
Webmin is not available in the official Ubuntu repositories, so you’ll need to add the Webmin repository to your sources list. To do this, type the following command in your terminal window:

```
echo "deb http://download.webmin.com/download/repository sarge contrib" | sudo tee /etc/apt/sources.list.d/webmin.list
```

This command will add the Webmin repository to your sources list.

### Step 2: Add the Webmin GPG key
Next, you’ll need to add the Webmin GPG key to your system. This key is used to verify the Webmin installation package.

To add the key, type the following command in your terminal window:

```
wget -q http://www.webmin.com/jcameron-key.asc -O- | sudo apt-key add -
```

This command will download the Webmin GPG key and add it to your system.

### Step 3: Install Webmin
Now that you’ve added the Webmin repository and GPG key to your system, you can install Webmin using the following command:

```
sudo apt update
sudo apt install webmin
```

This command will update your package list, and then install Webmin.

## Accessing Webmin
Once you’ve installed Webmin, you can access it by opening a web browser and entering the following URL: `https://your_server_ip:10000`

Replace `your_server_ip` with the IP address of your Ubuntu server. You’ll also need to add a security exception to your browser to proceed.

After you’ve added the exception, you’ll see the Webmin login screen. Enter your administrative username and password to log in and start using Webmin.

## Conclusion
In this article, we covered the basics of installing Webmin on Ubuntu Linux. With this powerful tool, you can manage your Ubuntu server with ease from a web interface. We hope this guide has been helpful in revolutionizing your Ubuntu Linux experience. Happy managing!

{{< youtube ZG7E5G_rM8M >}} 



Webmin is a powerful web front-end interface for Linux servers. It allows you to easily configure any system setting in your machine through a web browser. This makes Webmin a highly attractive utility for system administrators who want an accessible way to check on their remote machines. Here we show how to install and use Webmin on Ubuntu.
 
## What Makes Webmin Different?
 
One of the biggest advantages of Webmin is that it allows you to directly configure third-party services in your server. You will not need to memorize each configuration file for each service that you use in your machine.
 
Webmin also allows you to configure deep system files in your machine. For example, it is possible to configure your GRUB Bootloader directly from Webmin’s interface.
 
## Installing Webmin in Linux
 
Before you can install Webmin, you need to make sure that you have the following resources available and ready:
 
- Machine that you can access over the network, such as a local machine in your home or a VPS that you rent online.
 - Compatible Linux distribution in your machine that supports a wide range of Linux distributions. We are using Ubuntu.
 - Root access in your machine, to be used for configuring system files during the installation process.

 
### Obtaining Webmin’s Dependencies
 
The first step in installing Webmin is to import its repository archive, as Webmin is not included by default in Ubuntu 22.04.
 
To import the Webmin repository, copy the developer’s signing key:
 
Copy the repository information for Webmin to your /etc/apt/sources.list.d file:
 
Lastly, update apt to refresh your system’s repository listings:
 
### Configuring Your Firewall and Installing the Program
 
Make sure that Webmin is accessible from outside the server by using the iptables utility to enable port 10000 for incoming connections:
 
Lastly, install the Webmin utility with the following command:
 
## Managing Your System With Webmin
 
Once you have properly installed Webmin in your server, you can start configuring your system through it. However, you need to first find the IP address of your server.
 
Do that by running the following command:
 
After that, you can now open Webmin by going through your web browser and typing the machine’s IP address followed by the program’s port. In my case, I will type 192.168.68.165:10000.
 
A small login page for Webmin will open. To access the system, provide your current Ubuntu credentials. For example, I am typing user “ramces” followed by my password to access the Webmin interface.
 
### Installing a Service Using Webmin
 
Once inside, Webmin will display a visual dashboard of your system with a brief summary of your machine and how it utilizes its resources.
 
The visual dashboard also allows you to easily install and remove third-party services from your server by clicking the “Un-used Modules” category in the Dashboard’s left sidebar.
 
Webmin will list all of the available services that you can install. For example, I can click the “Apache Webserver” item to set up a web server in my machine.
 
Doing that will display a new page where Webmin will ask if you want to install a new service in your server. To begin the installation, click the “Install Now” button.
 
Webmin will list all the dependencies it needs to properly build the service that you want to install. To continue, click the “Install Now” button again.
 
The program will create a new terminal instance and run all of the commands that it needs to install your service. Click the “Return” button at the bottom of the current page to load your new service.
 
Tip: you can also learn how to configure Apache and PHP for a high traffic site.
 
### Configuring a System Setting Using Webmin
 
Another brilliant use of Webmin is configuring system files and services through its interface. This approach removes the need to constantly access the system through SSH for relatively minor tweaks and configurations.
 
Click the “System” category in the Dashboard’s left sidebar.
 
Webmin will display all the available system settings that you can tweak through its interface. For example, I can select the “Users and Groups” item to either modify a user or add a group in the server.
 
Doing that will load a new page where it lists all of the active user accounts and groups in the system. To add a new user, click the “Create a New User” button.
 
Note: it is considered best practice to avoid using the root user for daily tasks. Instead, create a new user with sudo privileges and use that account for your daily tasks.
 
For the most part, the user creation process in Webmin is similar to the useradd utility. However, one key difference between the two is that the Webmin’s approach allows you to associate an SSH key to a new user, allowing you to create secure accounts that do not rely on traditional password authentication.
 
Save your new user by clicking the “Create” button.
 
Lastly, restart your machine to fully apply your new configuration. Select the “Bootup and Shutdown” item in the left sidebar.
 
Scroll down to the bottom of the page and select “Reboot System.”
 
## Frequently Asked Questions
 
Image credit: Unsplash. All alterations and screenshots by Ramces Red.
 
### I am using an Nginx for my webserver. Can I use Webmin to manage it remotely?
 
Webmin only supports Apache 2, so you can’t use it to manage Nginx.
 
### I am getting an SSL error whenever I access the web interface. Is my installation broken?
 
This issue is mostly due to your browser not being able to recognize Webmin’s SSL certificate. A basic installation normally uses a self-signed certificate for its SSL. This allows it to establish a secure connection even in local networks.
 
For the most part, you can ignore this warning if you are only hosting Webmin in a closed local network. However, you need to create a proper SSL certificate if you intend on running it over the Internet. Generate a Let’s Encrypt certificate by going to “Webmin -> Webmin Configuration -> SSL Encryption.”
 
### Is it possible to access the system shell through Webmin?
 
To access the system shell, go to the “Tools” category. Click “Command Shell” or “SSH Login.” The former allows you to run single commands, while the latter gives you a full remote shell.
 
### How can I uninstall Webmin from my server?
 
Run the/etc/webmin/uninstall.shcommand to remove all traces of Webmin from your server.
 
Ramces is a technology writer that lived with computers all his life. A prolific reader and a student of Anthropology, he is an eccentric character that writes articles about Linux and anything *nix.
 
Our latest tutorials delivered straight to your inbox




