---
title: "Revamp Your Browsing Experience: Learn How to Reset Microsoft Edge Like a Pro!"
ShowToc: true 
date: "2022-11-25"
author: "Mark Lawrence"
---
*****
# Revamp Your Browsing Experience: Learn How to Reset Microsoft Edge Like a Pro!

Microsoft Edge is one of the most widely used web browsers today, and for good reasons. It's fast, stable, and packed with useful features that enhance your browsing experience. However, like any other software, Edge also has its occasional glitches and bugs that could slow down your browsing or hinder your productivity. And when this happens, resetting the browser often comes as necessary.

Resetting Edge can solve a myriad of issues, such as freezing, crashing, or slow performance. It also clears cookies, cache, and browsing history, giving you a fresh start to your browsing journey. So if you're experiencing any problems with your Edge browser, don't worry. In this article, we'll show you how to reset Microsoft Edge like a pro in just a few easy steps.

## Step One: Open Your Edge Browser Settings

To get started, you need to access your Edge browser settings. Launch your Edge browser and click on the three dots located at the top right corner of the window. This action opens a drop-down menu with several options. Click on "Settings" from the list, and a new settings window will open.

## Step Two: Go to Reset Settings

Once you're in the settings window, scroll to the bottom and look for the "Reset settings" option. This feature is located under the "Profiles" section. Click on the "Reset settings" button, and a prompt window will appear.

## Step Three: Confirm the Reset Process

The prompt window gives you two reset options: "Restore settings to their default values" or "Restore settings to their original defaults." To reset Microsoft Edge like a pro, you should choose "Restore settings to their default values."

When you click on this option, it will restore your browser's main settings, such as home page, search engine, security settings, and saved info. Note that this option does not delete your browser data, such as bookmarks and passwords. However, it will clear your cookies, cache, and browsing history, so you need to log in to your favorite sites again.

Finally, click on the "Reset" button to confirm the reset process. Your browser will then restart automatically, taking you to the default new tab page. You can now start browsing with a fresh browser instance and optimized settings.

## Conclusion

Resetting Microsoft Edge is a quick and effective way to fix common browser issues and restore its performance. By following these simple steps, you can reset your Edge browser like a pro and enjoy fast and smooth browsing. Remember to save your essential data before resetting your browser and keep your browser up-to-date with the latest versions to avoid future glitches.

{{< youtube XuJGXGJfuo0 >}} 



With Windows 10 Microsoft introduced it’s latest browser Microsoft Edge, which replaces its traditional browser Internet Explorer, although IE is still present in Windows 10 not as a default browser. Although Microsoft Edge is the latest browser which promises security and fast browsing, it could still break and lead to a crash and what not. Although Edge is a protected Windows 10 app, you can’t uninstall or remove it from Windows, and it is very unlikely that it could get compromised.
 

 
The only option you have is to reset edge in Windows 10 if something goes wrong with it. Unlike, how you can reset Internet Explorer there is no direct way to reset Microsoft Edge to default, but we still have some way to accomplish this task. So without wasting any time let’s see How to Reset Microsoft Edge to Default Settings in Windows 10 with the help of the below-listed guide.
 
## [GUIDE] Reset Microsoft Edge to Default Settings
 
Make sure to create a restore point just in case something goes wrong.
 
Contents
 
- [GUIDE] Reset Microsoft Edge to Default Settings
 - Method 1: Reset Microsoft Edge using Settings (Clear Browsing Data)
 - Method 2: Reset Microsoft Edge
 - Method 3: Run System File Checker and DISM
 - Method 4: Create a new local account
 - Method 5: Repair Install Windows 10

 
### Method 1: Reset Microsoft Edge using Settings (Clear Browsing Data)
 
1. Open Edge from Windows Search or Start Menu.
 
2. Click on the three dots on the upper right corner and select Settings.
 
3. Under Clear browsing data, click on Choose what to clear.
 
