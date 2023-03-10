---
title: "Get the Ultimate Secret to Fix Your Ubuntu Oneiric Dropbox Icons in Just a Few Clicks!"
ShowToc: true 
date: "2023-01-28"
author: "Charles Adams"
---
*****
Title: Get the Ultimate Secret to Fix Your Ubuntu Oneiric Dropbox Icons in Just a Few Clicks!

If you're running the Ubuntu Oneiric operating system on your computer and you're having trouble with your Dropbox icons, then you're in luck! In just a few clicks, you can fix the issue and get back to using the popular cloud storage service with ease. In this article, we'll show you how to get the ultimate secret to fix your Ubuntu Oneiric Dropbox icons in just a few clicks!

Step 1: Open your terminal

The first step is to open your terminal by pressing the Ctrl+Alt+T keys. Once the terminal is open, you'll need to input a few commands to fix the Dropbox icon issue.

Step 2: Install the Dropbox icon package

The next step is to install the Dropbox icon package. To do this, input the following command in your terminal:

sudo apt-get install nautilus-dropbox

Once the package is installed, your Dropbox icons should start working properly.

Step 3: Restart Nautilus

If your Dropbox icons still aren't working, you may need to restart Nautilus. To do this, input the following command in your terminal:

nautilus -q

This will close Nautilus and restart it. Once Nautilus has restarted, your Dropbox icons should be working properly.

Step 4: Log out and log back in

In some cases, you may need to log out of your Ubuntu Oneiric system and then log back in to get your Dropbox icons to work properly. To do this, click on the power button in the top right-hand corner of your screen and select "Log Out". Once you've logged out, log back in and check to see if your Dropbox icons are working correctly.

Conclusion

If you're having trouble with your Dropbox icons in Ubuntu Oneiric, don't worry! By following these easy steps, you can fix the issue in just a few clicks. Remember to install the Dropbox icon package, restart Nautilus if needed, and log out and log back in if necessary. With these tips, you'll be back to using Dropbox like a pro in no time!

{{< youtube g-FZCIF0HJw >}} 



If you are using Ubuntu Oneiric and Dropbox at the same time, you will find that the Nautilus Dropbox extension does not work as well as intended. While the Dropbox daemon is working fine and it will sync all files you place in the Dropbox folder, the sync icon and the Dropbox contextual menu is no longer there. This means that you can’t see whether the sync is successful or not and also access Dropbox feature, particularly the public link and shareable link, from the context menu. Here’s how you fix it (and it is incredibly simple).

The reason for this is because the Dropbox installer installs itself into the Nautilus extensions 2.0 folder while Nautilus 3.x is using the extensions 3.0 folders for the icons and context menu. To fix this, we just have to create a symlink between the respective files in extensions 2.0 and 3.0. 
 
Open a terminal and type:
 
Restart Nautilus:
 
That’s it. Open your Dropbox folder and you should see the sync icon and the Dropbox entry in the context menu.
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




