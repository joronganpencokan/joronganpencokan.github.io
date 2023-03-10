---
title: "Unlock the Secret to Lightning-Fast Boot Times with This Game-Changing BIOS to UEFI Conversion Tutorial!"
ShowToc: true 
date: "2022-12-20"
author: "Kathleen Seal"
---
*****
Title: Unlock the Secret to Lightning-Fast Boot Times with This Game-Changing BIOS to UEFI Conversion Tutorial!

Introduction:
Have you ever found the time-consuming process of booting up your computer frustrating? You are not alone. It used to be a tedious process that took up a significant chunk of your day. However, with the advent of UEFI (Unified Extensible Firmware Interface) technology, booting up your PC is now a breeze! This game-changing technology drastically reduces boot times, making your computer start up lightning fast. In this article, we will explore how you can convert your BIOS system to UEFI and unlock the benefits of this revolutionary technology.

Section 1: Understanding the Difference between BIOS and UEFI
Before we dive into the steps of converting a BIOS system to UEFI, it is essential to understand the difference between the two. BIOS (Basic Input/Output System) is a firmware used by older systems to boot up a computer. This system was replaced by UEFI, which offers more advanced and modern features. UEFI allows for more security features, faster booting speeds, and larger boot partitions. Compared to BIOS, UEFI is more intuitive, allowing for easier setup and configuration.

Section 2: Benefits of Converting to UEFI
UEFI not only offers significantly faster boot times but also features an extensive list of benefits. It allows for bootable devices up to 9,999 GB in size, whereas BIOS can only boot systems with a partition of up to 2 TB. UEFI also allows for more advanced performance features such as power management and fan control. Additionally, it supports modern peripherals and built-in networking.

Section 3: How to Convert Your BIOS System to UEFI
Converting your BIOS system to UEFI can seem daunting, but it is an easy process. To get started, follow these simple steps:

1. Identify whether your computer is compatible: You can check by running the command "msinfo32.exe" in the search bar of your Windows PC.

2. Create a bootable USB with a Windows installation media, such as the Windows 10 installation file.

3. Boot your system with the USB drive plugged in and access the BIOS settings.

4. Locate the "Secure Boot" option and disable it.

5. Find the option to switch the boot mode from BIOS to UEFI. This setting is usually under "Boot mode," "Boot option," or "System configuration."

6. Save the changes and reboot the system.

7. Windows will automatically install the UEFI drivers and update the boot partition.

Section 4: Conclusion
In conclusion, converting your BIOS system to UEFI is an easy process that can improve your computer's performance and speed. With the benefits of UEFI, your computer will boot faster, offer more storage, and provide advanced features such as power management and networking. By following the simple steps above, you can unlock the secret to lightning-fast boot times and take advantage of this game-changing technology. So, what are you waiting for? Convert your BIOS system to UEFI today!

{{< youtube 0aRUXQz5ygc >}} 



In older versions of Windows, you were forced to reinstall the entire operating system if you wanted to convert legacy BIOS or Master Boot Record (MBR) to UEFI or GUID Partition Table (GPT). However, a new and simple tool called MBR2GPT was introduced in Windows 10. It lets you convert legacy BIOS to UEFI with just two commands. 
 
Here is how you can convert legacy BIOS to UEFI in Windows 10. If you’re a Windows 11 user, you shouldn’t do anything, as UEFI mode is enabled by default on your device.
 
Do not skip any of the prerequisites of legacy BIOS to UEFI conversion mentioned below, as it can lead to system failure and even hardware issues in some cases.
 
## Why Convert Legacy BIOS to UEFI?
 
You probably have some inkling why you’d want to change from the legacy BIOS to UEFI, but just to confirm, here’s what you need to know. Both BIOS and UEFI perform the same function on your PC – namely under-the-hood software integrated into your motherboard chip that lets you control various important low-level things.
 
Your BIOS/UEFI lets you control things like boot order, connected hardware, fan speeds, the physical lights on your computer and system time. Modern motherboards even let you undervolt and overclock your CPU! It’s powerful stuff.
 
UEFI is basically the new BIOS, performing the same job but better. With UEFI, you get faster boot times (ostensibly), higher drive capacities, better update methods and driver support, and a 64-bit mode (where BIOS is only 16-bit). 
 
