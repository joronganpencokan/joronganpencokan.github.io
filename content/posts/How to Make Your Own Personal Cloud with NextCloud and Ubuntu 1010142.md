---
title: "Unlock the Secret to Your Own Cloud Space: Learn How to Create a Personal Cloud with Nextcloud and Ubuntu!"
ShowToc: true 
date: "2022-11-13"
author: "Carol Jones"
---
*****
Title: Unlock the Secret to Your Own Cloud Space: Learn How to Create a Personal Cloud with Nextcloud and Ubuntu!

Introduction:

Do you want to have a personal cloud space where you can store your files, documents, photos, and videos securely? Do you want to access these files from anywhere in the world without any hassle? If yes, then you should consider creating your own personal cloud using Nextcloud and Ubuntu.

Nextcloud is a self-hosted file sync and sharing software that allows you to create your own cloud space. Ubuntu is one of the best open-source operating systems that can be used to host Nextcloud on your server. In this article, we will explain how to create a personal cloud using Nextcloud and Ubuntu.

Step-by-Step Guide:

1) Install Ubuntu Server

Firstly, download the Ubuntu ISO file from the official website and create a bootable USB drive. Boot your server from this USB drive and follow the installation process.

2) Update your server

Once you have installed Ubuntu, update your server using the command:

sudo apt-get update 

sudo apt-get upgrade 

3) Install Nextcloud Server

Next, you need to install Nextcloud server using the following command:

sudo snap install nextcloud 

4) Configure Nextcloud

After installing Nextcloud, you need to configure it according to your preferences. To do this, first create a folder where you want to store your Nextcloud files. Then, navigate to the Nextcloud configuration file using the following command:

sudo nano /var/snap/nextcloud/current/nextcloud/config/config.php 

Here, change the default data folder to the folder that you have created in the previous step using the following line of code:

' datadirectory' => '/media/nextcloud/nextcloud-data', 

5) Configure Firewall

Next, you need to configure the firewall to allow incoming connections to Nextcloud. Use the following command to open port 80 and 443:

sudo ufw allow 80/tcp 

sudo ufw allow 443/tcp 

6) Set up SSL

SSL is important as it provides secure communication over the internet. To set up SSL on your server, install the Let's Encrypt SSL certificate by running the following command:

sudo apt-get install certbot 

sudo certbot certonly --standalone 

7) Create SSL Certificate for Apache

Once you have obtained the SSL certificate, move the certificate files to the appropriate directory using the following commands:

sudo mkdir /etc/apache2/ssl 

sudo mv /etc/letsencrypt/live/example.com/{fullchain.pem,privkey.pem} /etc/apache2/ssl/ 

8) Set up Apache Web Server

Next, you need to set up the Apache web server to serve your Nextcloud instance using the following command:

sudo apt-get install apache2 

9) Configure Apache

After installing the web server, you need to configure it for your Nextcloud instance using the following command:

sudo nano /etc/apache2/sites-available/nextcloud.conf 

Here, enter the following lines of code:

Alias /nextcloud "/var/snap/nextcloud/current/" 

<Directory /var/snap/nextcloud/current/> 

Options +FollowSymlinks 

AllowOverride All 

<IfModule mod_dav.c> 

Dav off 

</IfModule> 

SetEnv HOME /var/snap/nextcloud 

SetEnv HTTP_HOME /var/snap/nextcloud 

</Directory> 

10) Enable the Nextcloud Site

Finally, enable the Nextcloud site using the following command:

sudo a2enmod ssl 

sudo a2ensite nextcloud.conf 

sudo a2enmod rewrite 

sudo systemctl restart apache2 

Conclusion:

In conclusion, creating your own personal cloud space using Nextcloud and Ubuntu is a great way to secure your files while maintaining full control of your data. By following this step-by-step guide, you can easily create your own personal cloud space.

With your very own personal cloud, you can access your files from anywhere in the world, and never have to worry about data loss or security breaches. All you need is a server, some technical know-how, and Nextcloud and Ubuntu, to unlock the secret to your own cloud space.

{{< youtube I4wEIws4t6Y >}} 



Have you ever wanted to have your own private Dropbox, something that lets you manage and distribute files online but with no company telling you about data limits, bandwidth restrictions or even disabling certain file-types? Great news! This dream can easily be made a reality with the help of software known as Nextcloud.
 
This software makes it so anyone with a server can host and distribute their own storage and effectively have their own cloud! In this guide we’ll go over everything you need to know to make your own personal cloud storage solution – from going over the hardware required, getting the operating system in order, and even setting up syncing clients. Let’s get started!
 
Note: Nextcloud is a fork of Owncloud which is another self-hosted Dropbox clone.
 
## Hardware and Software Requirements
 
Let’s discuss the types of servers that are best to set up a home cloud powered by the NextCloud storage software. To start, the server should be running the latest version of Ubuntu server (or at the very least be running a version that supports snaps). Why Ubuntu server and not something like Redhat or CentOS? Simple, the developers of NextCloud currently distribute a snap package with the latest NextCloud software, something that these other operating systems don’t offer.
 
Additionally, NextCloud, when installed in other ways, takes a long time to set up and is not very user-friendly. By installing the snap version, zero setup is required, and everything pretty much works.
 
