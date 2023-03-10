---
title: "Revolutionary Tutorial: Master the Art of Removable Device Management in KDE!"
ShowToc: true 
date: "2023-01-04"
author: "Peter Norman"
---
*****
Revolutionary Tutorial: Master the Art of Removable Device Management in KDE!

As the usage of removable devices such as USB drives and external hard disks increases, proper management of these devices is becoming more important. In the KDE desktop environment, managing removable devices has become much easier with the help of its user-friendly interface. In this tutorial, we will provide step-by-step instructions on how to effectively manage removable devices in KDE.

Step 1: Mounting devices

The first step in managing removable devices in KDE is to mount them. The KDE environment will automatically detect unmounted devices, and you can click on the device icon to mount it. Once the device is mounted, it will show up in the file manager.

Step 2: Unmounting devices

Before you remove a device, you first need to unmount it. This is important because if you remove a device without unmounting it first, you risk losing data or even damaging the device. To unmount a device, simply right-click on the device icon and select the “Unmount” option.

Step 3: Ejecting devices

Some devices such as CD/DVD drives require ejecting before they can be removed. To eject a device in KDE, right-click on the device icon and select the “Eject” option. This will eject the device and allow you to safely remove it from your computer.

Step 4: Configuring device policies

KDE also allows you to configure device policies, which lets you specify how each device should be handled. For example, you can choose whether to automatically mount a device or ask for your permission first. To configure device policies, go to the “System Settings” and select “Removable Devices”. Here, you can configure policies for various types of devices such as cameras, phones, and storage devices.

Step 5: Using the Device Notifier

The Device Notifier is a KDE application that displays a pop-up notification when a removable device is inserted or removed. You can use Device Notifier to manage devices directly from the pop-up notification. For example, if you want to unmount a device, you can do so by right-clicking on its notification and selecting the “Unmount” option.

In conclusion, managing removable devices in KDE has never been easier. By following these simple steps, you can effectively manage your removable devices and avoid the risk of data loss or damage to your devices. With the user-friendly interface and powerful tools available, KDE provides a revolutionary way to manage removable devices.

{{< youtube ACJ1suTVouw >}} 



As with most tasks in Linux, there are multiple ways to handle removable devices, but for removable media in particular, KDE’s primary tool is the Plasma Device Notifier Widget. It is activated by default on the KDE panel in all 4.x versions of the desktop environment. From it, you can manage all sorts of removable media, including hard drives, SD cards, USB flash drives, CDs, DVDs, cameras, and music players.
 
The Device Notifier Widget is located on the KDE panel, but may be anywhere on the panel, depending on the default setup of your Linux distribution. It can sit on the panel as an icon, like the application launcher, or reside within the system tray. To add it to the system tray:
 
1. Right click on the tray and click “System Tray Settings”
2. Click “Plasma Widgets”
3. Check “Device Notifier” and click “OK”.

 
### Connecting Once
 
For most removable media, you will only want it to connect on a per-use basis. Once a device is inserted or attached, the Device Notifier will popup over the system tray icon, showing you the device. If you do nothing, it will slip away after a few seconds.  At any time, you can click on the icon to see the devices again.
 
For every device, it will provide three pieces of information:
 
1. The type/size and name of device
2. The amount of available storage space
3. The number of available actions you can perform with the device.
 

 
To the right of the device information, you will see an icon that looks like a plug or connector. Clicking it will immediately mount it but will not perform any further actions. This is useful if you want it mounted but do not necessarily want to access it at the moment.
 
Click anywhere else on the device to bring up the actions menu. Some example actions are: “Download photos with…”, “Open with File Manager”, “Play Audio CD with Amarok”, and “Copy with K3b”.
 
Once you are finished using your removable device, you need to unmount it before removing it. First make sure you are not accessing it with any applications. Although KDE applications will communicate with each other and automatically detect an unmount, others may keep the device busy and prevent you from unmounting it. To proceed, click the up-arrow icon that looks like an eject button.
 
### Automatic Connections
 
If you find yourself connecting the same devices frequently, you may want to consider making them mount automatically. For example, I have an external 250GB hard drive that is always at my desk. When I login to KDE, I want it mounted already.
 
To access the Device Notifier settings, right click on the icon and click “Device Notifier Settings”
 
“General” options tell the widget to display removable, non-removable, or all devices. “Device Actions” is where you can add, edit, or delete actions associated with media and device types.
 
In order to configure automatic mounting, click on “Removable Devices”. At the top are general options that will apply to all devices. In order to automatically mount any devices, check the first box to enable auto-mounting. The sub-settings underneath it are optional but may be useful, depending on your situation.
 
In the box below those settings, you will see “Device Overrides“. This section allows you to setup automatic mounting for specific devices, such as my external hard drive. In the first tree, it will show currently attached devices, including internal drives and their partitions. Find your device, and check “Automount on login”, “Automount on attach”, or both options.
 
In the second tree, you will see “Disconnected Devices”. Device Notifier will remember all of the devices you have ever connected. Using this, you can configure devices you might not have at the moment, but it also can be a security risk if you do not want a device to be listed. To remove one, select it and then click the “Forget Device” button at the bottom. When you are finished configuring, click “OK”.
 
### Other Places to manage devices
 
KDE applications are smart and will be aware of devices as they appear. They also allow various degrees of device management, depending on the application. These applications include:
 
- Dolphin (mount/unmount; show/hide from “Places”)
 - Kickoff and Lancelot menus (mount/unmount)
 - Other apps, such as Amarok and Digikam (mount/unmount; retrieve data)

 
KDE’s device management system is designed to provide ease of use while still offering flexibility and a variety of options. With it, you should rarely, if ever, need to drop to the command line to manage a removable device.
 
Tavis J. Hampton is a  freelance writer from Indianapolis.  He is an avid user of free and open source software and strongly believes that software and knowledge should be free and accessible to all people. He enjoys reading, writing, teaching, spending time with his family, and playing with gadgets.
 
Our latest tutorials delivered straight to your inbox




