---
title: "Rev Up Your Website's Speed in Just 3 Easy Steps with Pagespeed Module for Apache on Ubuntu Server!"
ShowToc: true 
date: "2023-06-08"
author: "Sharan Parsons"
---
*****
# Rev Up Your Website's Speed in Just 3 Easy Steps with Pagespeed Module for Apache on Ubuntu Server!

As website owners, we understand the value of website speed. A website that loads quickly not only improves the user experience, but it also helps in search engine optimization. However, optimizing website speed can be a challenging task for website admins who don't have any prior experience in server administration. Fortunately, the Pagespeed module for Apache on Ubuntu Server can help.

In this article, we will guide you through three easy steps to install and configure the Pagespeed module for Apache on your Ubuntu Server.

## Prerequisites
Before we delve into the installation and configuration process, you will need the following:

1. A Linux Ubuntu server with Apache installed
2. Sudo or root access to the server
3. SSH client to connect to your server via the terminal

## Step 1: Install the Pagespeed Module
The first step is to install the Pagespeed module. Open the terminal window and log in to your server using an SSH client. Then, run the following command:

```sudo apt-get install -y libapache2-mod-pagespeed```

This command will install the Pagespeed module on your Apache server.

## Step 2: Enabling the Pagespeed Module
Now that we have installed the Pagespeed module, the next step is to enable it. Run the following command to enable the module:

```sudo a2enmod pagespeed```

This command will enable the Pagespeed module on your Apache server. After this, restart your Apache server to apply the changes by running the following command:

```sudo service apache2 restart```

## Step 3: Configuring the Pagespeed Module
The last step is to configure the Pagespeed module as per your website requirements. To access the Pagespeed module configuration file, run the following command:

```sudo nano /etc/apache2/mods-available/pagespeed.conf```

This command will open the Pagespeed module configuration file in the Nano editor. You can now modify the settings as per your website's requirements. Here are some critical settings that you may want to change:

- **ModPagespeedEnableFilters**: This directive allows you to enable or disable individual filters of the Pagespeed module. To enable a filter, remove the '#' before the filter name. To disable a filter, add the '#' before the filter name.

- **ModPagespeedFileCachePath**: This directive allows you to specify the location of the file cache.

- **ModPagespeedImageMaxRewritesAtOnce**: This directive allows you to control the number of images this module will optimize concurrently.

After making changes to the Pagespeed module configuration file, save the file by pressing 'Ctrl+X' and then pressing 'Y' to confirm the changes.

Finally, restart your Apache server to apply the configuration changes by running the following command:

```sudo service apache2 restart```

And that's it! You have successfully installed and configured the Pagespeed module for Apache on your Ubuntu server.

## In Conclusion
Optimizing website speed is a crucial factor in enhancing the user experience and improving website ranking. The Pagespeed module for Apache on Ubuntu server is an excellent tool that can help website admins without any prior server administration knowledge.

By following the three easy steps mentioned above, you can boost your website's speed without breaking a sweat.

{{< youtube 0ZjTC9wJ1RM >}} 



There are many factors that can affect the speed of a website, and one of them is the server performance – how fast the server can render the web page and serve it to the browser. While there are many ways to improve the speed of a WordPress site, there are also server tools that can optimize the performance of a server. PageSpeed Module for Apache is one of them.
 
The PageSpeed module is a module for the Apache web server to optimise web pages, improve performance and apply output filters.
 
## Features
 
Some of the main features of the PageSpeed module include decreasing load time, the amount of requests and payload size. You can use up to 44 filters to optimize your webpage. Here is what the PageSpeed Module can do:
 
- Combine Javascript and CSS. One of the main things that the PageSpeed Module does is combine the Javascript and CSS to fewer files, thus reducing resources requests made to the server.
 - Minify Javascript and CSS. The PageSpeed module removes line breaks, blank spaces and unnecessary comments from Javascript and CSS files.

 

 
The above is minified to make this:
 
The above two files both do the same job, but the second one is smaller in size, hence translates to a fast load time of the site.
 
- Javascript Deferred Loading. The loading of Javascript file will be delayed until the web page is loaded. This will make sure that your visitor will see the content first as soon as possible. Do take note that this feature might break your site, depending on the functionality of the Javascript code. When activating this feature, first test your website before making it live.
 - The Pagespeed module comes with a number of rules that it uses to compress and optimize images to reduce the website’s load time. The rules include responsive images, lazyload images and Inline preview which shows a low quality of images.

 
## Installation
 
The following commands install the PageSpeed module in Ubuntu. Do note that this is for Apache, which mean your server need to be running Apache. If you are using Nginx, you have to build from source.
 
If you are using a 32-bit OS, run this command:
 
Run this command for a 64-bit OS:
 
The above commands download the package. These commands unpack and install it.
 
Installing PageSpeed adds Google’s repository to the system, so it will auto-update itself on every system update. We can verify the installation by running the command below and you will get the output shown:
 
## Configuration
 
The configuration file is stored at the “/etc/apache2/mods-available/” directory. When installing PageSpeed, the module is automatically enabled as well as the “mod_deflate” which is a module for gzip compression.
 
To turn the PageSpeed module on and off, edit the configuration file using your favorite text editor.
 
Opening the file, you can see that “ModPagespeed” is set to “on” by default. Changing this to “off” will disable the Pagespeed module.
 
While PageSpeed is optimizing a website, it generates some resources that are stored in a directory called “pagespeed_static”. To change this directory, edit the configuration file and add this line:
 
## Usage
 
The PageSpeed module gives a browser interface to view the statistics of its output. To access the browser interface on a public IP, you will need to edit the following lines in the configuration file:
 
Below the Allow from 127.0.0.1 line, add a similar line with your public address in place of the localhost address, something like:
 
Replace “192.xx.xx.xx” with your public IP address.
 
You can now restart Apache and visit that address. You will see an output that looks similar to this;
 
## Conclusion
 
The PageSpeed Module provides a good way for a webmaster to optimize the server performance without having to do a lot of tweaking. It can be easily installed and work out of the box. A little note though, when enabling its filters, it is best to test it on a test server and see if it works first before making it live. 
 
I am an intelligent and presentable individual with a degree in Computer Science and over four years experience in Management, Software Development, Information Technology Support and Tech article/tutorial writing. I possess a fresh, modern approach to the industry, employing creative and enthusiastic methods to problem-solving and would like to realize my full potential through practice, effectiveness, and innovation.
 
Our latest tutorials delivered straight to your inbox




