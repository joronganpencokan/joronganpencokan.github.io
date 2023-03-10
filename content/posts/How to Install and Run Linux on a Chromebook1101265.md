---
title: "Unlock the Secret Power of Your Chromebook: Learn How to Easily Install and Run Linux!"
ShowToc: true 
date: "2023-03-11"
author: "Edward Bush"
---
*****
# Unlock the Secret Power of Your Chromebook: Learn How to Easily Install and Run Linux!

Chromebooks have become popular due to their simplicity, portability, and affordability. However, many users feel limited by Chrome OS, the operating system developed by Google for these devices. If you own a Chromebook, did you know that you can run Linux alongside Chrome OS, unlocking a world of additional software and customization options? In this article, we'll explore how to install and run Linux on your Chromebook, including some popular distributions and tools.

## What is Linux?

Before we dive into the installation process, let's briefly explain what Linux is. Linux is a free, open-source operating system based on Unix. It has been developed by thousands of contributors worldwide and is used in various applications, from mobile devices to servers. Linux is known for its stability, flexibility, and security, and it comes with a broader range of software than Chrome OS.

## Installing Linux on Your Chromebook

There are several ways to install Linux on a Chromebook, depending on your model and preferences. However, the easiest and most versatile method is to use a tool called Crouton (short for "Chromium OS Universal Chroot Environment"). Crouton creates a virtual machine within Chrome OS, allowing you to run Linux alongside it.

Here are the steps to install Crouton and Linux on your Chromebook:

1. Enable developer mode on your Chromebook. This will wipe all your data, so backup your important files first. To enable developer mode, press the Esc+Refresh+Power buttons simultaneously, then follow the on-screen instructions.