4. Select everything and click the Clear button.
 
4. Wait for the browser to clear all the data and Restart Edge. See if you’re able to Reset Microsoft Edge to Default Settings, if not then continue.
 
### Method 2: Reset Microsoft Edge
 
1. Navigate to the following directory:
 
C:\Users\Your_Username\AppData\Local\Packages
 
Note: To open AppData folder you need to checkmark Show hidden files and folders in Folder Options.
 
2. Find Microsoft.MicrosoftEdge_8wekyb3d8bbwe folder in the list and double-click on it.
 
3. Select all the files and folders inside it and permanently delete them by pressing Shift + Delete.
 
Note: If you get a Folder Access Denied error, click Continue. Right-click on the Microsoft Edge folder and uncheck the Read-only option. Click Apply followed by OK and again see if you’re able to delete the content of this folder.
 
4. Now type PowerShell in Windows search then right-click on it and select Run as Administrator.
 
5. Type the following command into PowerShell and hit Enter:
 
Get-AppXPackage -AllUsers -Name Microsoft.MicrosoftEdge | Foreach {Add-AppxPackage -DisableDevelopmentMode -Register “$($_.InstallLocation)\AppXManifest.xml” -Verbose}
 
6. That’s it! You just reset Microsoft Edge browser to default settings.
 
### Method 3: Run System File Checker and DISM
 
1. Open Command Prompt. The user can perform this step by searching for ‘cmd’ and then press Enter.
 
2. Now type the following in the cmd and hit enter:
 
Sfc /scannow

sfc /scannow /offbootdir=c:\ /offwindir=c:\windows (If above fails then try this one)
 
3. Wait for the above process to finish and once done, restart your PC.
 
4. Again open cmd and type the following command and hit enter after each one:
 
Dism /Online /Cleanup-Image /CheckHealth

Dism /Online /Cleanup-Image /ScanHealth

Dism /Online /Cleanup-Image /RestoreHealth
 
5. Let the DISM command run and wait for it to finish.
 
6. If the above command doesn’t work, then try on the below:
 
Dism /Image:C:\offline /Cleanup-Image /RestoreHealth /Source:c:\test\mount\windows

Dism /Online /Cleanup-Image /RestoreHealth /Source:c:\test\mount\windows /LimitAccess
 
Note: Replace the C:\RepairSource\Windows with your repair source (Windows Installation or Recovery Disc).
 
7. Reboot your PC to save changes and see if you’re able to Reset Microsoft Edge to Default Settings.
 
### Method 4: Create a new local account
 
1. Press Windows Key + I to open Settings and then click Accounts.
 
2. Click on Family & other people tab in the left-hand menu and click Add someone else to this PC under Other people.
 
3. Click, I don’t have this person’s sign-in information in the bottom.
 
4. Select Add a user without a Microsoft account in the bottom.
 
5. Now type the username and password for the new account and click Next.
 
Sign in to this new user account and see if the Windows Store is working or not. If you can successfully Reset Microsoft Edge to Default Settings in this new user account, then the problem was with your old user account, which might have got corrupted, anyway transfer your files to this account and delete the old account to complete the transition to this new account.
 
### Method 5: Repair Install Windows 10
 
This method is the last resort because if nothing works out, then, this method will surely repair all problems with your PC. Repair Install using an in-place upgrade to repair issues with the system without deleting user data present on the system. So follow this article to see How to Repair Install Windows 10 Easily.
 
Recommended:
 
- Fix Photo App Keeps Crashing in Windows 10
 - How to Disable or Uninstall Microsoft Edge
 - Fix Slow Right Click Context Menu in Windows 10
 - Fix Mail and Calendar app crashes on opening in Windows 10

 
That’s it you have successfully learned How to Reset Microsoft Edge to Default Settings in Windows 10 but if you still have any questions regarding the above guide then feel free to ask them in the comment’s section.




