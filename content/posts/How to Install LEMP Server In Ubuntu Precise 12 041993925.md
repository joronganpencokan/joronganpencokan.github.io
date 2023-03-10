---
title: "You Won't Believe How Easy it Is To Install Lemp Server on Ubuntu Precise 12.04 – Check Out These Foolproof Steps Now!"
ShowToc: true 
date: "2023-06-19"
author: "Kenneth Frances"
---
*****
How to Install Lemp Server on Ubuntu Precise 12.04 – Foolproof Steps!

Are you struggling with setting up a Linux, Nginx, MySQL, and PHP (LEMP) server on Ubuntu Precise 12.04? You're at the right place! In this article, we will give you a step-by-step guide to install LEMP server on Ubuntu Precise 12.04.

What is LEMP Server?

The LEMP stack is a popular web stack used in developing web applications. It consists of four essential components, namely; Linux (Ubuntu), Nginx (Web server), MySQL (Database Management System), and PHP (Server-side scripting language). The LEMP stack is incredibly fast and efficient compared to the traditional LAMP stack.

Why Use LEMP Server?

LEMP is a powerful tool that allows developers to create high-performance web-based applications. It's optimized for performance and security, making it one of the best stacks for web developers. Besides, it's much easier to configure as compared to the Apache-based LAMP stack.

Here are the steps to follow to install LEMP server on Ubuntu Precise 12.04

Step One: Update the System

It's always essential to update your system before installing any packages to ensure that the system has all the latest updates.

sudo apt-get update
sudo apt-get upgrade

Step Two: Install Nginx

Nginx is a high-performance web server that can handle a large number of concurrent connections. To install Nginx on Ubuntu Precise 12.04, run this command:

sudo apt-get install nginx

Step Three: Install MySQL

MySQL is a popular database system that stores data for web-based applications. To install MySQL on Ubuntu Precise 12.04, run this command:

sudo apt-get install mysql-server mysql-client

In the process, you may be prompted to set a root password for the database management system.

Step Four: Install PHP

Finally, we need to install PHP, a server-side scripting language that powers most modern web applications. To install PHP on Ubuntu Precise 12.04, run this command:

sudo apt-get install php5-fpm php5-mysql

Step Five: Configure Nginx

After installing Nginx, you need to configure it to work correctly with PHP. To do this, we will edit the default Nginx configuration file:

sudo nano /etc/nginx/sites-enabled/default

Inside the file, add the following code:

location ~ \.php$ {
        fastcgi_pass unix:/var/run/php5-fpm.sock;
        fastcgi_index index.php;
        fastcgi_param SCRIPT_FILENAME $document_root$fastcgi_script_name;
        include fastcgi_params;
}

Afterward, save and exit the configuration file.

Step Six: Restart Nginx and PHP5-FPM services

After saving the Nginx configuration file, we need to restart the Nginx service by running the following command:

sudo service nginx restart

We'll also restart the PHP5-FPM service by running this command:

sudo service php5-fpm restart

That's it! You have successfully installed LEMP server on Ubuntu Precise 12.04.

Conclusion

In conclusion, the LEMP stack is a powerful tool that can help developers create high-performance web-based applications. Installing the LEMP stack on Ubuntu Precise 12.04 is a straightforward process that anyone can follow. With the steps outlined in this article, you're now ready to build your web applications using LEMP.


A LEMP server refers to a server running Linux, Enginx (Nginx), MySql and PHP (or Perl/Python). It is similar to the popular LAMP server except that the underlying web server is managed by Nginx instead of Apache. In this tutorial, we will show you how to install LEMP server in Ubuntu 12.04.

 
## Nginx vs Apache
 
For those who are not aware, Nginx is an open-source web server that can run faster and use lesser system resources than Apache. Under light load, the differences between Apache and Nginx is negligible. However, on heavy load, Nginx can scale accordingly and run as fast without taking up tons of memory resource. Apache is a beast by itself and can easily take up to several hundreds of RAM for heavy loads. 
 
Note: This tutorial assumes that Ubuntu 12.04 is already installed in your system. Command lines will be used instead of graphical interface since most web server doesn’t come with a desktop manager.
 
## Installing Nginx
 
In the terminal, type the following:
 
This will add the Nginx PPA to your repository so you are always updated with the latest stable version. 
 
Just in case Apache is installed and running in the background, we need to stop it before Nginx can run.
 
Start Nginx.
 
If the above command doesn’t work, use this:
 
Open a browser and browse to “http://localhost“. For a remote web host, you should type in your IP address instead. You should see the following:
 

 
## Installing and Configuring PHP
 
Installing PHP is easy, but getting it to work with Nginx will require some configuration. 
 
To install PHP5 and other essential modules:
 
“php5-fpm” is the essential module for PHP to work in Nginx environment, so make sure it is installed.
 
### Configuring Nginx to work with PHP
 
Open the “default” file in the /etc/nginx/sites-available directory.
 
Scroll down the list till you see the line index index.html index.htm;. Add a index.php at the end of the line, just before the “;“. It should become like this:
 
Next, scroll down further until you see this block of code:
 
Remove the first “#” at the front of end line (except the line #  fastcgi_pass unix:/var/run/php5-fpm.sock;) and add an extra line try_files $uri =404; at line 2, so it becomes like this:
 
Save (press “Ctrl + o”) and exit (Ctrl + x) the config file.
 
Restart Nginx.
 
To test if php5 is working in Nginx, we are going to create a php file, place it in the Nginx folder and see if it shows up in the browser.
 
Add the following code to the blank file:
 
Save and exit the file.
 
Now, go to the browser and type “http://localhost/phpinfo.php” or “http://your-ip-address/phpinfo.php”. 
 
If the php info shows up on the browser, then php is working fine with Nginx.
 
## Installing MySql
 
During the installation, it will prompt you to create the root password.
 
Once installed, you are done with the LEMP server setup. 
 
## Optional Install: phpmyadmin
 
Phpmyadmin is not part of the LEMP server setup, but it is very helpful for managing database and is often included in many web server setup.
 
To install phpmyadmin, 
 
When prompted to select either “apache2” or “lighttpd”, select none and click OK.
 
When prompted whether to configure database with dbconfig-common, select No.
 
After the installation, open the Nginx’s “default” file:
 
Add the following code after the php block of code:
 
Save and exit the file. Restart Nginx.
 
You should be able to connect to phpmyadmin via the URL: “http://localhost/phpmyadmin” or “http://your-ip-address/phpmyadmin“
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




