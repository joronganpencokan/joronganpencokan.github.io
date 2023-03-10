---
title: "You won't believe the hidden settings in Windows 10 Control Panel!"
ShowToc: true 
date: "2023-03-19"
author: "Juan Kidd"
---
*****
# You won't believe the hidden settings in Windows 10 Control Panel!

Windows 10 has been the go-to operating system for many years now. It is the most widely used OS in the world and has many features that make it stand out. While users may be familiar with the Control Panel and its basic functions, many aren't aware of the hidden settings that lie within.

In this article, we will explore some of the hidden settings in Windows 10 Control Panel that you may not know about.

## Advanced Power Settings

If you're someone who frequently uses their laptop and wants to maximize battery life, the Advanced Power Settings option in the Control Panel can help. This option allows you to customize power settings beyond the basic ones available in the Power Plan settings. 

By selecting "Advanced Power Settings," you have access to options like USB selective suspend, processor power management, and adaptive display. By changing these settings, you can cut down on battery usage and prolong your device's life.

## Device Manager

Did you know that the Device Manager in Control Panel can display hidden devices? This is helpful if you're trying to troubleshoot a hardware issue or uninstall a stubborn driver. 

To access this setting, open the Device Manager, click on the View menu, and select the option to show hidden devices. This will display a list of all devices, including those that are not currently connected to your computer or might have been disabled in the past.

## God Mode

Yes, you read that right. God Mode is a hidden feature within the Windows 10 Control Panel that gives users access to an overwhelming number of settings and options. 

To enable God Mode, create a new folder on your desktop and name it "GodMode.{ED7BA470-8E54-465E-825C-99712043E01C}". Once you open the folder, you will have access to over 200 customizable settings that are usually hard to access.

## Storage Spaces

Another hidden setting in Windows 10 Control Panel is Storage Spaces. It is a feature that allows users to create one large pool of storage from multiple drives connected to their computer. 

By using Storage Spaces, users can create a virtual drive that functions as a single storage location for all files. With this feature, users can utilize multiple drives without the need for third-party software or hardware.

## Summary

While the Windows 10 Control Panel may seem simple on the surface, it has many hidden settings that can improve your computer's performance and overall experience. The Advanced Power Settings option, the Device Manager's ability to show hidden devices, God Mode, and Storage Spaces are just a few examples of these settings.

Take some time to explore the Control Panel and see what other hidden settings you can find. Who knows what other useful features you could be missing out on!

{{< youtube E4arEKkEsuQ >}} 



Hide Items from Control Panel in Windows 10: Control Panel is one of the most important components of Windows, which gives the ability to the user to change System Settings. But with the introduction of Windows 10, Settings app is created to replace the classic Control Panel in Windows. Although Control Panel is still present in the system with a lot of a number of options which still isn’t available in the Settings app, but if you share your PC with your friends or use your PC in public then you might want to hide specific applets in Control Panel.
 

 
The Classic Control Panel is still used by many users over the Settings app and have options like Administrative tools, system backups, system security and maintenance etc which are not present in the Settings app. So without wasting any time let’s see How to Hide Items from Control Panel in Windows 10 with the help of the below-listed tutorial.
 
## Hide Items from Control Panel in Windows 10
 
Make sure to create a restore point just in case something goes wrong.
 
Contents
 
- Hide Items from Control Panel in Windows 10
 - Method 1: Hide Items from Control Panel in Windows 10 Using Registry Editor
 - Method 2: Hide Items from Control Panel in Windows 10 Using Group Policy Editor

 
#### Method 1: Hide Items from Control Panel in Windows 10 Using Registry Editor
 
Registry Editor is a powerful tool and any accidental click can damage your system or even make it inoperable. As long as you follow the below-listed steps carefully, you shouldn’t have any problem. But before doing that make sure to create a backup of your registry just in case, something goes wrong.
 
Note: If you have Windows Pro or Enterprise Edition then you can simply skip this method and follow the next one.
 
1.Press Windows Key + R then type regedit and hit Enter.
 
2.Navigate to the following Registry Key:
 
HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\Explorer
 
3.Now if you see Explorer then you’re good to go but if you don’t then you need to create it. Right-click on Policies then click New > Key and name this key as Explorer.
 
4.Again right-click on Explorer then select New > DWORD (32-bit) Value. Name this newly created DWORD as DisallowCPL.
 
5.Double-click on DisallowCPL DWORD and change it’s value to 1 then click OK.
 
Note: To Turn off hiding the Control Panel items simply change the value of DisallowCPL DWORD to 0 again.
 
6.Similarly, right-click on Explorer then select New > Key. Name this new key as DisallowCPL.
 
7.Next, make sure you are under the following location:
 
KEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer\DisallowCPL
 
8.Select DisallowCPL key then right-click on it and select New > String Value.
 
9.Name this String as 1 and hit Enter. Double-click on this string and under Value data field change it’s value to the name of the specific item you want to hide in Control Panel.
 
For example: Under the value data field, you can use any one of the following: NVIDIA Control Panel, Syn Center, Action Center, Administrative Tools. Make sure you enter the same name as its icon in the Control Panel (icons view).
 
10.Repeat the steps 8 and 9 above for any other Control Panel items you want to hide. Just make sure that every time you add a new string in step 9, you increase the number you use as the value’s name e.g. 1,2,3,4, etc.
 
11.Close Registry Editor and reboot your PC to save changes.
 
12.After the restart, you would be successfully able to Hide Items from Control Panel in Windows 10.
 
Note: Administrative Tools and Color Management is hidden in Control Panel.
 
#### Method 2: Hide Items from Control Panel in Windows 10 Using Group Policy Editor
 
Note: This method will only work for Windows 10 Pro and Enterprise Edition users, but be careful as it gpedit.msc is a very powerful tool.
 
1.Press Windows Key + R then type gpedit.msc and hit Enter.
 
2.Navigate to the following location:
 
User Configuration > Administrative Templates > Control Panel
 
3.Make sure to select Control Panel then in right window pane double-click on “Hide specified Control Panel items” policy.
 
4.Select Enabled and then click on Show button under Options.
 
Note: If you want to turn off hiding items in Control Panel then simply set the above settings to Not Configured or Disabled then click OK.
 
5.Now under Value, enter the name of any Control Panel items you want to hide. Just make sure to enter one item per line you want to hide.
 
Note: Enter the same name as its icon in the Control Panel (icons view).
 
6.Click OK then click Apply followed by OK.
 
7.When finished close gpedit.msc window and reboot your PC to save changes.
 
Recommended:
 
- Create Control Panel All Tasks Shortcut in Windows 10
 - Fix Context Menu Items Missing when more than 15 Files are Selected
 - Enable or Disable Control Panel and Windows 10 Settings App
 - Enable or Disable Shared Experiences Feature in Windows 10

 
That’s it you have successfully learned How to Hide Items from Control Panel in Windows 10 but if you still have any queries regarding this tutorial then feel free to ask them in the comment’s section.




