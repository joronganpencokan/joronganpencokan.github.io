---
title: "Revolutionary Hack: Photoshop Cs5 now available on Ubuntu Maverick 10.10 - Discover the Step-By-Step Installation Guide!"
ShowToc: true 
date: "2022-11-11"
author: "Carolyn Goldstein"
---
*****
Revolutionary Hack: Photoshop Cs5 now available on Ubuntu Maverick 10.10 - Discover the Step-By-Step Installation Guide!

For many years, Linux users have struggled to access Adobe Photoshop, considered by many as the definitive tool for professional digital image manipulation. In the past, avid Linux users have been forced to utilize alternative image editing software or to run Photoshop through virtual machines or Wine emulation software, often at significant cost in terms of speed and efficiency.

However, times are changing, and it seems that the Linux community has finally come up with a revolutionary hack that will enable Photoshop CS5 to run on Ubuntu Maverick 10.10 with minimal hassle. The possibilities that this opens up are exciting and significant for Linux users, many of whom have a great interest in photography, graphic design, web design or any other field that requires image manipulation tools.

In the following paragraphs, we will take you through the step-by-step installation guide for setting up Photoshop CS5 on your Ubuntu Maverick 10.10 machine.

Step One: Install Wine

Wine is software that enables Windows applications to be installed and run on Linux operating systems. It is required to run Photoshop CS5 on Ubuntu Maverick 10.10 effectively. To install Wine:

1. Open the Ubuntu Software Center
2. Search for "Wine"
3. Select "Wine Windows Program Loader" and click "Install"

Step Two: Download Photoshop CS5

Before downloading Photoshop CS5, it is advisable to check the compatibility of your machine using Wine's AppDB. This step is important to avoid some common errors that may occur during installation.
 
Once you are sure that your machine is compatible, you can download the software from Adobe's website. You will need to provide your Adobe credentials and then select the version of Photoshop CS5 that you wish to download.

Step Three: Begin Installation

1. Open the Terminal
2. Enter "cd Downloads" to navigate to the download folder
3. Type "wine setup.exe" and press Enter
4. The installation wizard should launch.
5. Follow the prompts and choose your installation settings.
 
Step Four: Run Photoshop CS5

After the installation process is complete, you can launch Photoshop CS5 by:

1. Opening the Terminal
2. Navigating to the installation directory using the "cd" command. For example, if you installed Photoshop CS5 to the default directory, use the following command: "cd ~/.wine/drive_c/Program Files (x86)/Adobe/Adobe Photoshop CS5"
3. Typing "wine Photoshop.exe" and pressing Enter
 
With these simple steps, you can now take advantage of Photoshop CS5 on your Ubuntu Maverick 10.10 operating system.

Conclusion

With the availability of Photoshop CS5 on Ubuntu Maverick 10.10, Linux users can now enjoy the full capabilities of this powerful software without having to resort to virtual machines or emulators. The revolutionary hack detailed above is a significant breakthrough for the Linux community, and it is hoped that it will pave the way for further developments in the field of digital imaging on Linux.


If you are running Ubuntu 10.10 Maverick and own a copy of the Photoshop CS 5 installer, you will find that you won’t be able to install it under wine. Photoshop CS5 on Ubuntu 10.4 works fine, but not 10.10. Here’s what I did to get it running on my Ubuntu Maverick machine.
 
What you’ll need:
 
- A computer running Ubuntu Maverick
 - A computer running Windows (it doesn’t have to be a computer. It can be a virtual machine running Windows in Virtualbox)
 - A copy of Photoshop CS5 installer. You can get the trial version at Adobe website

 

 
## Let’s get started
 
In your Windows machine, download (if you don’t own a copy) and install the Photoshop CS5.
 
Once the installation is completed, go the Start menu and type “regedit” on the search bar. The registry window will appear. Navigate to “HKEY_LOCAL_MACHINE -> Software -> Adobe“, right click the Adobe folder and select “Export”. When prompted, name the file “adobe.reg”.
 
Back to your Ubuntu Maverick machine, we will need to install wine and the Microsoft true type fonts
 
This will create the “.wine” folder and prepare wine for usage.
 
Next, we are going to perform some hacks
 
## Copying Photoshop files from Windows
 
Since we can’t get the installer to work in Ubuntu 10.10, we have to copy the core files from Windows to the Ubuntu machine. Folders/files you need to copy/paste are listed down below:
 
Lastly, save the “adobe.reg” file to the Home folder. In your terminal, type:
 
This will import the “adobe.reg” into the wine registry.
 
That’s it. Now go to “Home -> .wine -> drive_c -> Program Files -> Adobe ->Adobe Photoshop CS5“, right click on the Photoshop.exe file and select “Open with Wine Windows Program Loader”.
 
Photoshop CS5 should load. You can also add a shortcut to the Application Menu for quick access.
 
Note: 
 
1. Some people have mentioned that Photoshop CS5 in Ubuntu crashed with the text function. This has been fixed with the addition of atmlib.dll file.
 
2. Complex PSD file should load without problem. 
 
3. The above mods were done with wine version 1.2.1. and Photoshop CS5 trial version. If you are using other version of wine or Photoshop, there is no guarantee that the above method will work.
 
## Alternative to Photoshop CS5
 
For those who can’t get Photoshop CS5 to work, or find it too heavy for your daily usage, you can try out PhotoShop CS5 Portable. This is the unofficial portable version of Photoshop CS5 (not released by Adobe) and the installer work fine with wine. You will still need the atmlib.dll file for the text function to work.
 
PS: I am not going to tell you where to download the portable version. You can ask big brother G for answer. Also, any comment with links pointing to the file will also be deleted
 
Image credit: realtimecounter
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




