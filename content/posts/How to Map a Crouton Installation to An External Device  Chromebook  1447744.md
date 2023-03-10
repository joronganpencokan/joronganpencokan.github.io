---
title: "Unlock the Secret to Supercharging Your Chromebook: Learn How to Map Your Crouton Installation to an External Device Now!"
ShowToc: true 
date: "2023-05-26"
author: "Ellie Warren"
---
*****
# Unlock the Secret to Supercharging Your Chromebook: Learn How to Map Your Crouton Installation to an External Device Now!

If you're someone who loves using a Chromebook as your primary device for work or leisure, you're probably always looking for ways to improve your experience. Well, here's a secret that you need to know: mapping your Crouton installation to an external device can supercharge your Chromebook and give it extra power that you never thought possible.

Crouton is a program that enables users to install a Linux operating system on their Chromebooks, giving them access to a plethora of powerful tools and applications. However, the installation can take up a significant amount of storage space on your device, which might be a problem for some users who have limited storage or prefer to keep their devices as clean and organized as possible.

The good news is that you can map your Crouton installation to an external device, such as a USB drive or an SD card. By doing so, you can free up space on your Chromebook and make it run faster and smoother than ever before. In this article, we'll walk you through the steps on how to do it.

## Step 1: Prepare Your External Device

Before you can map your Crouton installation to an external device, you have to prepare it first. This means formatting your device to work with your Chromebook and ensuring that it has enough storage space to accommodate your Crouton installation.

To format your external device, connect it to your Chromebook and go to the "Settings" menu. Click "Device" and then "Storage Management." From there, select your external device and click "Erase."

Once your device is formatted, check its available storage space by clicking "Storage Management." Make sure that it has enough space to fit your Crouton installation, plus some extra space for other files and applications.

## Step 2: Install Crouton on Your External Device

The next step is to install Crouton on your external device. To do this, you need to open the terminal on your Chromebook and enter the command, "sudo sh ~/Downloads/crouton -r trusty -t xfce -e -f /media/removable/your_device_name/Crouton".

Note: Replace "trusty" with the release of Ubuntu you want to use, replace "xfce" with the desktop you want to use, and replace "your_device_name" with the name of your external device.

This command will install Crouton on your external device and allow you to access it from your Chromebook.

## Step 3: Access Your Crouton Installation on Your External Device

Now that you've installed Crouton on your external device, you can access it from your Chromebook. To do this, open the terminal and enter the command, "sudo startxfce4 -n your_chroot_name".

Note: Replace "your_chroot_name" with the name of your Crouton installation.

This command will start your Crouton installation on your external device and allow you to use it on your Chromebook.

## Step 4: Enjoy Your Supercharged Chromebook

Congratulations! You've successfully mapped your Crouton installation to an external device and supercharged your Chromebook. You can now enjoy the benefits of using Linux on your Chromebook without compromising its storage space and speed.

Conclusion

Mapping your Crouton installation to an external device is a simple process that can give your Chromebook a significant boost in performance. It frees up your device's storage space and allows you to access a powerful Linux operating system from your Chromebook. So, what are you waiting for? Give it a try and experience the difference for yourself.

{{< youtube UAAcQVJxfPk >}} 



You’ve heard of Crouton, right? It’s a really neat script written specifically for Chromebooks. It allows for you to install many different versions of Linux. This is a great thing, as it opens up Chrome devices to more operating systems.
 
Still, Chromebooks are notoriously low on storage space. Most of them max out at about 32 gigabytes of internal memory. For those that want to use a lot of big programs in their Crouton installations, this can be a big problem.
 
Fortunately, this lack of storage can easily be solved. With the help of this guide, you’ll be able to easily setup your Crouton installations to reside directly on an external device.
 
## Map Crouton to an SD card or USB stick
 
Before the installation can begin, you’ll need to set up your directories. Open the ChromeOS  terminal by pressing “Ctrl + Alt + T” on your keyboard, type in shell and press the Enter key.
 

 
Once the shell is open, you’ll need to move to the directory that the Crouton installer normally places the chroots.
 
While you’re in there, you’ll need to do a few things. First, however, you’ll need to make a new chroot directory on your removable SD card or USB stick.
 
Note: You have to change “NAME-OF-SD-CARD-OR-FLASH-DRIVE” to the actual name of your external device.
 
After the directory is made, it’s time to symbolically link it back to /usr/local.
 
Now that the directory has been created and linked to the correct location, the Crouton installer will place all your chroots to a USB stick or SD card.
 
## Installing Crouton
 
Since you set up a symbolic link from your USB stick or SD card to the /usr/local directory, the Crouton installer will find and follow your link instead of making a chroot folder in the same location. Obviously, this will allow you to have a whole lot more space with your Crouton installation.
 
Note: this process will not work without your Chromebook set to developer mode. On your keyboard, hit Escape, Power and the Refresh. When this is done, your Chromebook will present a warning message, and you’ll need to press “Ctrl + D” every time before booting.
 
Enter the command below to install Crouton.
 
Once your Crouton installation has been completed, you can launch it by entering the commands below.
 
## Backup your Crouton Chroot
 
Having Crouton an SD card or USB device is very handy. Still, since it’s a removable device, you should probably have a backup. To perform the backup, enter the command below into the shell.
 
Note: remember, to get to the ChromeOS shell, press “Ctrl + Alt + T” on your keyboard, then type shell.
 
To backup your installation to your Downloads folder.
 
To restore your installation from the Downloads folder.
 
## Conclusion
 
I love Crouton. It makes Linux even more convenient since you can swap to it at any time. The ability to move installations to bigger storage devices just makes Crouton installs even more useful. I hope that with the help of this guide, you find it useful too.
 
Derrik Diener is a freelance technology blogger.
 
Our latest tutorials delivered straight to your inbox




