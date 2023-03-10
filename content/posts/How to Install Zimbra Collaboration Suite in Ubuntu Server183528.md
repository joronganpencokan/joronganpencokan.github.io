---
title: "Revolutionize Your Email Game: Learn How To Install Zimbra Collaboration Suite On Your Ubuntu Server Today!"
ShowToc: true 
date: "2022-12-20"
author: "Julia Allmon"
---
*****
Revolutionize Your Email Game: Learn How To Install Zimbra Collaboration Suite On Your Ubuntu Server Today!

Email communication is one of the fundamental aspects of modern-day business transactions. And with the increase in remote working due to the recent pandemic, businesses worldwide are shifting to cloud-based email clients for secure communication.

Zimbra Collaboration Suite is a renowned email collaboration platform that offers seamless email services designed for small, medium, and large organizations. With its advanced features, Zimbra has become the preferred choice of businesses worldwide.

In this article, we will introduce you to the step-by-step guide on how to install Zimbra Collaboration Suite on your Ubuntu server.

Step 1: Pre-Installation

Before installing Zimbra Collaboration Suite, you need to ensure that your Ubuntu server has a Stable FQDN (Fully Qualified Domain Name).

First, check your hostname using the following command:
$ hostname

Next, check your domain name using the following command:
$ domainname

If you don't have an FQDN, you need to set up one. You can do so by following the instructions provided here: https://www.linuxtechi.com/set-hostname-domainname-linux-systems/

Step 2: Download & Install Zimbra Collaboration Suite

First, create a folder to download Zimbra Collaboration Suite using the following command:
$ mkdir ~/Downloads && cd ~/Downloads

Next, download Zimbra Collaboration Suite from their official website using the following command:
$ wget https://files.zimbra.com/downloads/8.8.15_GA/zcs-8.8.15_GA_3869.UBUNTU18_64.20190918004220.tgz

The above command will download the Zimbra Collaboration Suite package into your ~/Downloads folder.

Once downloaded, extract the Zimbra Collaboration Suite package using the following command:
$ tar -xzvf zcs-8.8.15_GA_3869.UBUNTU18_64.20190918004220.tgz

Navigate to the extracted Zimbra Collaboration Suite directory using the following command:
$ cd zcs-8.8.15_GA_3869.UBUNTU18_64.20190918004220

Run the installation script using the following command:
$ sudo ./install.sh

The installation script will ask you to accept the Zimbra Collaboration Suite license agreement. Once accepted, it will start the installation process. The entire process may take up to 30 minutes, depending on your server configuration.

Step 3: Post-Installation Configuration

Once the installation process is complete, you need to configure the Zimbra Collaboration Suite server to suit your needs.

To configure the Zimbra Collaboration Suite server, you need to log in to the Zimbra Admin Console. You can access the Admin Console by navigating to the following URL in your web browser:
https://<your-server-FQDN>:7071

Log in to the Admin Console using the credentials configured during the installation process.

Once logged in, you can configure Zimbra Collaboration Suite to suit your needs. You may want to configure things like email policies, spam filters, mailbox quotas, and more.

Conclusion

In conclusion, Zimbra Collaboration Suite is an excellent email collaboration platform that offers advanced features designed for modern-day business communication. By following the step-by-step guide above, you can install and configure Zimbra Collaboration Suite effortlessly on your Ubuntu server.

With Zimbra Collaboration Suite, you can take your email game to the next level, boost productivity, and facilitate seamless communication within your organization. So, why wait? Install Zimbra Collaboration Suite today and revolutionize your email game!

{{< youtube 9ZGuipObYFg >}} 



Zimbra Collaboration Suite (ZCS) is a next generation collaboration and communication platform, with a mission to answer the challenges posed on large organisations by legacy mailing systems. While Zimbra also offers hosted solutions, the Open Source edition is a self hosted mailing platform, retaining most of the functionality of the paid version.
 
## Zimbra is…
 
- Cross platform: (Linux, Mac, Windows). Running from a server, it can be accessed as an AJAX web application from most major browsers
 - Innovative: The interface features functionality usually found in desktop applications such as drag and drop or advanced search functionality
 - Secure: You get full control over your accounts and data
 - Easy to maintain: You get full CLI or web-based control over your installation
 - Compatible: Besides the web-client, you can access our Zimbra messages from Outlook and other desktop mail clients as well.

 