In other words, switching to UEFI is a bit of an upgrade and worth doing. Note that even modern computers (including Windows 11) tend to still call the motherboard software the BIOS, even if it’s technically UEFI.
 
## Prerequisites for Legacy BIOS to UEFI Conversion
 
- While there will be no data loss while converting legacy BIOS to UEFI, please back up your system as a precaution.Always verify whether your Windows system is capable of supporting UEFI in the first place. Generally, all motherboards launched after 2014 are UEFI secure boot capable but that’s not always the case. So you should verify the eligibility for your device specifically.

 
To do so, use the Run command with the shortcut Win + R and type msinfo32 to launch the System Information window. In its right-hand side panel, check your BIOS Version/Date. If it says UEFI, your device is eligible for legacy BIOS to UEFI conversion. However, if it only gives the name of your BIOS version, the device does not have UEFI firmware settings. Trying to convert the legacy BIOS will lead to hardware failures.
 
- You should be using Windows 10 v1703 or higher. If you are not sure, press Win + R, type winver and press Enter. On the second line, you should see “version 1703” or higher.

 
- The disk you are trying to convert should not have more than three partitions. If you have more than three partitions on the Windows 10 installation drive, either merge or delete the excess partitions. Otherwise, you’ll encounter a “Disk Layout Validation Failed” error, which is fixable but best avoided.If you are using BitLocker to encrypt your system, decrypt the drive and disable BitLocker protection before starting the conversion process. With BitLocker protection turned on, Windows 10 cannot convert your drive from legacy BIOS to UEFI.After converting, you may have to change your motherboard firmware settings from legacy BIOS to UEFI. Depending on your motherboard manufacturer, the procedure to switch from one to the other will be different. Have your motherboard manual handy to make things easier for you.Don’t proceed with the legacy BIOS to UEFI conversion if your Windows device is already on UEFI with secure boot enabled. We’ll show you how to check for this below.

 
If you want to know more, we have a full guide on the differences between UEFI and BIOS.
 
## Do I Need to Convert Legacy BIOS to UEFI in Windows 11?
 
If you’re using Windows 11, it means your device is past the milestone in switching from legacy BIOS to UEFI. This is because migrating to a UEFI secure boot is a mandatory Windows 11 compatibility requirement. There is no separate provisioning of legacy BIOS in Windows 11. 
 
In rather simple words, Windows 11 doesn’t support legacy BIOS at all. If you want to install Windows 11 on an older Windows 10 device, you should first check whether that computer supports UEFI mode or not, and it should have a GPT partition, not MBR (check the following section for more details on this). 
 
You can check this from a “Windows Security” option where “Secure boot” is displayed as On. Microsoft recommends you keep it that way to deter any malicious software from loading when the device is booting. 
 
The secure boot settings can also be verified from the BIOS options (called UEFI Firmware Settings) accessible in Windows 11 “Advanced startup.” After the BIOS screen shows up, navigate to the Boot Options tab. According to Microsoft, UEFI should be shown as the “first or only option.” This is especially true for Dell, HP, and Lenovo laptops. However, some other manufacturers may have continued to retain both UEFI and legacy/CSM. 
 
## How to Check Whether You Are Using Legacy BIOS
 
Before you switch from legacy BIOS to UEFI in Windows 10, check whether you are actually using legacy BIOS. After all, there is no use converting if you are already on UEFI.
 
- Search for “Create and format hard disk partitions” in the Start menu and press Enter to open the built-in Disk Management tool.Right-click on the Windows installation disk, Disk 0, and select “Properties.”

 
- In the Properties Window, go to the “Volumes” tab. If you see “Master Boot Record (MBR)” next to “Partition style,” you are on Legacy BIOS. If, on the other hand, it says “GUID Partition Table (GPT)” as in the image below, then you’re already on UEFI and don’t need to do anything more!

 
## How to Convert Legacy BIOS to UEFI
 
Once you’ve confirmed you are on legacy BIOS and have backed up your system, you can convert Legacy BIOS to UEFI.
 
