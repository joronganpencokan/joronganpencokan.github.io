---
title: "Unlock the Secret to Supercharging Your Web Browsing Speed: Move Your IE Temporary Internet Files Folder Now!"
ShowToc: true 
date: "2023-04-23"
author: "Irene Carter"
---
*****
Title: Unlock the Secret to Supercharging Your Web Browsing Speed: Move Your IE Temporary Internet Files Folder Now!

As a web user, you may find that browsing the internet can be frustratingly slow at times. Often, your internet connection may not be at fault, but rather the speed at which your browser loads web pages. This can be due to a variety of reasons, but there is one factor that you can control to speed up your web browsing time: the temporary internet files folder in Internet Explorer (IE).

The temporary internet files folder is where IE stores copies of web pages, images, and other media files that you have visited on the internet. The purpose of this is to speed up the loading time of web pages upon your return, as the files are stored locally on your computer. However, with time, this folder can grow to an enormous size and start to slow down your browsing speed.

So, what can you do to supercharge your web browsing speed?

The answer is simple: move your IE temporary internet files folder to a different location.

By moving the temporary internet files folder to a separate hard drive or partition, you can free up space on your main hard drive and improve the speed at which your browser loads web pages. This is because the temporary internet files folder will no longer have to compete for space with your operating system and other applications.

To move the temporary internet files folder in IE, follow these steps:

1. Open Internet Explorer and go to "Internet Options" in the Tools menu.
2. Select the "General" tab and click on "Settings" under "Browsing history".
3. In the "Temporary Internet Files" section, click on "Move Folder".
4. Choose a new location for your temporary internet files folder and click on "OK" to save the changes.

It is important to note that moving the temporary internet files folder may affect your browsing history and offline access to web pages. However, this can easily be remedied by adjusting the settings in Internet Options to accommodate the new location of the folder.

In conclusion, moving your IE temporary internet files folder is a simple and effective way to supercharge your web browsing speed. By freeing up space on your main hard drive and allowing your browser to load web pages faster, you can save time and frustration while browsing the internet. So, give it a try and unlock the secret to faster web browsing today!

{{< youtube D0-BHy34H6E >}} 




This article explains how to move the Temporary Files folder in Internet Explorer on Windows 11 through Windows XP, but there are differences.

 
### 
What to Know
 
- First, configure Windows to show hidden files and folders, then open Run dialog box and enter inetcpl.cpl.In the Browsing history section, select Settings > Move folder .Find the default folder Internet Explorer uses to store temporary internet files > OK.

 
##   Reset the Internet Files Folder to Its Default Location  
 

First, configure Windows to show hidden files and folders. Some steps below require that hidden folders are viewable, so this prerequisite is a must-do. After you hidden files and folders are viewable, follow these steps:

 
Microsoft no longer supports Internet Explorer and recommends that you update to the newer Edge browser. Head to their site to download the newest version.
 
- Open the Run dialog box with the WIN+R shortcut.
 - Type inetcpl.cpl in the text box, and then press OK.
 - Select Settings from the Browsing history section.
 - Choose Move folder at the bottom of the window.
 - Select the down arrow or plus sign (whichever you see) next to the C: drive to open that folder.
 - Select the arrow or plus sign next to Users, or Documents and Settings if you see that, followed by the folder corresponding to your username. For example, I would expand the folder Tim since that's my username.
 - Navigate to the default folder Internet Explorer uses to store temporary internet files:
 - Windows 11, 10, and 8:
 - C:\Users\[username]\AppData\Local\Microsoft\Windows\iNetCache\
 - Windows 7 and Vista:
 - C:\Users\[username]\AppData\Local\Microsoft\Windows\Temporary Internet Files
 - Windows XP:
 - C:\Documents and Settings\[username]\Local Settings\
 - Once you've landed on the last folder in the path you see above, just highlight it, you don't need to select the arrow or plus sign next to it.
 - Don't see the right folder? Windows may not be configured to show hidden files and folders, or you might need to also show protected operating system files. See Step 1 above for more information. If you complete Step 1 now, you have to jump back to Step 5 to refresh the folders.
 - Select OK in the Browse for Folder window, and then again in the other window.
 - Select Yes if prompted to log off to finish moving temporary internet files.
 - Your computer will immediately log off, so be sure to save and close any files you might be working in before choosing Yes.
 - Log back onto Windows and test to see if returning the Temporary Internet Files folder to its default location has solved your problem.
 - Configure Windows to hide hidden files and folders. These steps demonstrate how to hide hidden files from normal view, undoing the steps you took in Step 1.

 
##   Reset IE Temporary Files Folder Using Windows Registry  
 

Another way to make this change is to use the Windows Registry. It's much easier to use Internet Explorer as described above, but if you can't for some reason, try this method.

 

