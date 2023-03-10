---
title: "Unlock the Secret to Browsing Bliss: Learn How to Install Safari on Linux Today!"
ShowToc: true 
date: "2022-11-14"
author: "Michael Krzeczkowski"
---
*****
# Unlock the Secret to Browsing Bliss: Learn How to Install Safari on Linux Today!

If you're a Linux user, you're probably familiar with the challenge of finding the right browser. There are plenty of options available, such as Firefox, Chromium, and Opera, but what if you're looking for something different? What if you're used to browsing the web on a Mac or an iPhone and miss the functionality of Safari? Fortunately, there's a way to install Apple's browser on your Linux desktop. In this article, we'll guide you through the process of installing Safari on Linux.

## Step 1: Check Your System Requirements

Before you start the installation process, make sure your Linux system meets the required specifications for running Safari. According to Apple, the minimum system requirements for running Safari are:

* A Mac computer with an Intel processor or an iPhone, iPad, or iPod touch with iOS 12 or later
* Mac OS X 10.11.6, macOS 10.12.6 or later, or iOS 12 or later
* At least 2 GB of RAM
* A screen resolution of 1280x800 or higher

If your Linux machine meets these requirements, you're ready to move on to the next step.

## Step 2: Download and Install Wine

Safari is not available for Linux, so we need to use some trickery to get it running. The solution is to use Wine, a popular compatibility layer that allows Windows applications to run on Linux. To install Wine, follow these simple steps:

1. Open a terminal window on your Linux desktop.
2. Type the following command to add the Wine repository to your system:

```bash
sudo add-apt-repository ppa:ubuntu-wine/ppa
```

3. Type the following command to update your package list:

```bash
sudo apt-get update
```

4. Type the following command to install Wine:

```bash
sudo apt-get install wine-stable
```

Once Wine is installed, we're ready to move on to the next step.

## Step 3: Download and Install Safari

Now that we have Wine installed, it's time to download Safari. You can download the latest version of Safari from the Apple website.

