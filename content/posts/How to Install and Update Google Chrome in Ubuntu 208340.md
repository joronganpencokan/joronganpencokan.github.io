---
title: "Revolutionize Your Ubuntu Experience: Learn How to Install and Update Google Chrome Like a Pro!"
ShowToc: true 
date: "2022-11-13"
author: "Monica Wicks"
---
*****
# Revolutionize Your Ubuntu Experience: Learn How to Install and Update Google Chrome Like a Pro!

Google Chrome is one of the most popular web browsers used globally, offering a stable and secure browsing experience across various platforms. If you are an Ubuntu user, you can upgrade your browsing experience by installing Google Chrome on your machine.

Here is a straightforward guide on how to install and update Google Chrome on your Ubuntu machine to enjoy a seamless browsing experience.

## Step 1: Download Google Chrome

Visit the Google Chrome website to download the latest version of the browser. Ensure that you download the appropriate package for your Ubuntu architecture (32 bit or 64 bit). The package comes in the form of a Debian file with a .deb file extension.

## Step 2: Install Google Chrome on Ubuntu

The next step is to install Google Chrome. You can either use the terminal or graphically install it. Here's how:

### Terminal Installation

1. Open your terminal by pressing "Ctrl + Alt + T" on your keyboard.
2. Use the "cd" command to navigate to the directory where you downloaded the Google Chrome package.
3. Type in "sudo dpkg -i Google-Chrome-Stable_current_amd64.deb" to start the installation process.

### Graphical Installation

1. Locate the directory where you downloaded the Google Chrome package
2. Double-click the package to open it.
3. Click on the "Install" button to start the installation process.

## Step 3: Update Google Chrome

To update Google Chrome, you need to ensure that you have the latest Chrome repository added to your system. You can do this by running the following command in your terminal:

```sudo sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list'```

Once you've added the repository, run the following command in your terminal to update Chrome:

```sudo apt update && sudo apt upgrade google-chrome-stable```

## Conclusion

Congratulations! You can now install and update Google Chrome on your Ubuntu machine with ease. By following these simple steps, you can upgrade your browsing experience and enjoy the full power of one of the most popular web browsers in the world. So, revolutionize your Ubuntu experience by installing Google Chrome like a pro!

{{< youtube CRXbjLbepqc >}} 



Most users who want to install Google Chrome in Ubuntu tend to use an App Store or go through Ubuntu Software. What they don’t know is that Google Chrome isn’t available in any major Linux distribution archives, so it can’t be installed directly from the Software Center. Here we show you how to install Google Chrome in Ubuntu.
 
## Download and Install Google Chrome
 
Since Google Chrome is not found in the Software Center, we need to download the installer from its website.
 
- Go to the official Google Chrome download page and click “Download Chrome.”

 
- Select the package for your Linux platform. This may be the 64-bit .deb (for Debian/Ubuntu), 64-bit .rpm (for Fedora/openSUSE), or, if you don’t use either of those, you can get a community-supported version.

 
Note: if you are using Arch Linux, Google Chrome is found in the AUR. You can install it with any of these AUR helpers.
 
- On the same page, read the Google Chrome Terms of Service, then click the blue “Accept & Install” button if you’re happy with what they have to offer (or don’t care what is written on it). The installer file should start to download.

 
- If this didn’t work for you, try a direct download of Google Chrome for Linux.
 - Once the download is completed, open your file manager and double-click on the installer package to begin the installation.

 
- Click the “Install” button once the software app opens.

 
- If prompted, enter your password.
 - Wait until the Software Installer installs the Chrome browser.

 
- Click “Launch” once the install is complete to open Google Chrome.

 
- Customize your options.

 
Enjoy the Google Chrome browser on Ubuntu.
 
## Install Chrome Using Flatpak Library
 
If you prefer a more direct method of obtaining Chrome, try using Flatpak. Chrome browser is available on Flathub; however, Google doesn’t support or manage the application on the platform, so you will be installing the package at your own risk. (You can learn how to install Flatpak on Ubuntu and other distributions.)
 
- Open the Terminal and type the following command:

 
- Press Y , then  Enter.

 
Let the Terminal download packages and install the browser.
 
Chrome will be installed successfully on Linux PC.
 
Open the menu and search for the browser.
 
## Manually Update the Chrome Browser on Ubuntu
 
There are a few ways to update Google Chrome on your Ubuntu machine. By default, on a regular update, the system will update Google Chrome, too. But if it fails to update on its own, you can use any of the following methods to manually update Google Chrome on your machine.
 
### Use Software Center
 
- Search and open “Software Center” from the menu.

 
- Click on “Updates” from the top menu.

 
- Click “Install” or “Install All” to update the packages.

 
Note: if your Ubuntu Software center is not working, we have fixes here.
 
### Use Command Line
 
- Open a terminal.
 - Run the sudo apt update command in the Terminal.
 - Type sudo apt --only-upgrade install google-chrome-stable command to upgrade Google Chrome only.

 
### Use Software Updater
 
- Open “Software Updater” from the menu.

 
- Click on the “Settings & Livepatch” button.

 
- Select “Other Software” from the top menu.
 - Check the box beside the APT Line of the Google repository and close the window.

 
The Software Updater will notify you of new software updates when they are available for your computer.
 
Tip: not keen on using Ubuntu? Check out other Debian-based Linux distributions here.
 
## Frequently Asked Questions
 
All screenshots by Krishna Kumar Silvery.
 
### Is there a Google Chrome package for 32-bit Ubuntu?
 
No, Google axed the Chrome 32-bit version in 2016.
 
### Is Flatpak Google Chrome safe?
 
While Flatpak is an open-source project, the Chrome package on the platform isn’t monitored or managed by Google. You have to install it at your own risk.
 
### Do I need to add the Google Chrome repository separately?
 
The Chrome DEB or RPM package has the repository info and saves it in the computer after installation. You don’t have to register the repository separately.
 
### Do I have to update the Flatpak packages separately?
 
Flatpak updates appear along with the system updates. You don’t have to add the Flathub repository or download additional tools to receive or update the applications. Use the universal command sudo apt update and install Flatpak app updates.
 
I'm a passionate writer.
 
Our latest tutorials delivered straight to your inbox




