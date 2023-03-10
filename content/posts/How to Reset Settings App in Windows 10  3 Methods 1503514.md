---
title: "Is Your Settings App Driving You Crazy? Use These 3 Easy Methods to Reset in Windows 10!"
ShowToc: true 
date: "2023-03-04"
author: "Jennifer Schiff"
---
*****
Is Your Settings App Driving You Crazy? Use These 3 Easy Methods to Reset in Windows 10!

The Settings app in Windows 10 is a handy tool that allows you to control various aspects of your device. From tweaking display settings to managing device storage, it's aimed at providing an all-in-one solution for customizing the device as per your preferences.

However, sometimes the Settings app may become unresponsive or malfunction, leading to frustration among users. If you're also facing similar issues with your device's Settings app, then resetting it might be the way to go. Here are three easy ways to reset the Settings app in Windows 10.

1. Using the Settings App

If the Settings app is still partially functioning, try to reset it by using its built-in resetting option. Here are the steps to follow:

Step 1: Open the Settings app by pressing the Windows + I keys together.

Step 2: Click on the "System" option from the list of settings.

Step 3: In the left pane, scroll down and click on "Apps & features."

Step 4: In the right pane, search for the Settings app and click on it.

Step 5: Click on the "Advanced options" link.

Step 6: Scroll down and click on the "Reset" button.

Once the reset process is complete, restart your device and check if the Settings app is working as intended.

2. Using PowerShell

If the Settings app is completely unresponsive, you can use the PowerShell command to reset it. Here's how to do it:

Step 1: Type "PowerShell" in the search bar on the taskbar and select "Windows PowerShell" from the results.

Step 2: Right-click on the Windows PowerShell option and select "Run as administrator."

Step 3: In the PowerShell window, type the command "Get-AppxPackage *windows.immersivecontrolpanel* | Foreach {Add-AppxPackage -DisableDevelopmentMode -Register "$($_.InstallLocation)\AppXManifest.xml"}" (without quotes) and press Enter.

This will initiate the resetting process, which might take some time. Once it's complete, restart your device and check if the Settings app is working correctly.

3. Using the Control Panel

If both the above methods fail or you're more comfortable with using the Control Panel, you can reset the Settings app via it. Here's how to do it:

Step 1: Press the Windows + R key together to open the Run dialog box.

Step 2: Type "control" and press Enter to open the Control Panel.

Step 3: Click on the "Programs and Features" option.

Step 4: In the left pane, click on the "Turn Windows features on or off" link.

Step 5: Locate the "Settings" option and uncheck it, then click on "OK."

Step 6: Restart your device.

Step 7: Follow Steps 1 to 4 again and check the "Settings" option, then click on "OK" and restart your device.

This will reset the Settings app, and it should work correctly once again.

In Conclusion

Resetting the Settings app can help you get rid of any issues that are driving you crazy. We hope these three methods help you in resetting the Settings app on your Windows 10 device. Try them out and let us know which one worked for you.

{{< youtube s8ABl5WFmPw >}} 



However, just like every other app, the Settings app can also sometimes malfunction. Recently, lots of users have reported that they are facing problems while accessing the Settings app. Few have reported that the Settings app crashes and fails to open.
So, if you are experiencing problems with the Settings app in Windows 10, you might expect some help here. This article will list down the best ways to reset the Settings app in Windows 10. So, let’s check out.
Also Read: Enable “Share Settings” Option in the Windows 10 Settings App

 
## 3 Best Methods to Reset Settings App in Windows 10


Note: Like resetting any other apps, resetting the Settings app will also remove various settings. It will bring different options to their default values. So, if you are using custom settings for any Windows feature, backup the important files.

 
### 1. Reset From the Start Menu


In this method, we will use the default Start menu to reset the Settings app on Windows 10. Follow some of the simple steps given below.
Step 1. First of all, open the Windows Search box and type in ‘Settings.’

Step 2. Right-click on the Settings app, and click on ‘App Settings.’

Step 3. Now on the Settings Window, scroll down and click on the ‘Reset‘ button as shown below.

Step 4. On the confirmation popup, click on the ‘Reset’ button once again.


 
### 2. Reset Settings App Using PowerShell


If you are running Windows 10 version 21H2 or later, you can use PowerShell to reset the Windows 10 Settings app. Follow some of the simple steps given below to reset the Settings app via PowerShell.
Step 1. First of all, open Windows Search and search for ‘Windows PowerShell.’
Step 2. Right-click on the Windows Powershell and select ‘Run as Administrator.’

Step 3. On the PowerShell window, enter:
Get-AppxPackage *windows.immersivecontrolpanel* | Reset-AppxPackage

Step 4. Once done, press the Enter button.
That’s it! You are done. This is how you can reset Windows 10 Settings app via Powershell.

 
### 3. Reset the Settings App via Command Prompt


If you are not running Windows 10 version 21H2, you need to utilize the Command Prompt to reset the Settings app. Follow some of the simple steps given below to reset the Settings app via CMD.
Step 1. First of all, open Windows search and search for ‘Command Prompt.’
Step 2. Right-click on the Command Prompt and select ‘Run as administrator.’

Step 3. On the Command Prompt, enter the command –
PowerShell -ExecutionPolicy Unrestricted -Command "& {$manifest = (Get-AppxPackage *immersivecontrolpanel*).InstallLocation + '\AppxManifest.xml' ; Add-AppxPackage -DisableDevelopmentMode -Register $manifest}"

Step 4. Once done, press the Enter button.
That’s it! You are done. This is how you can reset the Settings app via Command Prompt.
So, this guide is all about how to reset the Settings app on Windows 10. I hope this article helped you! Please share it with your friends also. If you have any doubts related to this, let us know in the comment box below.





