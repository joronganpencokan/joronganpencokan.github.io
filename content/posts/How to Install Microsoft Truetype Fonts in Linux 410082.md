---
title: "Unlock a whole new world of typography on Linux with this one simple trick: Installing Microsoft Truetype fonts!"
ShowToc: true 
date: "2023-06-24"
author: "John Ancira"
---
*****
---
title: Unlock a Whole New World of Typography on Linux with This One Simple Trick: Installing Microsoft Truetype Fonts!
date: 2021-11-04
description: Learn how to install the popular Microsoft Truetype fonts on your Linux system and explore a world of new typography possibilities.
---

As a Linux user, you are probably well aware of the wide range of fonts available to you through the operating system's native font library. However, there may be times when you need access to a particular font that is not included in the library. One popular font family that is not included in Linux distributions is Microsoft's Truetype fonts.

The good news is that it is relatively easy to install these fonts on your Linux system, giving you access to a whole new world of typography possibilities. In this article, we will walk you through the process of installing Microsoft's Truetype fonts on your Linux operating system.

## What Are Microsoft Truetype Fonts?

Truetype is a popular font format, originally developed by Apple in the late 1980s, and later adopted by Microsoft for use in Windows. Truetype fonts are designed to be highly readable, scalable, and compatible with a wide range of devices, making them a popular choice for both print and digital media.

The Microsoft Truetype font family includes a wide range of styles and designs, from classic serif fonts to modern sans-serif fonts, each with its unique character and personality. Some of the most popular Microsoft Truetype fonts include Arial, Times New Roman, Georgia, and Verdana.

## How to Install Microsoft Truetype Fonts on Linux

To install Microsoft Truetype fonts on your Linux system, follow these simple steps:

### 1. Download the Microsoft Truetype font pack.

First, you need to download the Microsoft Truetype font pack. You can do this by visiting the Microsoft website and searching for "Microsoft Truetype font pack." Once you find the pack, click on the "Download" button to start the download process.

### 2. Extract the font files.

Once the font pack is downloaded, extract the font files to a folder on your system. You can do this by right-clicking on the downloaded file and selecting "Extract Here" or by using a file extraction tool.

### 3. Copy the font files to your Linux system's font folder.

Next, you need to copy the font files to your Linux system's font folder. The font folder is usually located in the "/usr/share/fonts/" directory. You can access this directory using the terminal or file manager.

```bash
sudo cp -r /path/to/font/files /usr/share/fonts/truetype/msttcorefonts/
```

### 4. Update the font cache.

Finally, you need to update your Linux system's font cache to register the new fonts. You can do this by running a simple command in the terminal.

```bash
sudo fc-cache -f -v
```

## Exploring the World of Microsoft Truetype Fonts on Linux

Once you have installed the Microsoft Truetype fonts on your Linux system, you can start exploring the unique typography possibilities they offer. Here are some tips to help you get started:

### 1. Experiment with different font styles and designs.

With the Microsoft Truetype fonts on your Linux system, you can experiment with different font styles and designs to find the perfect fit for your project. Try using classic serif fonts for a traditional look or modern sans-serif fonts for a more contemporary feel.

### 2. Use Microsoft Truetype fonts in your documents and presentations.

Microsoft Truetype fonts are compatible with a wide range of document and presentation software, including LibreOffice, OpenOffice, and GIMP. Use these fonts to add a professional touch to your documents and presentations.

### 3. Customize your Linux system with Microsoft Truetype fonts.

You can also use Microsoft Truetype fonts to customize your Linux system's look and feel. You can set these fonts as your system font, use them in your terminal, or even create custom themes using these fonts.

## Conclusion

Installing Microsoft Truetype fonts on your Linux system is a simple process that can unlock a whole new world of typography possibilities. With these fonts, you can add a professional touch to your projects and customize your Linux system to your liking. So why wait? Download the Microsoft Truetype font pack today and start exploring the world of typography on Linux!

{{< youtube rLZk7cWbycI >}} 



Although there are thousands of fonts available, the popularity of Windows leads to the extensive use of Microsoft’s fonts that come with the OS. For many users, fonts such as “Arial,” “Times New Roman” and “Impact” are considered standard. Thus, if you’re collaborating and exchanging documents with Windows users, you need to have access to these fonts even if you are using Linux.
 
Thankfully, it’s easy to bring those fonts onboard your Linux distribution. Let’s see how to do it.
 
## The Classic Installer
 
If you’re using a variant of Ubuntu, unlike users of other distributions, you still have access to an old installer that makes adding the core Microsoft fonts to your OS easy. To do that, enter in a terminal:
 
For Fedora (or any distro using rpm), here is an old, but still working, method to install Microsoft Fonts.
 
In Arch Linux, you can install the ttf-ms-fonts package from AUR.
 
A universal way to install Microsoft Fonts on any Linux distribution is to extract the fonts from Windows and move them to your system.
 
## Copy from Windows Installation
 
If you have access to a working Windows machine, you can copy the fonts from there. Run your favorite file manager and point it to “C:\Windows\Fonts.” Note that the path might be different if you didn’t use the default path when installing Windows. Select all files in that directory and copy them to your USB drive.
 
Transfer the font files back to your Linux machine and place them in the “.fonts” folder in your Home directory. If the “.fonts” folder (mind the dot in front of the name) doesn’t exist, create it.
 
## Copy from Windows 10 ISO
 
If you don’t have access to a Windows installation, you can easily download the Windows ISO file and extract the fonts from the ISO image. 
 
1. Download Microsoft’s official Download Windows 10 Disc Image (ISO File). Scroll a bit downward and select your edition from the pull-down menu – pick the latest “full” version available, not an upgrade.
 
Although we haven’t seen any difference in font availability between different product languages, we suggest you download either a version of Windows for your primary language or the “English International” option.
 
2. To extract the fonts from the Windows ISO, we will need 7Zip. If you have not installed it, do so with the command:
 
On OpenSUSE, you can try:
 
On Arch and other Arch-based distros like Manjaro, try this:
 
3. In the terminal, cd to the directory where you have downloaded the Windows ISO. First, you’ll have to extract a large archive that contains other files used for the installation of Windows. The font files we need are among them. To do that, use:
 
Replace “Win10_XXXX_EnglishInternational_x64” with the exact name of the Windows ISO file.
 
Note that this part of the process will take a while depending on your CPU’s performance. It will also demand more than 4 GB of space to extract the large file from the ISO.
 
4. After the process is completed, extract the Fonts directory from the “install.wim” archive. Run the command:
 
Like before, give it some time, and soon you’ll find all the fonts contained in the Windows installation media in a “fonts” subfolder next to the downloaded ISO.
 
## Install the fonts
 
The easiest way to install the fonts in Linux is by moving them to the “.fonts” folder in your Home directory. You can do that with:
 
On Arch, the “~/.fonts” folder is considered deprecated, so try the following instead:
 
Finally, for your new fonts to be available in most applications, update your installation’s font cache with:
 
Fire up any program like LibreOffice’s Writer, and you’ll find your newly-installed fonts among the ones you were already using.
 
Even if you have all the fonts, there are times when you have trouble identifying the fonts used, particularly in an image. Also, if what you need is the Windows application instead of the fonts, you can still run the Windows app in Linux via WINE.
 
OK's real life started at around 10, when he got his first computer - a Commodore 128. Since then, he's been melting keycaps by typing 24/7, trying to spread The Word Of Tech to anyone interested enough to listen. Or, rather, read.
 
Our latest tutorials delivered straight to your inbox




