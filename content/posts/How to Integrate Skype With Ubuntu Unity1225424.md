---
title: "Discover the Ultimate Hack to Effortlessly Integrate Skype with Ubuntu Unity!"
ShowToc: true 
date: "2023-02-24"
author: "William Crawford"
---
*****
Title: Discover the Ultimate Hack to Effortlessly Integrate Skype with Ubuntu Unity!

Are you a proud owner of a Linux-based system or specifically an Ubuntu Unity, but struggling to integrate the popular video chat application, Skype? Look no further as we have just the ultimate hack for you! In this article, we will go through a simple process to ensure a seamless integration of Skype with your Ubuntu Unity.

Step 1: Adding Canonical Partners Repository

To begin with, we first need to add the Canonical Partners repository, which is a repository for some proprietary software packages such as Skype. We can add the repository through the Ubuntu Software Center by following these simple steps:

● Open the Ubuntu Software Center
● Click on the Edit tab
● Choose Software Sources
● In the Software Sources window, select the Other Software tab
● Check the "Canonical Partners" option

Click on "Close" and "Reload." Wait for a few moments for the software center to update its repository.

Step 2: Downloading and Installing Skype

After we have added the Canonical Partners repository, now it's time to download and install Skype. We can do this through the Ubuntu Software Center as well, or we can use a simple command in the terminal. Let's go through both the methods one by one:

Method 1: Through the Ubuntu Software Center

● Open the Ubuntu Software Center
● Type "Skype" in the search bar
● Choose Skype from the results
● Click on "Install"

Method 2: Through the Terminal

If you prefer using the terminal, then you can simply enter the following command:

sudo apt install skypeforlinux

Step 3: Integrating Skype with Ubuntu Unity

Now that we have successfully installed Skype let's proceed towards integrating it with our Ubuntu Unity. The following instructions will guide you through the simple process:

● Go to the Unity Dash
● Type "Skype" in the search bar
● Right-click on the Skype icon
● Choose "Add to Launcher"

That's it! We have now integrated Skype with our Ubuntu Unity. You can easily access Skype by clicking on the icon in your Unity launcher.

In conclusion, we have just discovered the ultimate hack to effortlessly integrate Skype with Ubuntu Unity. By following the simple steps outlined in this article, you can easily install Skype and add it to your Unity launcher. Now you can enjoy seamless video chats with your friends and family without any hassle.

{{< youtube EuWYqolc73w >}} 



If you are both a Skype and Ubuntu user, you will know that Skype does not really integrate well into the system. While Skype comes with a Linux desktop client that you can install on Ubuntu, it doesn’t integrate itself into the system theme, nor does it makes use of the system notification panel. If you like a unified look and feel for Skype on Ubuntu (unity), here is the way to do it.
 
Skype-wrapper is a plugin that integrates Skype with Unity. It adds the Skype icon to the messaging menu and quicklist items to the launcher. It also uses the Unity notification style to notify you of incoming calls/messages. 
 
## Installation
 
Open a terminal and type:
 
The above commands assume that you have already installed Skype in your system.
 
## Running Skype-wrapper
 
Once you installed Skype and Skype-wrapper, you will find that there are two instances of Skype in your computer. You need to identify which is which and run only Skype-wrapper, and not Skype.
 
1. Open Nautilus File Manager and navigate to “usr/share/applications”. Scroll down the application list till you see two Skype icons. 
 

 
2. To identify which one is which, right click on the Skype icon and select Properties. The one that shows the “skype-wrapper” in the Command field is the one that you want. Drag this icon to the Unity Launcher.
 
3. Click on the icon to launch Skype. A popup will appear to prompt you to grant access to the skype-wrapper app. Check “Remember this selection” and click “Yes”.
 
Once it is authorized, you should see the Skype entry in the messaging menu and any incoming notification will follow the Unity style.  
 
Right clicking the Skype icon on the launcher also show the quicklist items. You can View Incoming Message and Add Contacts.
 
Skype-wrapper also comes with a Settings option that allows you to configure its behavior. From the dash, search for skype-wrapper and you should see the “Skype-Wrapper Settings” app. In the Settings, you can configure the events to show notification and whether the file transfer progress should appear in the launcher. 
 
## Removing Skype icon from the systray
 
After the unity integration, there is one thing left that you need to get rid of. If you can’t stand the green Skype icon that didn’t go well with the Unity theme, you can remove it by uninstalling the “sni-qt” package. Note that a few other application, such as Dropbox, depend on the “sni-qt” package to display icon in the systray, and removing this package will affect these apps as well. Here’s what you need to do:
 
The next time you launch Skype-wrapper, the green Skype icon won’t be around anymore.
 
## Uninstalling Skype-wrapper
 
To completely remove Skype-wrapper from your computer, first open up your Skype option and go to “Public API” (the last option in the left sidebar). Select “Skype4Py” and click Remove.
 
Next, uninstall skype-wrapper from your computer:
 
That’s it. 
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