- Access Command Prompt from Windows’s advanced startup by pressing Win + X.Go to “Shut down or sign out” and click on the “Restart” button while holding the Shift key.

 
- The above action will reboot your system to the Advanced Startup screen. Go to “Troubleshoot -> Advanced Options” and select the option “Command Prompt.”

 
- Validate the disk you are trying to convert. Type the below command and press Enter.

 
If you see the “Validation completed successfully” message, proceed to the next step. If you see any errors, your disk or system may not meet the conversion requirements.
 
If you have problems validating at this point, enter the following command. We highly recommend you use this add-on code to not lose data.
 
- After validating the disk, execute the below command:

 
As soon as you execute, Windows 10 will start the conversion process, i.e., add all the required UEFI boot files and GPT components, then update the Boot Configuration Data.
 
- Restart your system, launch your motherboard firmware settings screen and change it from legacy BIOS to UEFI. The procedure to change from Legacy BIOS to UEFI depends on your motherboard manufacturer. Consult the manual for the exact steps.After booting into Windows 10, you can verify whether or not you are converted. Just as before, open the disk properties window from the Disk Management tool and go to the “Volumes” tab. Here, you should see “GUID Partition Table (GPT)” next to “Partition style.”

 
## How to Fix the MBR2GPT “Disk Layout Validation Failed” Error
 
While changing your hard drive from MBR to GPT, you may sometimes receive the error message: “MBR2GPT Disk layout validation failed for Disk#,” with the number # referring to your boot disk.
 
There are two reasons for this error: more than three partitions and no available space in C drive, the boot disk.
 
- To solve the “Disk Layout Validation Failed” error, go to “Create and format hard disk partitions” from the search menu and check whether you have more than three partitions in the boot disk, Disk 0. You need to “merge and delete” some of these extra partition volumes to bring down the number of partitions to three or less. Do create a backup of any important data in the extra partitions.

 
- The second reason for the error is the Disk 0 drive not having enough space for an MBR to GPT conversion. To resolve this, you need to shrink its volume to anything between 200 MB to 2 GB.

 
Note: if your device is already on a GPT layout, these options will be greyed out.
 
## Frequently Asked Questions
 
Image Credit: Unsplash
 
### Why am I seeing a black screen after changing legacy BIOS to UEFI?
 
If you’re seeing a black screen after changing over from legacy BIOS to UEFI, it means you did not complete one or more prerequisites we have listed above.
 
Having a black screen after restart may or may not indicate hardware failure. If your Windows device is healthy, you should be able to access its “safe mode” by pressing the Power button followed by what is known as a “Boot key.” Common boot keys include F2, F6, F12, Del, and Esc. They vary among laptop/PC manufacturers and you should check your precise laptop/PC model to know its boot key. 
 
Once the Safe mode menu items are visible, attempt a factory image restore of your Windows computer. This will revert your Windows device to the exact configuration in which it was shipped by the manufacturer. You can also try a simpler System Restore if it works for you. 
 
If you cannot access the Safe mode using Power button and boot keys, it definitely indicates hardware failure. This leaves you no other choice but to have the device repaired by a competent PC hardware expert.
 
### How do I resolve the "0x514; MBR2GPT failed to enable backup/restore privileges" error on Windows 10?
 
Some users have experienced an “administrator not found on the system” error while performing the MBR to GPT conversion on a command prompt even though they were signed into the computer as administrator. To deal with this problem, ensure that you are running the elevated Command Prompt which is the Administrator mode. It can be easily accessed from the Start menu.
 
### Can I go back to legacy BIOS from UEFI? 
 
If you had your Windows 10/11 OS installed in UEFI mode, it is possible to go back to legacy BIOS (although we’ll highly recommend not doing this). You have to initiate an “advanced startup” on your Windows device and enter the UEFI Firmware settings to disable the UEFI secure mode which can be reenabled later.
 
Sayak Boral is a technology writer with over eleven years of experience working in different industries including semiconductors, IoT, enterprise IT, telecommunications OSS/BSS, and network security.  He has been writing for MakeTechEasier on a wide range of technical topics including Windows, Android, Internet, Hardware Guides, Browsers, Software Tools, and Product Reviews.
 
Our latest tutorials delivered straight to your inbox




