---
title: "You won't believe how easy it is to host a website on Ubuntu using Tor - learn how now!"
ShowToc: true 
date: "2023-04-21"
author: "Alice Girard"
---
*****
# You won't believe how easy it is to host a website on Ubuntu using Tor - learn how now!

Have you ever wanted to host a website but were hesitant due to security concerns? Look no further than Ubuntu and Tor! 

In this article, we'll guide you through the simple steps to host a website on Ubuntu using Tor. 

## What is Ubuntu and Tor?

Ubuntu is a popular Linux distribution known for its user-friendly interface and reliability. It's a great choice for hosting websites as it's secure and easily customizable.

Tor, on the other hand, is a free and open-source software that allows users to browse the web anonymously. It's often used by users who wish to protect their online privacy or access content that may be restricted in their country.

## Installing Ubuntu and Tor

First, you'll need to install Ubuntu on your server. You can do this by downloading the Ubuntu Server ISO from the official website and following the installation instructions.

Once Ubuntu is installed, you'll need to install Tor. Open a terminal and type the following command:

```
sudo apt-get install tor
```

This will install Tor on your Ubuntu server. 

## Configuring Tor

Next, you'll need to configure Tor to act as a web server. Open the Tor configuration file by typing the following command:

```
sudo nano /etc/tor/torrc
```

Add the following lines at the end of the file:

```
HiddenServiceDir /var/lib/tor/hidden_service/
HiddenServicePort 80 127.0.0.1:80
```

Save and close the file. 

## Hosting your website

Now that Tor is configured, you can start hosting your website. Create a new directory for your website by typing the following command:

```
sudo mkdir /var/www/mywebsite
```

Create an index.html file by typing the following command:

```
sudo nano /var/www/mywebsite/index.html
```

Add the following HTML code:

```html
<!DOCTYPE html>
<html>
<head>
	<title>Welcome to my website</title>
</head>
<body>
	<h1>Hello, world!</h1>
</body>
</html>
```

Save and close the file. 

## Accessing your website

To access your website, you'll need to find the .onion URL that Tor generated. Type the following command:

```
sudo cat /var/lib/tor/hidden_service/hostname
```

This will display your website's .onion URL. 

Copy and paste the .onion URL into the Tor browser, and voila! You've successfully hosted a website on Ubuntu using Tor. 

## Conclusion

In conclusion, hosting a website on Ubuntu using Tor is incredibly easy and secure. With just a few simple steps, you can ensure the privacy and security of your website and its visitors. So why wait? Try it out for yourself today!

{{< youtube 5IHaokn-59w >}} 



The Tor network is a revolutionary piece of software. With a single program, it is now possible to browse and view the Web anonymously. This makes Tor an essential tool for users who want to preserve their privacy when browsing a website. It is also possible to use Tor for hosting a local web server online to make it incredibly helpful for privacy-conscious users who want to share information publicly without revealing themselves.
 
Note: find out what Tor and onion routing are first before you proceed.
 
## Why Host Your Website Over Tor?
 
One of the biggest advantages of hosting over Tor is that its connection also goes through intermediary nodes similar to the Tor Browser. A visitor checking out your website will not be able to know where you are hosting it from.
 
Aside from that, you also do not need to forward any ports to make your Tor-only website work. This makes hosting simple and accessible even in highly restricted networks. For example, a machine under a Carrier-Grade NAT network can still publish a website directly through Tor.
 
## Requirements
 
Before you can install both Nginx and Tor, you need to first make sure that you have the following resources ready:
 
- An Internet connection that does not restrict Tor for both incoming and outgoing requests. This allows you to broadcast your website through the Tor network.
 - A machine that can handle the website you are hosting. In most cases, a dual core desktop with 4GB of RAM should be enough for a basic website.
 - Root access to your hosting machine, as configuring Tor requires you to access system files.

 
The below image shows how to host an Nginx Tor-only website on an Ubuntu 22.04 LTS machine.
 
## Installing Nginx and Tor
 
Open a terminal. Type the following command to install Nginx and Tor:
 
## Configuring Firewall
 
