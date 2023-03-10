---
title: "Unlock Your Data Now: Get Rid of Write Protection from USB or SD Card with Simple Techniques!"
ShowToc: true 
date: "2023-01-22"
author: "Christine Young"
---
*****
Introduction

Nowadays, storing data on USB or SD Cards has become a common practice. These portable storages are widely used for transferring files between devices, and even for backing up important data. However, sometimes we run into an issue where our USB or SD Card gets write-protected. This can be quite frustrating, especially when we need to make changes or update the files on the storage device. In this article, you will learn how to get rid of write protection from USB or SD Card with simple techniques.

What is Write Protection?

Write protection is a feature that restricts users from making changes or updating files on a storage device. When a USB or SD Card is write-protected, you can read files from the device, but you cannot write or delete them. This feature is usually enabled to prevent users from accidentally deleting important files or corrupting the data on the storage device.

How to Remove Write Protection on USB or SD Card

There are several methods to remove write protection on USB or SD Card. Here are some simple techniques that you can try:

Method 1: Check the Lock Switch

Most USB or SD Cards have a lock switch that users can turn on/off to enable/disable write protection. This switch is usually located on the side of the storage device. Check to see if the switch is in the locked position. If it is, simply move the switch to the unlocked position to remove write protection.

Method 2: Modify Registry Settings

If the lock switch is not the issue, you can modify the registry settings on your computer to remove write protection. Here is how you can do it:

- Press Windows + R to open the Run dialog box.
- Type in "regedit" and hit Enter to launch the Registry Editor.
- Navigate to "HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\StorageDevicePolicies".
- If "WriteProtect" is set to 1, double-click on it to change the value to 0.
- Close the Registry Editor and restart your computer.

Method 3: Use Diskpart Command

Diskpart is a Windows utility that allows users to manage drives, partitions, and volumes on their computer. Here is how you can use Diskpart to remove write protection:

- Press Windows + R to open the Run dialog box.
- Type in "cmd" and hit Enter to launch the Command Prompt.
- Type in "diskpart" and hit Enter to launch Diskpart.
- Type in "list disk" to display a list of all the storage devices connected to your computer.
- Identify the disk number associated with your USB or SD Card.
- Type in "select disk x" (replace "x" with the disk number associated with your storage device).
- Type in "attributes disk clear readonly".
- Type in "exit" to close Diskpart.

Conclusion

In conclusion, write protection on USB or SD Card can be quite frustrating, but it can be easily fixed with the above techniques. You can try these methods to remove write protection from your storage device and update or make changes to your files without any restrictions. Always remember to backup your data before attempting to remove write protection, to avoid any data loss.

{{< youtube BKr6f7U_CVs >}} 



## Remove Write Protection From Your USB Or SD Card


There are many ways to remove write protection from your USB or SD Card. So, in this article, we are going to share a few best methods to remove write protection from your USB drive or SD card in 2020.

 
### 1. Check Device For Virus



Sometimes, viruses and malware trigger the write protection on USB drives or SD cards. This thing is done to restrict users from removing the virus filled files or software. So, if you haven’t enabled the write protection on your PenDrive, then you need to scan it with an Antivirus. For a complete list of the best antivirus, check out this article Best Antivirus For PC.

 
### 2. Check the Write Protection Button



Many USB devices come with a write protection button. If this button is turned on, then you can’t copy, paste, or delete the data stored on the device. Simply, turn off the write protection switch to remove the write protection from the USB drive.

 
### 3. Ensure The USB Drive Isn’t Full


USB flash drive often shows Write protect error due to insufficient storage. To check out if your drive is full or not, open Windows Explorer and right-click on your USB drive and select “Properties”.

The properties section will show you the File system along with Storage capacity. If your disk space is full, you need to remove some files to avoid the Write Protect error.

 
### 4. Check For Individual Files


Mostly the write protect error occurs because of a single file that is marked as “read-only”. That single file can upset you. If any of your files are set to read-only mode, then you can’t just delete that file. On return, the single file can deny a full format.

Locate the file that is undeletable and then right-clicks on it and select ‘Properties’. At the bottom of the panel, under attributes, you will find the Read-only option, make sure to uncheck the “Read Only” box.

 
### 5. Using the Command Prompt


In this method, we will remove write protection from Pendrive using commands in Cmd. This will fully remove the write protection of the Pendrive.
Step 1. Click on Start->Cmd. Type Diskpart and press enter.

Step 2. Type list disk.

Step 3. Type select disk 1 and this will select your Sdcard/USB Pendrive.

Step 4. Now type “attributes disk clear readonly” and press enter.

Now exit from cmd and format your Sdcard/USB Pendrive. This will remove write protection from your SD card or Pendrive.

 
#### Video Tutorial:




 
### 6. Using Registry Editor


In this method, we will edit some registry values of computer as when they are overwritten by some reason, our media can show an error message of Write Protection
Step 1. Open the RUN dialog box. On the RUN dialog box, enter ‘Regedit’ and click on ‘Ok’

Step 2. Now follow up this path in Registry Editor
Step 3. There you will find the write protection option just click on it and set its value to 0.

That’s it! you are done. By this, the default value of the write protection register will be changed and the write protection will permanently get removed from that media device.

 
#### What If You didn’t Find StorageDevicePolicies?


If you can’t find StorageDevicePolicies in Registry Editor then you can create a key For that you need to head over Registry Editor and follow this path
 

Here you need to right-click on the white space in the control folder and choose New>Key and carefully enter the name “StorageDevicePolicies”

Now double click on the newly created folder and right-click and then choose New>DWORD and name it WriteProtect and set its value to 0. Click OK, exit Regedit and make sure to restart your computer.

 
### 7. Turn Off Bitlocker Partition in Windows


Well, if you have enabled the BitLocker encryption on your hard drive partition, then you will get write protection errors. So, in this method, you need to turn off the BitLocker partition in Windows to remove Write protection from USB or SD Card. Follow, some of the simple steps given below to turn off BitLocker Partition in Windows 10.
Step 1. First of all, open My Computer and then right-click on any of the storage devices and select the option ‘Manage BitLocker’

Step 2. Now on the BitLocker Drive Encryption page, you need to turn off the BitLocker for the USB or SD Card.

Step 3. Now you need to wait for few minutes until Bitlocker decrypts your storage device.

Step 4. Once done, you will see a screen like below. If it shows ‘BitLocker off’ then you have successfully decrypted the drive.

That’s it, you are done! This is how you can turn off BitLocker partition to remove write protection from your USB or SD Cards.
So, these are the best methods to remove write protection from USB. I hope this article helped you! Please share it with your friends also.





