---
title: "You Won't Believe How Easy It Is To Use Your iPhone As An External Drive In Ubuntu!"
ShowToc: true 
date: "2023-06-27"
author: "Robert Dresbach"
---
*****
# You Won't Believe How Easy It Is To Use Your iPhone As An External Drive In Ubuntu!

If you have ever tried accessing files on your iPhone from a Ubuntu machine, you might have found it quite challenging. This is because Apple makes it quite difficult to use their devices outside of their ecosystem. In this article, we will be discussing how to use an iPhone as an external drive in Ubuntu.

First, you need to ensure that your iPhone is connected to your Ubuntu machine. Make sure that your iPhone is unlocked, and the Trust This Computer prompt shows up. Choose Trust, and your iPhone should be recognized by your Ubuntu system.

To access your iPhone from your Ubuntu machine, you will need to install a utility called libimobiledevice. This is a collection of software that allows communication with Apple devices through USB.

To install libimobiledevice, open up a terminal window and type the following command:

```
sudo apt-get install libimobiledevice-utils
```

This will prompt you for your password, and then proceed to download and install the necessary software.

Once libimobiledevice is installed, we can check whether your iPhone is recognized by your Ubuntu machine. To do this, open up a terminal window and type the following command:

```
ideviceinfo
```

This will output a list of information about your iPhone, including its name, serial number, and iOS version. If this command doesn't return any data, make sure that your iPhone is connected properly and unlocked.

Now that we have confirmed that your iPhone is recognized by your Ubuntu machine, we can move to the next step. We need to mount your iPhone as an external drive to access its files.

To do this, we will use a tool called ifuse. This software allows us to mount the iPhone as a file system on the Ubuntu machine.

To install ifuse, open up a terminal window and type the following command:

```
sudo apt-get install ifuse
```

With ifuse installed, we can now mount your iPhone's file system in Ubuntu. To do this, type the following command:

```
ifuse ~/iphone
```

This command mounts your iPhone's file system in the ~/iphone directory in your home folder. You can change this directory to any other location that you prefer.

Now that your iPhone is mounted as an external drive in Ubuntu, you can access its files just like you would with any other external drive. You can copy, paste, and delete files from your iPhone using the file manager or commands in the terminal.

To unmount your iPhone from your Ubuntu machine, type the following command:

```
fusermount -u ~/iphone
```

This will unmount your iPhone, and it will no longer be accessible from your Ubuntu machine.

In conclusion, using an iPhone as an external drive in Ubuntu is quite easy. All you need is to install the necessary software, and you're good to go. With this method, you can access your iPhone's files from your Ubuntu machine without any hassle. Give it a try, and you'll be surprised at how seamless it is.

{{< youtube d4ghirmM1Ys >}} 



Using an iPhone as an external Ubuntu drive used to be tricky. Linux support for iOS devices like the iPhone, iPad, and iPod used to be pretty poor, but that situation has changed. Here’s how to mount your iPhone (and iPad) storage on Ubuntu and other Linux distributions using the libimobiledevice library. 
 
## Installing libimobiledevice
 
For iPhone and other iOS devices to be recognized on Ubuntu, you’ll need to install the libimobiledevice library first. This allows Ubuntu and other Linux operating systems to interact with these iOS devices.
 
This is important, especially due to Apple’s security measures. Libimobiledevice lets you access system information for your device as well as the internal storage. The libimobiledevice website has a list of currently-included features as well as features planned for the future.
 
If you want to use your iPhone as an external drive, you’ll need to install libimobildevice first.
 
You don’t need to add any additional package repositories to install libimobiledevice. Open a terminal window and type:
 
Once libimobiledevice has installed, try to connect your iPhone. If your iPhone file system doesn’t mount automatically when connected, you may need to pair your iPhone. Open a terminal and type:
 
A success message should appear after running this. Then, run the following:
 
This allows for multiple connections between your iPhone and your Ubuntu installation.
 
After running all of these commands, if you still can’t connect to your iPhone, you’ll need to install and use a second package called iFuse to mount your iPhone manually.
 
## Installing iFuse
 