Once you have installed both packages in your system, you can secure your server by configuring your firewall to only accept incoming connections from the Tor network by typing the following commands in the terminal:
 
The first two commands open both the HTTP and HTTPS ports in your system, while the last command explicitly opens the SOCKS port for the Tor network. This approach ensures that Tor will be able to properly redirect any traffic that is going to your machine.
 
## Creating a Tor Service for Your Website
 
Next, you need to create a hidden service entry for your web server. This is a service-specific configuration that will allow you to broadcast in the Tor network.
 
First, switch to your root account. You can do that by running the following command:
 
Once you are inside root, create your hidden service by editing the “/etc/tor/torrc” file. In my case, I am opening this file through GNU Nano.
 
Find the “location-hidden services” section by pressing Ctrl + W, then typing “location-hidden.”
 
You will see a couple of examples that demonstrate how to create your own Tor hidden service. For the most part, however, you only need to set two options: HiddenServiceDir and HiddenServicePort.
 
The HiddenServiceDir option tells Tor where it should save the configuration files for your hidden service. The HiddenServicePort option tells Tor how it should redirect any requests to your hidden service.
 
The following lines of code will create a new hidden service for your webserver:
 
Reload the Tor daemon to apply your new settings by running the following commands:
 
Tip: learn how to use Tor with your VPN connection.
 
## Creating a Simple Website Using Nginx
 
Once a Tor hidden service is up and running, start setting up your webserver. Create a new configuration file through the touch command:
 
Edit your new Nginx configuration file as a basic web server. For example, the following block of code will deploy a simple web server at port 80:
 
- The two listen variables set both the ports and host that this server configuration should listen to. In this case, Nginx listens at port 80 on both IPv4 and IPv6.
 - The root variable sets the location where Nginx will look for the files on your webserver.
 - The server_name variable contains the domain name of your server. Find it by running sudo less /var/lib/tor/nginx-tor-service/hostname.
 - The location variable contains functions on how Nginx deals with the files in your website’s root. In this example, it only sets the 404 error for any missing files.

 
Create a symbolic link for your new configuration file to “/etc/nginx/sites-enabled.”
 
Lastly, enable your new website by restarting Nginx:
 
## Accessing Your Website Over Tor
 
With both Tor and Nginx up and running, check whether your website is accessible from the Tor network. (Need to find more websites in the dark web? Check out these search engines.) First, download the latest Tor browser binary:
 
Extract the browser’s files in the current directory by running the following command:
 
Also, make sure that the Tor browser binary has the right execution bits:
 
Run and install Tor Browser on your machine by running the following command:
 
Lastly, browse to your new Tor website by typing its domain name in the address bar.
 
## Frequently Asked Questions
 
Image credit: Unsplash. All alterations and screenshots by Ramces Red.
 
### Is it possible to host a game server using Tor?
 
Yes, but running a Tor game server will result in a very poor gaming experience. For example, running a Minetest server over Tor will have a latency between 1000 and 5000 milliseconds.
 
While there are ways to speed up your Tor connections, the developers of Tor did not design the network to work in low-latency applications. Because of that, Tor is mostly helpful in publishing webpages and applications that do not depend on low latency.
 
### I am trying to host an FTP website but can't access it through Tor.
 
This issue is most likely due to a missing configuration in the “/etc/tor/torrc” file. To properly host a new service over Tor, make sure that the proper ports are open both in your firewall and torrc.
 
For example, add HiddenServicePort 21 127.0.0.1:21 and HiddenServicePort 22 127.0.0.1:22 to create an open FTP and SFTP port in your machine.
 
### Is it possible to host my website over SSL in Tor?
 
It is important to note that SSL is not a hard requirement when securing your Tor website. By default, Tor already encrypts your connections as soon as you load the Tor browser, so any website you visit on Tor is end-to-end encrypted.
 
If you want, obtain an SSL certificate for your Tor website, though the process can be tricky, as there are only a handful of certificate authorities that actively issue TLS for .onion domains.
 
Ramces is a technology writer that lived with computers all his life. A prolific reader and a student of Anthropology, he is an eccentric character that writes articles about Linux and anything *nix.
 
Our latest tutorials delivered straight to your inbox