1. Open your web browser and go to the [Safari download page](https://www.apple.com/safari/).
2. Click on the "Download" button to download the Safari installer.
3. Once the installer has finished downloading, go to your Downloads folder and double-click on the Safari installer file to begin the installation process.
4. Follow the on-screen instructions to complete the installation.

Once Safari is installed, it should automatically launch in Wine. If not, you can launch Safari by typing the following command in a terminal window:

```bash
wine "/path/to/safari.exe"
```

Replace "/path/to/safari.exe" with the actual path to the Safari executable file.

## Step 4: Enjoy Browsing Bliss with Safari

Congratulations! You have successfully installed Safari on your Linux desktop. You can now enjoy browsing the web with the same browser you're used to from your Mac or iOS device. Keep in mind that Safari may run a bit slower on Linux than on a Mac, but it should still work perfectly fine for most use cases.

In conclusion, installing Safari on Linux is not as complicated as it may seem. With the help of Wine, you can easily get your hands on Apple's popular browser and enjoy the same browsing experience you're used to. Give it a try and see for yourself how easy it is to unlock the secret to browsing bliss!

{{< youtube 6WgjQpm9VWE >}} 



When you think of the major web browsers, chances are that Apple’s Safari features somewhere on your list. However, despite its popularity, Safari has never been officially released for Linux – particularly strange considering macOS and Linux both have historical ties to UNIX.
 
If you’re a Linux user and a web developer and need to provide support for the Safari browser, the good news is that there are some workarounds to get Safari up and running on Linux. Although you’ll be restricted to Safari 5, this version still has everything you need for surfing the Web.
 
## Installing Safari Browser on Linux
 
There are two potential workarounds for installing Safari on Linux: using WINE (the compatibility layer, not the drink) or using WINE and PlayOnLinux, which provides a graphical user interface (UI) for WINE. 
 
As an added bonus, you can use WINE and PlayOnLinux to install many other Windows applications beside Safari.
 
### How to Install WINE
 
WINE is one of the most well-known Linux packages and is found in most Software Center/Package managers. In Ubuntu (or Ubuntu-based distro), you can install WINE with the following command:
 
One thing to note is that the WINE version in Ubuntu is pretty outdated. If you want to get the latest stable version of WINE, do the following:
 
- Add the WINE key.

 
- Add the repository.

 
The above command is for Ubuntu 21.10 (impish). If you are using version other than Ubuntu 21.10, change the name accordingly (like “bionic,” “xenial,” etc.)
 
- Update the system:

 
- Lastly, install the stable version of WINE.

 
WINE will now be installed. For more information, refer to our guide on installing WINE on Linux.
 
### Installing Safari using WINE
 
Before downloading Safari, we need to create a download and build directory. 
 
- Open a Terminal window and run the following commands:

 
- Download Safari using a wget command:

 
- Once the download is complete, launch Safari Setup using the following:

 
- At this point you may be prompted to download some additional software, such as Mono or Gecko. If prompted, click “Install” and wait for these packages to download.

 
- Once you have all the necessary supporting software, the Safari Installer should launch automatically.

 
Once you’ve completed the standard Safari setup, the web browser will be installed, and you can start using Safari on Linux! 
 
### Installing Safari Using PlayOnLinux
 
WINE isn’t always the most user-friendly software, so you may want to consider installing PlayOnLinux, which provides a graphical user interface for the underlying WINE code.
 
- To install PlayOnLinux, use the following command:

 
- You can now find PlayOnLinux in your Applications menu.

 
- In the PlayOnLinux window, select “Install a program.”

 
- Enter “Safari” in the search bar.

 
- When the web browser appears, select it and click “Install.” Read the disclaimer, and if you accept it, click “Next -> Next.”

 
The Safari installer will be downloaded to your computer.
 
### Using the Safari Install Wizard in Linux
 
Once PlayOnLinux is installed, It will display a custom installation wizard that will guide you through the installation of Safari. 
 
- The screen will show a brief summary of the installer’s maintainer as well as where it will install the browser.

 
- Press “Next” to begin the installation process. The installer will first create a sandbox where it will install a version of WINE that is compatible with Safari in Linux.

 
- In some cases, PlayOnLinux will ask if you want to install the optional WINE Mono package. This is a compatibility layer that ensures .NET programs have the required DLL files to work properly. If you receive this message, press “Install.”

 
- PlayOnLinux will also ask you if you want to install the optional WINE Gecko package. Similar to Mono, this will provide a more seamless compatibility with the Safari browser. Once again, press “Install.”The wizard will ask whether you want to use a custom binary or download the installer. Select “Download the program,” then press “Next.”

 
- PlayOnLinux will run the Safari installer, and you can proceed with the standard browser installation process.Be sure to uncheck both the “Install Bonjour for Windows” and “Automatically update Safari” options during the install.

 
## Installing a Safari Theme for Firefox in Linux
 
While using a native Safari 5 client in Linux can be helpful for some users. This particular version of the browser can present some issues, especially if you are visiting modern websites. This is mostly because the Safari 5 browser no longer receives new updates from Apple.
 
As a result, using this version of Safari can result in either broken or insecure websites. For example, it is not possible to access YouTube from a native Safari 5 client.
 
One way of dealing with this issue is to use a modern browser and convert it to look and feel like the Apple browser. For example, it is possible to take Firefox and theme it to look like the modern version of Safari.
 
### Converting Firefox through White Sur GTK
 
Converting Firefox to look like Safari is relatively simple with the WhiteSur-gtk theme for Firefox.
 
- Download the theme by either downloading the ZIP file from the author’s Github page or running the following command:

 
- Extract the repository’s ZIP file to the current working directory and go inside it by running the following commands:

 
- Run the initial install script, which will prepare all the necessary files and dependencies for your Firefox theme, by running the following command:

 
- Run the Firefox theme installer by typing the following:

 
- Doing this will, then, automatically copy all the necessary settings and configurations for your Firefox client.

 
It’s important to note that the installer will not run if Firefox is currently running. Once done, however, you can reload the browser to look at your converted Firefox instance.
 
If all this talk made you curious about what you can do more with Linux. You can check this article where we discuss how you can use sed for basic tasks.
 
## Frequently Asked Questions
 
Image credit: Unsplash. All screenshots by Ramces Red.
 
### Is it possible to install Safari in Linux using the Mac installer?
 
Sadly, no. While it is possible to install DMG files in Linux, the native Safari browser for macOS is purpose built to only run for that operating system, as the browser uses Mac-specific functions which allow it to integrate well into macOS. For example, the Quick Note feature in Safari relies on external Apple programs to work properly.
 
### I already have WINE installed. Is it alright to install PlayOnLinux on top of it?
 
Yes! By default, PlayOnLinux creates its own set of virtual drives where it places the custom WINE version that it uses. Because of that, it is safe to install PlayOnLinux alongside with a mainline version of WINE. For example, when you install Safari through PlayOnLinux, it creates a clean sandbox where it installs all the programs and WINE patches that it needs.
 
Further, this approach also means that removing a program that you previously installed through PlayOnLinux is incredibly simple: press “Right click” on the “Safari 5” entry in the main menu and select “Remove.”
 
### Is it possible to remove the Safari theme and return Firefox to the default?
 
Yes! It is relatively simple to remove the Safari theme and revert your Firefox installation back to its default settings. First, go back to the White Sur directory that you extracted. From there, you then need to type the following command: ./tweaks.sh -f -r && ./install.sh -u.
 
Doing that will allow you to remove all the Safari-related files for Firefox as well as delete all theme files from your machine. With that done, the last thing that you need to do is to restart the browser to reload your default settings.
 
Ramces is a technology writer that lived with computers all his life. A prolific reader and a student of Anthropology, he is an eccentric character that writes articles about Linux and anything *nix.
 
Our latest tutorials delivered straight to your inbox