2. Download and open the Crouton script from the official website (https://github.com/dnschneid/crouton).

3. Choose the Linux distribution you want to install (e.g., Ubuntu, Debian, Kali Linux, etc.) and enter the appropriate commands in the terminal.

4. Wait for the installation to complete (it may take a while), then run the "startxfce4" command to launch the Linux desktop.

Congratulations! You now have Linux running on your Chromebook. To switch between Chrome OS and Linux, press Ctrl+Alt+Shift+Back/Forward buttons. You can also customize your Linux environment by installing software and tweaking the settings to your liking.

## Popular Linux Distributions and Tools for Chromebooks

Now that you have Linux installed, let's explore some of the best distributions and tools you can use on your Chromebook.

### Ubuntu

Ubuntu is one of the most popular Linux distributions, known for its user-friendly interface and extensive software library. You can install Ubuntu on your Chromebook using Crouton or a dedicated installer like GalliumOS. Once installed, you can access the Ubuntu Software Center and install thousands of free and open-source applications, including office suites, media players, graphic editors, programming tools, and more.

### Kali Linux

Kali Linux is a popular distribution among security professionals and enthusiasts. It comes with pre-installed tools for penetration testing, network analysis, digital forensics, and other security tasks. You can use Kali Linux on your Chromebook to test your network's security or learn more about ethical hacking.

### Crouton Integration

Crouton Integration is a set of scripts that allow you to use your Chromebook's hardware (such as audio, video, touchpad, and USB devices) within the Linux environment. It also enables clipboard sharing and easy file transfer between Chrome OS and Linux. To install Crouton Integration, follow the instructions on the official GitHub page (https://github.com/iSoron/u2f-tutorial/tree/master/crouton-integration).

### Wine

Wine is a compatibility layer that allows you to run Windows programs on Linux. You can install Wine on your Chromebook and run some Windows applications, although not all of them may work correctly. Wine is not a perfect solution, but it can give you access to some programs that are not available on Linux natively.

Conclusion

Linux can give your Chromebook a new level of power and versatility, allowing you to run a broader range of software and configurations. By installing Linux alongside Chrome OS, you can enjoy the best of both worlds and switch between them as you wish. We have seen how to install Linux on your Chromebook using Crouton and explore some popular distributions and tools. With a bit of experimentation and learning, you can unlock the full potential of your Chromebook and use it for various tasks and hobbies. Happy hacking!

{{< youtube Nwfa97Z0mJQ >}} 




Run a full-fledged version of the Linux operating system on your Chromebook, opening up a whole world of possibilities on what is essentially a low-budget machine.

 

Before installing Ubuntu on your Chromebook, you first need to enable Developer Mode.

 
##   Enable Developer Mode  
 

While most of your data in Chrome OS is stored server-side in the cloud, you may have important files saved locally, such as those found in your Downloads folder. In addition to disabling certain security restrictions and allowing you to install a customized version of Ubuntu, activating Developer Mode deletes all local data on a Chromebook automatically. Therefore, back up essential local data on an external device or move it to the cloud before taking the steps below.

 
- Turn on your Chromebook, then press and hold the Esc+Refresh keys and tap the Power button. When the forced reboot begins, release the keys.
 - After the reboot is complete, a screen appears with a yellow exclamation point and a message that Chrome OS is missing or damaged. Press Ctrl+D to initiate Developer Mode.
 - The following message displays: To turn OS verification OFF, press ENTER. Press the Enter key.
 - A new screen appears stating that OS verification is off. Don't touch anything at this point. After a few sections, you receive notification that the Chromebook is transitioning to Developer Mode. This process may take some time and could involve multiple reboots. You are eventually returned to the OS verification is OFF message, accompanied by a red exclamation point. Ignore this message and wait until you see the welcome screen for Chrome OS.
 - Since all local data and settings were deleted when you entered Developer Mode, you may have to re-enter your network details, language, and keyboard orientation on the OS welcome screen, as well as agree to the operating system's terms and conditions. Once completed, sign in to your Chromebook.

 
##   Install Ubuntu Using Crouton  
 

The main reasons to choose Crouton are its simplicity, and it can run Chrome OS and Ubuntu side-by-side, eliminating the need to hard boot into one operating system at a time.

 

Turn on your Chromebook, then press and hold the Esc+Refresh keys and tap the Power button. When the forced reboot begins, release the keys.

 

After the reboot is complete, a screen appears with a yellow exclamation point and a message that Chrome OS is missing or damaged. Press Ctrl+D to initiate Developer Mode.

 

The following message displays: To turn OS verification OFF, press ENTER. Press the Enter key.

 

A new screen appears stating that OS verification is off. Don't touch anything at this point. After a few sections, you receive notification that the Chromebook is transitioning to Developer Mode. This process may take some time and could involve multiple reboots. You are eventually returned to the OS verification is OFF message, accompanied by a red exclamation point. Ignore this message and wait until you see the welcome screen for Chrome OS.

 

Since all local data and settings were deleted when you entered Developer Mode, you may have to re-enter your network details, language, and keyboard orientation on the OS welcome screen, as well as agree to the operating system's terms and conditions. Once completed, sign in to your Chromebook.

 

To get started, open the Chrome browser, and follow these steps:

 
- Go to the Crouton official GitHub repository.
 - Crouton
 - Click the goo.gl link, located to the right of the Chromium OS Universal Chroot Environment header.
 - A Crouton file downloads to your Downloads folder. Open the Chrome OS developer shell in a new browser tab by pressing Ctrl+Alt+T.
 - Type shell and press the Enter key.
 - At the prompt, enter sudo sh ~/Downloads/crouton -e -t xfce, then press the Enter key. On a Chromebook device with a touchscreen, use the following syntax instead: sudo sh ~/Downloads/crouton -e -t touch,xfce.
 - The latest version of the Crouton installer downloads. You're prompted to provide and verify both a password and an encryption passphrase because the Ubuntu installation is encrypted through the -e parameter in the previous step. While this flag isn't required, it is recommended. Choose a secure password and passphrase that you will remember and enter these credentials accordingly, if applicable.
 - After the key generation completes, the Crouton installation process begins. This process takes several minutes and requires minimal intervention. However, you can view details of each step in the shell window as the installation progresses. You are eventually asked to define a username and password for the primary Ubuntu account toward the end of the process.
 - After the installation completes, the command prompt displays. Enter sudo startxfce4, then press the Enter key. If you chose encryption in the previous steps, you are prompted for your password and passphrase.
 - An Xfce session begins, and the Ubuntu desktop interface appears.
 - Crouton runs Chrome OS and Ubuntu simultaneously. To switch between the two operating systems without rebooting, use the Ctrl+Alt+Shift+Back and Ctrl+Alt+Shift+Forward keyboard shortcuts.
 - These shortcuts don't work on a Chromebook with an Intel or AMD chipset, as opposed to ARM. In this case, use the Ctrl+Alt+Back, Ctrl+Alt+Forward, and Ctrl+Alt+Refresh shortcuts.

 
##   Start Using Linux  
 

After you enable Developer Mode and install Ubuntu, follow these steps to launch the Linux desktop each time you power on your Chromebook. You'll see the warning screen stating that OS verification is off every time you reboot or turn the power on because Developer Mode remains active until you manually disable it, and is required to run Crouton.

 

Go to the Crouton official GitHub repository.

 

Click the goo.gl link, located to the right of the Chromium OS Universal Chroot Environment header.

 

A Crouton file downloads to your Downloads folder. Open the Chrome OS developer shell in a new browser tab by pressing Ctrl+Alt+T.

 

Type shell and press the Enter key.

 

At the prompt, enter sudo sh ~/Downloads/crouton -e -t xfce, then press the Enter key. On a Chromebook device with a touchscreen, use the following syntax instead: sudo sh ~/Downloads/crouton -e -t touch,xfce.

 

The latest version of the Crouton installer downloads. You're prompted to provide and verify both a password and an encryption passphrase because the Ubuntu installation is encrypted through the -e parameter in the previous step. While this flag isn't required, it is recommended. Choose a secure password and passphrase that you will remember and enter these credentials accordingly, if applicable.

 

After the key generation completes, the Crouton installation process begins. This process takes several minutes and requires minimal intervention. However, you can view details of each step in the shell window as the installation progresses. You are eventually asked to define a username and password for the primary Ubuntu account toward the end of the process.

 

After the installation completes, the command prompt displays. Enter sudo startxfce4, then press the Enter key. If you chose encryption in the previous steps, you are prompted for your password and passphrase.

 

An Xfce session begins, and the Ubuntu desktop interface appears.

 

Crouton runs Chrome OS and Ubuntu simultaneously. To switch between the two operating systems without rebooting, use the Ctrl+Alt+Shift+Back and Ctrl+Alt+Shift+Forward keyboard shortcuts.

 
These shortcuts don't work on a Chromebook with an Intel or AMD chipset, as opposed to ARM. In this case, use the Ctrl+Alt+Back, Ctrl+Alt+Forward, and Ctrl+Alt+Refresh shortcuts.
 
- Return to the developer shell interface by using the Ctrl+Alt+T keyboard shortcut.
 - Type shell at the crosh prompt and press Enter.
 - Type sudo startxfce4, then press Enter.
 - Enter your encryption password and passphrase if prompted.

 

The version of Ubuntu that you installed doesn't come with much pre-installed software. The most common method for locating and installing Linux applications is through apt-get. This command-line tool searches for and downloads countless applications within Ubuntu.

 

Return to the developer shell interface by using the Ctrl+Alt+T keyboard shortcut.

 

Type shell at the crosh prompt and press Enter.

 

Type sudo startxfce4, then press Enter.

 

Enter your encryption password and passphrase if prompted.

 

AMD and Intel-based Chromebooks offer access to more working applications than those running ARM chips. However, ARM-based Chromebooks run some of the most popular Linux applications.

 
##   Back up Your Data  
 

While most data and settings in Chrome OS are automatically stored in the cloud, the same cannot be said for files created or downloaded during your Ubuntu sessions. Use Crouton to back up your Ubuntu data.

 
- Launch the developer shell interface by pressing Ctrl+Alt+T.
 - Type shell at the crosh prompt and press the Enter key.
 - Type sudo edit-chroot -a, then press Enter.
 - The name of your chroot displays in white text (for example, precise). Type the following syntax followed by a space and the name of your chroot: sudo edit-chroot -b. (for example, sudo edit-chroot -b precise), then press Enter.
 - When the backup process concludes, the chroot displays a message that it finished backing up along with a path and filename. Generally, the backup is a tar file located in your Chrome OS Downloads folder, which is shared and accessible from both operating systems.

 
##   Remove Linux From Your Chromebook  
 

To remove Linux from your Chromebook, follow this procedure:

 

Launch the developer shell interface by pressing Ctrl+Alt+T.

 

Type shell at the crosh prompt and press the Enter key.

 

Type sudo edit-chroot -a, then press Enter.

 

The name of your chroot displays in white text (for example, precise). Type the following syntax followed by a space and the name of your chroot: sudo edit-chroot -b. (for example, sudo edit-chroot -b precise), then press Enter.

 

When the backup process concludes, the chroot displays a message that it finished backing up along with a path and filename. Generally, the backup is a tar file located in your Chrome OS Downloads folder, which is shared and accessible from both operating systems.

 
- Restart your Chromebook.
 - When the OS verification is OFF message appears, press the spacebar.
 - Confirm reactivating OS verification. Press the Enter key.
 - A notification alerts you that OS verification is now on. Your Chromebook reboots and is restored to its original state. After the process completes, the Chrome OS welcome screen appears.

 

Restart your Chromebook.

 

When the OS verification is OFF message appears, press the spacebar.

 

Confirm reactivating OS verification. Press the Enter key.

 

A notification alerts you that OS verification is now on. Your Chromebook reboots and is restored to its original state. After the process completes, the Chrome OS welcome screen appears.

 

Get the Latest Tech News Delivered Every Day