The developers have said in the past that it is hard to update NextCloud when they are based on distributions or integrated repositories. Ubuntu’s snap technology allows them to get the latest security updates to you as soon as possible on their own terms.
 
Hardware devices that are perfect for making your own cloud solution:
 
- Any used or old DDR2-era (or better) 64bit PC/laptop that can stay on 24/7
 - Raspberry Pi 2 or 3 that can run Ubuntu Snappy Core
 - Any home or enterprise grade server

 
## Making Preparations
 

 
Users will need to make a USB image to install the latest version of Ubuntu server. Download the ISO disk image from this page.
 
### Raspberry Pi 2/3 users
 
The Pi doesn’t currently run a traditional version of the Ubuntu server. Instead, users must use Ubuntu Snappy Core. Download the image here. Extract the image in the terminal:
 
Follow the Ubuntu wiki to get started with Snappy Core’s first boot. You will need to sign up with Canonical, using an email address.
 
With the disk image downloaded, it’s time to make the USB (or SD) install medium. Download the USB/SD tool Etcher. Follow the instructions on the page to create your installation USB or SD if you are using a Raspberry Pi 2/3. It is an easy three-step process.
 
## Installing Ubuntu Server
 
Plug in your USB device and configure your machine to boot from it via the BIOS. For some, this key may be F2 or DEL. For others, it is Esc. It is best to research the manual to be sure.
 
With Ubuntu server loaded, select the correct language on the language screen, then press Enter on the option “Install Ubuntu Server.” This will take the user through a menu that asks what the keyboard layout and country is. Select the appropriate options and move on to the next page.
 
Users will then be asked to enter a hostname for Ubuntu server. Enter “ubuntu-server,” “ubuntu-nextcloud,” “Ubuntu” or something to that effect. Then, using the arrow keys, navigate to the “Continue” button, and press Enter to move to the next page.
 
On the next page the installation tool will ask the user to set up a username and a password that goes with this username. Enter a username, and a secure but memorable password, then select “Continue” to move to the next page.
 
Next in the installation process, the user must tell Ubuntu server how to install to the hard drive. Select “guided – use entire disk.” This lets the system automatically set up partitions. No tinkering or manual partitioning is necessary. With this option selected, the installation will begin.
 
Soon after the initial Ubuntu server data finishes copying to the system, users will have to tweak a setting. The security updates a feature, to be exact. This feature, when enabled, allows the system to automatically install security updates. Select “install automatically.”
 
Lastly, before the installation finishes, some packages are needed. Using the spacebar, find “LAMP server” and select it. Additionally, select “OpenSSH server” if you want remote shell access ready to go. When the packages are selected, press the Enter key to install them to the system.
 
## Installing NextCloud
 
Ubuntu Server is installed to the system. Now it is possible to get NextCloud working. Install the software on the system with this command:
 
With NextCloud installed, use the command ifconfig to find the internal IP address of the server. Using the web browser on a phone, tablet or computer, go to the internal IP address as if it were a website.
 
This will bring up the Nextcloud Setup Wizard. This wizard will prompt the user to set up an admin account with a password.
 
## Using NextCloud
 
After creating the Admin account in next Cloud, the webUI will load, and the user will then have complete administrative control. Access Nextcloud at any time by heading to (in the web browser) the internal IP address used earlier.
 
Files from the admin account can be uploaded directly from the web via the browser (just like Google Drive, Dropbox and One Drive). Don’t like the web? Download the official sync client for Linux, Mac or Windows. There’s also an Android and iOS app, too.
 
### Uploading files
 
Upload a file or directory to your Nextcloud by clicking the “+” icon, then clicking the upload button.
 
### Creating new users
 
Users cannot register on Nextcloud. Instead, the admin must make a new account. Go to the top-right corner of the web UI and click on “admin.” Find “Users” and select it. This will bring you to the user management area.
 
Using the UI, set the username and password for the new user. Additionally, add the user to a new group by clicking “+ Add group.”
 
To modify how much storage a particular user is allowed to use, go to “Quota” and either select a preset option or enter your own storage quota limit.
 
### Syncing
 
To sync, enter the local IP address into the Nextcloud sync client.
 
Next, enter your username and password.
 
With the information entered, the Nextcloud client will create a Nextcloud folder on your local machine. Place anything you wish to sync inside it. The sync tool will detect it and upload the files.
 
## Conclusion
 
Cloud storage is a fact of modern-day life. Everyone has a Dropbox, a Google Drive, or something to that effect. As a result, large technology companies have large servers which hold precious, private information. For some, the trade-off and privacy risk is alright. They feel that Dropbox, etc., are reliable and versatile, and they’re willing to take the risk.
 
Nextcloud isn’t for those types of people. This software is for those who see the benefits of cloud storage but want to totally control their data. It is my hope that with this guide more and more people will embrace Nextcloud and break free of proprietary cloud storage services.
 
Do you host your own cloud solution? Why or why not? Tell us below!
 
Image credit: Christine und Hagen Graf
 
Derrik Diener is a freelance technology blogger.
 
Our latest tutorials delivered straight to your inbox




