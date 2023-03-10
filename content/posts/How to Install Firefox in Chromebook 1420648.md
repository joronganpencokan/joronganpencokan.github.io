---
title: "Unveiling The Ultimate Hack: Installing Firefox on a Chromebook Like A Pro!"
ShowToc: true 
date: "2023-05-30"
author: "Stan Tuck"
---
*****
Unveiling The Ultimate Hack: Installing Firefox on a Chromebook Like A Pro!

Chromebooks are widely known for their lightning-fast performance, long battery life, and simplicity in design. However, Chrome OS has its limitations when it comes to software and app availability. For instance, the default browser on a Chromebook is Google Chrome, and it usually suffices for casual browsing.

But what if you want to use a different browser on your Chromebook, say Mozilla Firefox? Well, you'll be pleased to know that it's possible to install Firefox on your Chromebook with relative ease. In this article, we'll show you how to do it like a pro.

Step 1: Enable Developer Mode

Before you can install Firefox on your Chromebook, you need to enable developer mode on it. You can do this by following these steps:

1. Press and hold the Esc + Refresh + Power buttons simultaneously until the recovery screen appears.

2. Press Ctrl + D to enable developer mode.

3. Press Enter to start the process.

4. Your Chromebook will reboot and erase all local data.

5. After reboot, press Ctrl + Alt + T to open the Chrome OS terminal.

6. Type shell and press Enter.

7. Type sudo su and press Enter.

8. Type the system password if prompted.

Once developer mode is enabled, you can proceed to the next step.

Step 2: Download and Install Crouton

Crouton is a tool that makes it possible to install Linux on your Chromebook. To install Crouton, follow these steps:

1. Download the latest version of Crouton from the official website.

2. Press Ctrl + Alt + T to open the terminal.

3. Type shell and press Enter.

4. Type sudo install -Dt /usr/local/bin -m 755 ~/Downloads/crouton and press Enter.

5. Type sudo crouton -t xfce,xiwi -r buster -n firefox and press Enter.

The installation process may take some time, so be patient.

Step 3: Install Mozilla Firefox

With Crouton installed, you can now install Mozilla Firefox on your Chromebook. To do this, follow these steps:

1. Press Ctrl + Alt + T to open the terminal.

2. Type sudo startxfce4 to enter the Linux environment.

3. Open the Mozilla Firefox website and download the Linux version of Firefox.

4. After downloading, locate the downloaded file in the Downloads folder.

5. Right-click on the file and select Open with Other Application.

6. Select the Firefox Web Browser application.

Voila! You've successfully installed Firefox on your Chromebook using Crouton. The next time you want to use Firefox, simply enter the Linux environment by typing sudo startxfce4 in the terminal and launch Firefox.

In conclusion, installing Firefox on a Chromebook may seem like a daunting task, but with the right tools and steps, it's possible to do it like a pro. By following the steps outlined in this article, you can enjoy the added flexibility that comes with having multiple browsers on your Chromebook.

{{< youtube qUo8eY6KdaA >}} 



Chromebook runs Chrome OS, which is essentially the Google Chrome browser. When you power on your Chromebook, the Chrome browser will launch automatically so you can surf the Web immediately. What if you are not a fan of Google Chrome? Or perhaps you are paranoid about the data Google is collecting behind your back when you are using its browser. Luckily, there are several ways you can install Firefox on Chromebook. Here is how you can do so.
 
## Install Firefox Android app
 
Most of the newer Chromebook comes with support for Android apps, which means you can easily install Firefox from the Play Store.
 
1. Open up Play Store on your Chromebook.
 
2. Do a search for Firefox.
 

 
There are several Firefox browsers that you can choose from, namely the standard Firefox, Firefox Focus and Firefox Preview. Firefox Focus is a minimal privacy browser that blocks a wide range of online trackers. Firefox Preview is an experimental browser by Mozilla. If you are looking for a browser with the most features, installing the standard Firefox browser is your best bet.
 
3. After the installation, you will be able the use the Android version of the Firefox browser.
 
Firefox for Android supports extensions, too, though the choices are pretty limited. Since it is a mobile browser at its core, you won’t get a good desktop user experience.
 
## Install Firefox as Linux app
 
If your Chromebook supports Linux apps, then you can install the Linux version of desktop Firefox.
 
To check if your Chromebook supports the Linux app, open the menu drawer and open Settings.
 
In the Settings, search for “linux.”
 
If you see the “Linux (beta)” option, then your Chromebook can install the Linux app. Click on it to enable it (if you have not done so).
 
### Install Firefox ESR
 
The underlying Linux container is running Debian, and only Firefox ESR is available in its repository. Open the terminal in the menu drawer. Type the following command to install Firefox-ESR.
 
Once the installation is completed, you should see a Firefox icon in the dock. You can start to use Firefox in Chromebook.
 
Firefox-ESR stands for Firefox Extended Support Release, which is a long-term support release. It is a stable release meant for enterprise use. Releases will be maintained for more than a year, with point releases containing security updates coinciding with regular Firefox releases. New features in the regular Firefox releases will only be made available in the ESR at the next major release, after the end of the current release’s cycle.
 
### Install the standard Firefox
 
If you want to use the regular Firefox release instead of Firefox ESR, here is one simple way to install it in Chromebook.
 
1. First install Firefox-ESR. This will install the dependency files required by Firefox.
 
2. Next, remove Firefox-ESR without removing its dependencies:
 
3. Go to the Mozilla website and download Firefox to your Linux home folder. (Your Linux Home folder is the “Linux files” directory in the Files app.)
 
4. Extract the tar file to your Home folder with the following command in the Terminal. (Change the Firefox filename in the command below.)
 
You should now see a Firefox folder.
 
5. Lastly, we are going to create a Firefox desktop icon. In the terminal, type the following:
 
In the editor, paste the following:
 
Change “USERNAME” to your username in the Linux terminal. Your username is the name in the terminal before “@penguin.” In my case my username is “damienohwj.”
 
Save (Ctrl + o) and exit (Ctrl + x) the nano editor.
 
6. You should now see a Firefox icon in the menu drawer. (If not, restart your Chromebook.) Click on it and the Firefox browser will launch. It will also auto-update itself in the future.
 
## Conclusion
 
While the Chrome browser is the default browser in Chromebook, that doesn’t mean you have to be stuck with it. With support for Android and Linux apps, you now have options to install the browser of your choice, including Firefox. If you like Opera or Vivaldi, you can install those as well.
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




