---
title: "Discover the Secret to Install OpenOffice Org 3.2 in Ubuntu 9.10 Like a Pro!"
ShowToc: true 
date: "2023-03-02"
author: "Timothy Pearce"
---
*****
Introduction

OpenOffice Org 3.2 is a free, open-source office productivity suite that has garnered a loyal following over the years. It is an excellent alternative to Microsoft Office, providing users with all the standard features and services one would expect from a top-notch productivity suite. One of the best things about OpenOffice Org 3.2 is that you can easily install it on Ubuntu 9.10, a popular Linux distribution. In this article, we'll show you how to install OpenOffice Org 3.2 on Ubuntu 9.10 like a pro.

Step-by-Step Guide to Install OpenOffice Org 3.2

Step 1: Prepare your system for installation

Before you install OpenOffice Org 3.2, you need to ensure your system is up-to-date. To achieve this, run the following command in the terminal:

sudo apt-get update && sudo apt-get upgrade

It is important to mention that if you have an older version of OpenOffice Org installed on your system, you need to uninstall it before proceeding with the installation of OpenOffice Org 3.2. This can be achieved by running the following command:

sudo apt-get --purge remove openoffice*.*

Once you have completed the above steps, you are now ready to proceed with the installation of OpenOffice Org 3.2.

Step 2: Download OpenOffice Org 3.2

The next step is to download OpenOffice Org 3.2. You can do this by visiting the official website and choosing the appropriate version for Linux. Alternatively, you can execute the following command in the terminal:

wget https://sourceforge.net/projects/openofficeorg.mirror/files/3.2.1/oo_3.2.1_linux_x86_install-deb_en-US.tar.gz/download -O oo_3.2.1_linux_x86_install-deb_en-US.tar.gz

This will download the file to your system.

Step 3: Extract and Install OpenOffice Org 3.2

Once you have downloaded the file, the next step is to extract and install OpenOffice Org 3.2. You can achieve this by executing the following commands in the terminal:

tar -xzvf oo_3.2.1_linux_x86_install-deb_en-US.tar.gz

cd OOO320_m18_native_packed-1_en-US.9502

sudo dpkg -i *.deb

This will extract the files and launch the OpenOffice Org 3.2 installer. Follow the on-screen instructions to complete the installation process.

Step 4: Launch OpenOffice Org 3.2

Once you have completed the installation, you can launch OpenOffice Org 3.2 by going to the Applications menu and selecting Office. You should see OpenOffice Org listed as an option. Click on it to launch the application.

Conclusion

Installing OpenOffice Org 3.2 in Ubuntu 9.10 is a relatively simple process that you can easily accomplish by following the steps outlined in this article. With OpenOffice Org 3.2, you can enjoy all the productivity features you need without the need for expensive proprietary software. Start using OpenOffice Org 3.2 today and discover the benefits of an open-source, community-based approach to productivity.

{{< youtube nJS_F0FlDIM >}} 



Few free software projects have had as large of an impact as OpenOffice.org.  It is used by millions of users all over the world and is the primary competition to Microsoft Office in the desktop market.  The latest version of OpenOffice.org (3.2) adds a number of notable features worth trying.  Among them are:
 
- Faster startup times (a 46% increase)
 - Better open and proprietary file format support
 - Better Asian language support
 - Numerous Calc (spreadsheet) improvements
 - and many others.

 
The upcoming release of Ubuntu (10.04 “Lucid Lynx”) will include OpenOffice.org 3.2 by default, and the release is on April 29 — just around the corner.  But if you happen to be a little impatient or just want to give it a try, there are packages available directly from the OpenOffice.org website that work well with Ubuntu 9.10.
 
To install, just follow these steps:

1. Point your web browser to the OpenOffice.org download page
 
2. Scroll down to the table of release packages.
 
3. In the left column, select your language.
 
4. Run your mouse pointer across the page to the Linux 32-bit DEB or Linux 64-bit DEB, depending on the distribution you are running.
 
Note: If you are not sure, run “uname -a” from a terminal. If you are using 64-bit, it will say x86_64 at the end of the string before GNU/Linux.
 
5. Click “Download” and save the compressed file to a new folder (You can call it openoffice if you like).
 
6. Open a terminal window (such as gnome-terminal or konsole).
 
Note: At this point, it is a good idea to remove the existing OpenOffice installation with the following command:
 
7. Change to the directory you just created:
 
8.  Unpack the archive with the following command:
 
9. Change to the newly created directly:
 
10. Install all of the open office deb files:
 
11. Now add the desktop integration package:
 
Once you have OpenOffice.org installed, you should test it to make sure it works properly. It should have installed the necessary menu icons in the appropriate location, regardless of whether you use Gnome, KDE, or any other desktop. If you had your own shortcuts anywhere else, however, you may need to update them to reflect the installation location, which is: /opt/openoffice.org3.
 

 
There were a couple of features I was not able to get working, mainly KDE 4 integration (file picker and theme). The packages were designed to integrate with KDE 3. If that is a show-stopper for you, then it is best to wait for the official Ubuntu release.
 
When I first started it, I immediately noticed the speed boost and some of the most noticeable “Writer” features. Try creating various documents, saving, closing, and reopening to make sure it all works before you start creating critical documents. If it all checks out fine, you will have successfully installed OpenOffice.org 3.2 on Ubuntu 9.10.
 
Tavis J. Hampton is a  freelance writer from Indianapolis.  He is an avid user of free and open source software and strongly believes that software and knowledge should be free and accessible to all people. He enjoys reading, writing, teaching, spending time with his family, and playing with gadgets.
 
Our latest tutorials delivered straight to your inbox