The iFuse package allows you to mount an iPhone and access its file system in Linux. It’s likely that iFuse will install itself along with libimobiledevice, but if it hasn’t, you’ll need to install it manually.
 
Like libimobiledevice, you should find iFuse in the usual Ubuntu package repositories.
 
To install it, open your terminal and type:
 
This will install iFuse and any additional packages it may need on your Ubuntu installation.
 
## Accessing Your iPhone Storage
 
If you have Ubuntu with the GNOME desktop environment, then your iPhone file system should mount automatically once you plug it in. Reboot your PC if, in the first instance, your device doesn’t mount automatically. You should also unlock your iPhone device screen. If you don’t, you won’t be able to access the internal storage.
 
If that doesn’t work, you may need to mount your iPhone manually. You may also need to do this if you don’t use the standard Ubuntu installation with GNOME.
 
First, pair your iPhone by opening a Linux terminal and typing:
 
You should see a success message appear after running this command, or idevicepair will inform you it can’t find your iOS device.
 
If that’s the case, restart and try it again. Once your device is paired, type the following to mount your iPhone:
 
Replace the “/media/iphone” directory with another directory of your choice. This is where your iPhone files and folders will be seen on your device.
 
Once mounted, you should then be able to see your iPhone file system in your chosen file manager. You can then remove or add files to the iPhone as an external drive.
 
If you mounted your device manually and want to safely unmount it, open your terminal again and type:
 
This will safely unmount your iPhone storage. Once done, you can then unplug it from your Ubuntu PC or laptop.
 
## Frequently Asked Questions
 
### 1. Do I need to jailbreak my iPhone to mount it in Ubuntu? 
 
No. This should work on your iPhone either way. Jailbreaking your device does void the warranty. However, you’re free to jailbreak it if you want more control over the device. The method above doesn’t require it though.
 
### 2. Which iOS versions does libimobiledevice support?
 
The great thing about libimobiledevice is it’s designed to be compatible with 1.x series devices through current devices. Even if a new iOS version is released, everything should still work correctly.
 
### 3. My iPhone just upgraded to a new iOS version. Why isn’t libimobiledevice working?
 
New firmware releases have been known to cause rare glitches. These are typically addressed by the community to provide a more stable release of libimobiledevice. Check to see whether there is a new version available. It may take a few weeks after an iOS release for all glitches to be addressed.
 
### 4. Does this allow me to sync my music?
 
Currently, music sync isn’t supported on newer iPhones. However, some community members are working on allowing seamless music syncing. You’ll need to use alternative methods, such as VirtualBox, for this to work at the moment.
 
### 5. Will this hurt apps installed on my device?
 
No. The only issue you may face is running out of storage. If you’re an app collector, you may need to remove apps in order to make room for your Linux files. Pay close attention to your remaining storage capacity to ensure you always have room for the apps you want along with necessary updates.
 
### 6.Why isn’t anything working?
 
It’s possible that the process didn’t quite work correctly. To ensure your device is recognized, open a terminal and run:
 
As long as you see details about your device, Linux does recognize your iPhone. If you don’t get any details, try the process again. As simple as it sounds, restarting Linux may also help. 
 
### 7. Is it worth using my iPhone as an external device for extra storage?
 
Ideally, you’d want to use your iPhone for emergency storage or just transferring files. Since this isn’t the simplest process, you may want to consider using a different type of device, such as USB or external hard drives. You could even use cloud storage. 
 
## Using Your iPhone for Storage on Linux
 
With storage capacity from 16GB to 512GB, the iPhone makes for a good external drive for your Linux PC. If you’re not filling your device with apps, photos, and videos, it makes sense to put the excess storage to good use. Or, if you just have an older iPhone you’re not using, this is a great way to recycle it.
 
If you’re running out of space, you may need to look at freeing up storage on your iPhone first. You might find it easier to use an Android device for your external storage, however.
 
Crystal Crowder has spent over 15 years working in the tech industry, first as an IT technician and then as a writer.  She works to help teach others how to get the most from their devices, systems, and apps. She stays on top of the latest trends and is always finding solutions to common tech problems.
 
Our latest tutorials delivered straight to your inbox




