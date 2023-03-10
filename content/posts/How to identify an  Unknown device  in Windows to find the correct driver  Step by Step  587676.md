---
title: "Stop Searching for Drivers Blindly- The Ultimate Guide to Identifying Unknown Devices in Windows!"
ShowToc: true 
date: "2022-11-21"
author: "Richard Alcantar"
---
*****
# Stop Searching for Drivers Blindly- The Ultimate Guide to Identifying Unknown Devices in Windows!

If you have ever encountered the frustration of dealing with an unknown device in Windows, you know how time-consuming and challenging it can be to find and install the corresponding driver. Luckily, identifying unknown devices in Windows doesn’t have to be a daunting task. In this guide, we will walk you through the steps to identify and install drivers for unknown devices.

## Using Device Manager

Windows’ built-in Device Manager is the go-to tool for identifying unknown devices. Here is how to access it:

1. Press the Windows key + X and select Device Manager.
2. Look for any devices with a yellow exclamation mark (!) next to them. These devices indicate that the drivers are missing or outdated. 

To find the correct drivers, right-click on the device with the yellow exclamation mark and select Update Driver. Windows will attempt to find the correct driver automatically. If it cannot find the driver, you will need to search for and install it yourself.

## Using Hardware IDs

If Device Manager cannot find the correct driver, you can use Hardware IDs to identify the device and find the correct driver. Here is how to use Hardware IDs in Windows:

1. Right-click on the device with the yellow exclamation mark and select Properties.
2. Click on the Details tab.
3. Select Hardware Ids from the dropdown menu.

You will see a series of characters and numbers listed beneath the Hardware Ids field. This information is used to identify the device and find the correct driver.

Take the characters listed after “VEN_” and “DEV_” and enter them into Google or Bing. This will return search results with information on the device and links to download the driver.

## Using Third-Party Software

If you are not comfortable searching for drivers manually, there are several free third-party software options available to find and install drivers for unknown devices. Here are a few popular options:

- DriverPack Solution: This software automatically detects and installs drivers for all devices on your computer.
- Snappy Driver Installer: This software is a lightweight and portable tool that also automatically finds and installs drivers for unknown devices.
- Driver Easy: This software has a simple, user-friendly interface and a database of over 3 million drivers.

## Conclusion

Identifying and installing drivers for unknown devices in Windows doesn’t have to be a daunting task. By using Device Manager, Hardware IDs, or third-party software, you can quickly and easily find and install the correct driver for your device. Say goodbye to the frustration of searching for drivers blindly and hello to a smooth and efficient computing experience.

{{< youtube xsLJZyih3Ac >}} 



In this Windows How-to, you are going to learn how to identify the name of an “Unknown device” in Windows that is giving you trouble, that way you can properly find the correct driver.
 
How many times did you find the message “unknown device” in Windows Device Manger? Many times, right? And how hard is to find drivers for something that you don’t even know what it is? Yeah, you may have an idea, if you find an unknown device and the only thing that is not working is the sound in your computer, but this is not always the case.
 
There are a lot unknown device identifier software out there that could help in this situation, but I am not really a fan of installing a piece of software for every little thing that is going on in my computer, if there is a way to do it manually and it works, it is enough for me. Keep reading to learn more.
 
## Instructions
 
1.  Open Windows Device Manager by either going to the Control Panel or in Windows Vista or Windows 7 by going to Start and type device manager in the search box and press Enter. 
 
2.  Locate the unknown device, right-click on it and select Properties.
 

 
3.  Navigate to the Details tab and under Property select Hardware ids.
 
4.  Next, under Value right-click and copy either the four-part, three-part, or two-part device ID.
 
5.  Then open your favorite web browser do a search with the ID that you copied  — here I’ll recommend you to start with the four-part ID and work your way down until you can identify the device name.
 
Now just match the Device ID (PCI\VEN 8086…) with a device name (Intel(R) ICH9…) from the search result . For this Windows How-To article I am doing a search for known device on my lab computer, and if you see the first search result it has a pretty good guess of device name — see also the image in step 4 at the box title and you’ll see that both device name match –. Now the only thing left to do is to visit the device or computer manufacture, download and install the correct driver. 
 
As a personal note, you could keep investigating if you are not too sure by visiting some of the links in the search result and read more about the device, once you are sure and you know what to look for, do a search for the correct Windows device driver. Also this method that I am showing you today should work in Windows 7, Windows Vista, Windows XP, and pretty much most version of Windows.




