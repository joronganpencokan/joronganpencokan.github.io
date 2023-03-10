---
title: "Discover The Ultimate Guide To Install Wordpress On Your Computer Or Server And Revolutionize Your Website Building!"
ShowToc: true 
date: "2023-05-30"
author: "Jenny Myers"
---
*****
# Discover The Ultimate Guide To Install Wordpress On Your Computer Or Server And Revolutionize Your Website Building!

WordPress is a powerful Content Management System (CMS) used by millions of people all over the world. WordPress allows anyone to build a website, regardless of their technical skills. However, before you build your first WordPress website, you need to install it on your computer or server. In this article, we’ll show you how to install WordPress and revolutionize your website building.

## Why Install WordPress Locally?

Installing WordPress locally means that you install it on your computer’s hard drive rather than on the webserver of your hosting provider. There are several advantages to installing WordPress locally first, such as:

- Speed: Your local computer is much faster than any webserver. So, your site will run faster, and you’ll be able to test your site’s plugins, themes, and other features without waiting for them to load.
- Security: Your local computer is much safer than any webserver. If your website gets hacked on your local machine, it won’t affect your real website hosted online. Also, nobody else can access your website while it’s on your local computer.
- Flexibility: Installing WordPress locally gives you more control over your website’s settings and configurations.

## Installing WordPress On Your Computer

Now that you’re aware of the benefits of installing WordPress locally, let’s get started with the installation process. Here are the steps involved in installing WordPress on your computer:

### Step 1: Download and Install XAMPP

To install WordPress on your computer, you need to create a local server environment. The first thing you need to do is download and install XAMPP from https://www.apachefriends.org/index.html. XAMPP is a free development stack that allows you to run PHP and MySQL on your computer.

### Step 2: Start XAMPP

Once you’ve installed XAMPP, you need to start it. After starting XAMPP, you’ll see several modules that run on your local server environment, such as Apache and MySQL.

### Step 3: Create a Database

The next step is to create a database for your WordPress installation. To do this, open your web browser and type in http://localhost/phpmyadmin/. This will take you to the phpMyAdmin interface, where you can create a database.

### Step 4: Download WordPress

Now that you’ve created a database, it’s time to download WordPress. Go to https://wordpress.org/download/, and download the latest version of WordPress. After downloading, extract the WordPress files to C:\xampp\htdocs\wordpress, or any other location of your choice.

### Step 5: Install WordPress

To install WordPress, open your web browser and type in http://localhost/wordpress/. This will bring up the WordPress installation screen. Follow the on-screen instructions to complete the installation process. Make sure to enter the database details you created in Step 3.

### Step 6: Start Building Your Website

Once you’ve installed WordPress successfully, you’re ready to start building your website. Install themes and plugins to customize your website, and start creating content.

## Installing WordPress On Your Server

If you’re ready to take your website live, you should install WordPress on your webserver. Here are the steps involved in installing WordPress on your server:

### Step 1: Choose a Hosting Provider

The first step is to choose a hosting provider. A hosting provider is a company that provides you with web hosting services to store your website files online. There are many hosting providers available, such as Bluehost, SiteGround, and HostGator.

### Step 2: Choose a Domain Name

After choosing a hosting provider, you need to choose a domain name for your website. Your domain name is your website’s address, and it’s what people will type in to access your site. Choose a domain name that’s catchy, easy to remember, and relevant to your business.

### Step 3: Install WordPress

Most hosting providers offer a one-click installation process for WordPress. To install WordPress, log in to your hosting provider’s control panel, and look for the WordPress installer. Click on it, and follow the on-screen instructions to complete the installation process.

### Step 4: Start Building Your Website

Once you’ve installed WordPress on your server, you’re ready to start building your website. Install themes and plugins to customize your website, and start creating content.

## Conclusion

Installing WordPress on your computer or server is easier than it sounds. With the steps outlined above, you can install WordPress in no time and start building your website. Whether you’re a blogger, business owner, or developer, WordPress is a powerful tool that can help you create stunning websites in no time. So, what are you waiting for? Install WordPress today, and revolutionize your website building!

{{< youtube pf8wji-tjPw >}} 



Part 1: How to install and configure XAMPP in Windows
 
There are various components that we need to find, install and configure before installing WordPress in our machine or server. Instead of hunting down all the components, we are going to use XAMPP that is an easy to install Apache distribution containing MySQL, PHP and Perl.
 
 Go to apachefriends website, Click “EXE” and download XAMPP for Windows.
 

 
Image 1.
 
 
 
Next Double Click the downloaded file “xampp-win32-1.7.3.exe”, XAMPP installation will launch Click “Browse” and choose an installation destination folder, example “C:\Install” and Click “Install”.
 
Image 2.
 
After the installation is completed, a command prompt window will open and answer the following questions.
 
Images 3-8.
 
Double Click the desktop shortcut named “XAMPP Control Panel” to launch “XAMPP Control Panel Application”, Click on Apache “Start”button and MySQL “Start”button and wait until their status change to ”Running”.
 
Image 9.
 
To access and configure your newly installed Apache server Click the “Admin” button (See image 9) your favorite web browser will launch to http://localhost/xampp/splash.php and after selecting your language to start (See image 10) you will be redirected to the main XAMPP page http://localhost/xampp (See image 11)
 
Image 10.
 
Image 11.
 
Click on “Status” to check that everything is working fine.
 
Image 12.
 
When you install XAMPP in your computer, the “root” user password for the MySQL is empty, this is not recommended, and without a password the database is accessible by anyone. To avoid this, we should set a password to the user “root”. See image 13.
 
Image 13.
 
To change the password Click MySQL “Admin” button in the “XAMPP Control Panel Application” panel and in your web browser select the SQLtab and type the following:
 
UPDATE mysql.user SET Password=PASSWORD('MyNewPass') WHERE User='root';

FLUSH PRIVILEGES;
 
Click “GO” to submit. See image 14.
 
Image 14.
 
Now, if you try to reload MySQL page, you will receive an error. This is because phpMyAdmin does not know about the new ‘root’ password. To fix it, browse to the {XAMPP installation folder} /phpMyAdmin/and open the file config.inc.php with a text editor, find the section /* Authentication type and info */ and look for the line:
 
$cfg[‘Servers’][$i][‘password’]             = ‘ ‘; 
 
Type the password of root user between the [ ‘ ‘] and save the file. See image 15.
 
Image 15.
 
Restart Apache and MySQL server, then you will be able to access MySQL server without problems.
 
You are now done setting up XAMPP; in the next part we will install WordPress.
 
Pureinfotech Video Tutorials
 
 
 
Continue to Part 2 