Open the Run dialog box with the WIN+R shortcut.

 

Type inetcpl.cpl in the text box, and then press OK.

 

Select Settings from the Browsing history section.

 

Choose Move folder at the bottom of the window.

 

Select the down arrow or plus sign (whichever you see) next to the C: drive to open that folder.

 

Select the arrow or plus sign next to Users, or Documents and Settings if you see that, followed by the folder corresponding to your username. For example, I would expand the folder Tim since that's my username.

 

Navigate to the default folder Internet Explorer uses to store temporary internet files:

 

Windows 11, 10, and 8:

 

C:\Users\[username]\AppData\Local\Microsoft\Windows\iNetCache\

 

Windows 7 and Vista:

 

C:\Users\[username]\AppData\Local\Microsoft\Windows\Temporary Internet Files

 

Windows XP:

 

C:\Documents and Settings\[username]\Local Settings\

 

Once you've landed on the last folder in the path you see above, just highlight it, you don't need to select the arrow or plus sign next to it.

 
Don't see the right folder? Windows may not be configured to show hidden files and folders, or you might need to also show protected operating system files. See Step 1 above for more information. If you complete Step 1 now, you have to jump back to Step 5 to refresh the folders.
 

Select OK in the Browse for Folder window, and then again in the other window.

 

Select Yes if prompted to log off to finish moving temporary internet files.

 

Your computer will immediately log off, so be sure to save and close any files you might be working in before choosing Yes.

 

Log back onto Windows and test to see if returning the Temporary Internet Files folder to its default location has solved your problem.

 

Configure Windows to hide hidden files and folders. These steps demonstrate how to hide hidden files from normal view, undoing the steps you took in Step 1.

 
- Open Registry Editor.
 - Navigate to the HKEY_CURRENT_USER hive and then follow this path:
 - Software\Microsoft\Windows\CurrentVersion\Explorer\User Shell Folders
 - Double-click Cache on the right side of Registry Editor.
 - Type the correct value for your version of Windows:
 - Windows 11, 10, and 8:
 - %USERPROFILE%\AppData\Local\Microsoft\Windows\iNetCache\
 - Windows 7 and Vista:
 - %USERPROFILE%\AppData\Local\Microsoft\Windows\Temporary Internet Files
 - Windows XP:
 - %USERPROFILE%\Local Settings\Temporary Internet Files
 - Select OK.
 - Repeat Steps 3–5 but under this path, also in the HKEY_CURRENT_USER hive:
 - Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders
 - Close Registry Editor.
 - Restart your computer.

 
##   Why Move IE Temporary Files?  
 

By default, the Temporary Internet Files folder in Internet Explorer is buried deep within several folders. As the name would suggest, the IE browser uses this folder to store temporary internet files.

 

Open Registry Editor.

 

Navigate to the HKEY_CURRENT_USER hive and then follow this path:

 

Software\Microsoft\Windows\CurrentVersion\Explorer\User Shell Folders

 

Double-click Cache on the right side of Registry Editor.

 

Type the correct value for your version of Windows:

 

%USERPROFILE%\AppData\Local\Microsoft\Windows\iNetCache\

 

%USERPROFILE%\AppData\Local\Microsoft\Windows\Temporary Internet Files

 

%USERPROFILE%\Local Settings\Temporary Internet Files

 

Select OK.

 

Repeat Steps 3–5 but under this path, also in the HKEY_CURRENT_USER hive:

 

Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders

 

Close Registry Editor.

 

Restart your computer.

 

If for some reason the location of that folder has moved—like due to a malware issue or a change you made yourself—some very specific issues and error messages can occur, the ieframe.dll DLL error being a common example.

 

Moving this folder back to its default location is easy through Internet Explorer's own settings, so you don't have to remove and reinstall Internet Explorer or reset all of its options.

 
##   Still Can't Change the Folder?  
 

If after making the changes above, the location of the Temporary Internet Files folder still won't change, even after a reboot, there are a couple of things to look at that could be the cause.

 
If you don't remember changing this folder location yourself, and especially if your computer is behaving abnormally, be sure to run a malware scan to remove any potentially unwanted program that could have changed the folder location without you knowing.
 

For starters, check that your antivirus program is running and actively scanning to catch malware. It's possible that a virus on your computer is to blame for these settings not changing when you tell them to.

 

With that being said, some antivirus programs are over-protective of the registry and will prevent changes, so even if you're making the change yourself, the antivirus program might be blocking your attempts. If you're sure you're not currently suffering from malware, temporarily disable your antivirus program and try again.

 

If the folder can be altered while your antivirus program is off, reboot and check again just to be sure. If the new folder location stays, turn your security software back on. The change you made should stick since the antivirus program wasn't active during the change.

 

Get the Latest Tech News Delivered Every Day




