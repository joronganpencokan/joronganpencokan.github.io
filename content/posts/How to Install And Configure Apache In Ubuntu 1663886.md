---
title: "Unlock the Secrets of Web Hosting: Learn How to Install and Configure Apache in Ubuntu Now!"
ShowToc: true 
date: "2023-05-09"
author: "Tracy Wickus"
---
*****
Title: Unlock the Secrets of Web Hosting: Learn How to Install and Configure Apache in Ubuntu Now!

Introduction:

In today's digital era, having a website has become a fundamental necessity for businesses and individuals alike. But, to make your website available to the world, you need a web hosting service that stores your site files on a server and makes it accessible through the internet.

The most commonly used web server software is Apache, which is open-source and free to use. Apache provides stable, reliable, and efficient processing of web requests and has excellent support for PHP, Perl, and other scripting languages.

In this article, we will guide you on how to install and configure Apache web server on Ubuntu, a popular Linux distro.

Body:

Step 1: Update Ubuntu
Before installing any software on Ubuntu, it's always best to update the packages to the latest versions. Open your terminal and type the following command:
sudo apt-get update

Step 2: Install Apache
After updating the packages, run the following command to install Apache2:
sudo apt-get install apache2

Step 3: Start the Apache Service
Once the installation completes, you can start the Apache service by running the following command:
sudo systemctl start apache2

Step 4: Check Apache Status
To check if Apache is running correctly, type the following command:
sudo systemctl status apache2

You should see a message stating that Apache is active and running.

Step 5: Configure Apache to Work with your Domain
Now that Apache is up and running, you need to configure it to work with your domain.

Locate the Apache configuration file by typing the following command:

sudo nano /etc/apache2/sites-available/yourdomain.com.conf
[Note: Replace yourdomain.com with your actual domain name]

Add the following code to the configuration file:

<VirtualHost *:80>
ServerAdmin webmaster@yourdomain.com
ServerName yourdomain.com
ServerAlias www.yourdomain.com
DocumentRoot /var/www/yourdomain.com/public_html
<Directory /var/www/yourdomain.com/public_html>
Options Indexes FollowSymLinks MultiViews
AllowOverride All
Require all granted
</Directory>
</VirtualHost>

Save the changes and exit the editor.

Step 6: Enable your Domain
Now that your domain configuration is in place, you need to enable it. Type the following command:

sudo a2ensite yourdomain.com.conf

Step 7: Restart Apache
To apply the changes, restart Apache by running the following command:

sudo systemctl restart apache2

Congratulations! You have successfully installed and configured Apache on Ubuntu and are now ready to host your website.

Conclusion:

In conclusion, Apache is a powerful web server that is easy to install and configure on Ubuntu. With its robust features and support for multiple scripting languages, it's an excellent choice for hosting websites of all sizes. By following the steps outlined in this article, you can quickly set up an Apache web server and get your website up and running in no time.

{{< youtube 1CDxpAzvLKY >}} 



If you intend to set up a web server (or streaming server) in your Ubuntu machine, apache is one important module that you must install. In this tutorial, we will show you how to install and configure apache for your Ubuntu. 
 
Note: If you just want to have a quick setup of LAMP server, follow the guide here.
 
## Installing Apache
 
Getting apache onto your Ubuntu machine is easy. Using either the Synaptic Package Manager, Ubuntu Software Center, search and install the “apache2” module. Alternatively, you can open a terminal and type the following command:
 
Once the installation finished, open a browser and go to the URL “http://localhost“. If you see the word “It Works!“, then your installation of apache is successful.
 

 
## Configuring Apache
 
Start, Stop and Restart Apache
 
After you have installed Apache, it will be added to the init.d list and will auto start whenever you boot up your computer. The following commands allow you to start, restart, stop Apache.
 
To prevent Apache from autostart when booting up:
 
To restore Apache back to the autostart list:
 
Note: the above commands will work in debian-based distro (including Ubuntu) only.
 
Changing the default localhost folder
 
By default, apache will operate on the “/var/www” folder. This means that whatever files you place in this /var/www folder will be visible from the URL http://localhost. In some instances, you may want the “localhost” to point to another folder instead, say /home/user/public_html. Here is how you do it:
 
First, make sure the /home/damien/public_html folder exists. Create a simple html file, name it index.html and place it in the public_html folder. 
 
Open a terminal and type:
 
Change DocumentRoot /var/www to DocumentRoot /home/user/public_html.
 
Change <Directory /var/www/> to <Directory /home/user/public_html/>.
 
Save and exit the file.
 
Restart the apache
 
Now, in your browser, reload the URL http://localhost. You should see the html file that you have placed in the public_html folder.
 
Configuring different sites
 
The above trick allows you to change the default operating folder of apache, however, some of you might not want to override the default settings. An alternative is to create multiple sites and point apache to the active site.
 
Create a new settings file for your new site.
 
Next, edit this settings file.
 
Disable the default setting and make active the site1 settings
 
Lastly, restart the apache.
 
With this trick, you can create multiple site configuration file, each pointing to a different folder. You can then easily switch between the sites with the a2dissite and a2ensite command
 
Enabling .htaccess file
 
.htaccess file is a powerful file that can be used to control and customize a site server behavior without editing the core Apache module. By default, the .htaccess functionality is turned off and all instances of .htaccess files are completely ignored. The server will not even attempt to read .htaccess files in the filesystem.
 
To enable .htaccess file, open up the settings file that you have created earlier:
 
Scroll down the file until you see the part “<Directory /home/user/public_html/>“. Underneath that line of code, change AllowOverride None to AllowOverride All.
 
Recommended read:
1. Install LAMP server in Ubuntu 
 
2. How to install VLC-Shares in Ubuntu and stream audio/video to Android
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