Installing Zimbra is surprisingly straight forward and could be completed under 10 minutes. Zimbra recommends that you disable SELinux and any firewall running, before installation. The OpenSouce Edition was installed on a fresh, full-stack Ubuntu 14.04.2 LTS Server; the instance for this was for tutorial’s sake, with all standard components left intact.
 
## Preparing your system
 
After logging or sshing in to your Ubuntu 14.04 Server installation, you need to become root. Instead of using su, it is a good idea to proceed with
 
Besides the advantages of sudo over su, sudo -s will not change your $HOME variable, thus you will keep working in your user’s home directory.
 
Zimbra will conflict with postfix. You could just disable it, but it is probably best to uninstall it entirely if you plan to use Zimbra for messaging anyway.
 
Ubuntu links sh to dash, but the Zimbra installer will complain if it does not find bash where it expects it. To fix this, you should point sh to bash:
 
## Configuring the network
 
You will need a static IP address, if you do not already have one. Editing the /etc/network/interfaces file would be the easiest option.
 
Change the file to include the following lines. Of course, the addresses should be replaced according to your own network configuration.
 

 
On the test installation, the hostname used was “ubuntu-test.com”, which is not a registered domain name. Yours should be a real one, if you plan to use Zimbra.
 
After running
 
and specifying your own domain, edit the file /etc/hosts
 
And change it to include the following (using your own IP and domain name, of course):
 
Save it and restart the network services, to make sure all the changes take effect.
 
Now your server is almost prepared. To install prerequisite packages, it is best to let the Zimbra installer script check what’s missing.
 
## Obtaining Zimbra
 
You can get the installation files in any way you like from the Zimbra download page. At the time of writing, the freshest available OpenSource version was 8.6.0 GA. To get it from the terminal, just copy and paste
 
and wait for the download to finish. Once it is downloaded, you’ll need to unpack the file. Using the asterik (*) wildcard below will unpack whatever version of Zimbra you have just downloaded, (if it is the only such downloaded file in your current directory), so you are safe to copy and paste the below command:
 
## Installing missing dependencies
 
The Zimbra install script has automatic dependency checking. You can run it just to see what you might be missing. Enter the unpacked directory, and run the installer:
 
It will ask you to accept the License Agreement
 
You will then have to select all the packages, like you were to install them, and the installer will tell you what is missing:
 
Quit the installer and install all the missing packages
 
## Installing Zimbra OS Edition
 
You should run the installer again:
 
After having you accept the license once again, it will not complain now, but start building Zimbra.
 
You will still have a few questions to answer. First you will need to select (again) the components you want to install. The default answer is “yes;” pressing Enter will accept the component. To skip any of the components, press “n.”
 
After accepting the “System will be modified” dialogue, the installation continues, up to the point of the DNS check. At this point it might complain about MX (mail exchange) record. It is best to set up an MX domain here. Fortunately the installer has the option to do this in-line:
 
The installer should soon take you to main the configuration menu:
 
An obvious next step is to set up the missing admin password. Pressing “7” will take you to the zimbra-store sub-menu:
 
If you press “4”, you will find it has generated a random password for you. Press Enter to accept it (and don’t forget to make a note of it), or type your own here.
 
Note: This is a weak point of the otherwise solid installer script. The password will be written plain on the screen and there is no confirmation dialogue either. Be careful, you only have one shot. It is best to double-check your password before pressing Enter.
 
Press “r” to return to the main menu
 
You can choose which components should be enabled or disabled and set them up one by one, entering their number. Once ready, press “a” to finish up the installation.
 
Congratulations, if you’ve managed to get this far, you have just installed Zimbra OS edition on your server.
 
## Checking if everything works
 
To make sure everything is up and running, check the status of each component with the zimbracontrol command. Zimbra has created a new user called “zimbra”, to which you should switch next, using su
 
Then start the status monitor:
 
You should have a similar result:
 
To access your web admin interface and configure your installation, go to
 
(using the IP you have specified of course), and enter your credentials.
 
## Conclusion
 
Zimbra is an excellent collaboration and communication tool that is surprisingly easy to install on Ubuntu Server. You can have Zimbra up and running in under ten minutes. For further information on how to set up and use your new installation, you can find detailed documentation in PDF format in your downloaded Zimbra package or by visiting the Zimbra support website.
 
Attila is a writer, blogger and author with a background in IT management. Using GNU/Linux systems both personally and professionally, his advice stems from 10+ years of hands on experience. In his free time he also runs the popular Meditation for Beginners blog.
 
Our latest tutorials delivered straight to your inbox




