---
title: "Uncover the Secret to Installing Hyper V on Windows 11 Home in Just a Few Clicks!"
ShowToc: true 
date: "2022-12-01"
author: "Harold Crispin"
---
*****
# Uncover the Secret to Installing Hyper V on Windows 11 Home in Just a Few Clicks!

If you are a Windows 11 Home user and want to install Hyper V on your system, you might be facing some hurdles. Hyper V is a virtualization software program that allows you to run multiple operating systems on a single computer. This means you can create virtual machines, switch between them, and use them to run tests, develop software, or simulate different environments on your device.

However, installing Hyper V on a Windows 11 Home system is not as straightforward as it is on a Windows 11 Pro or Enterprise edition. That is because Home versions do not come with native support for virtualization, making it impossible to install Hyper V from the Settings app.

In this article, we will uncover the secret to installing Hyper V on your Windows 11 Home system with just a few clicks. Follow the steps below to get started.

## Step 1 – Check your System’s Compatibility

Before you start installing Hyper V, make sure that your system meets the hardware requirements. Hyper V requires a 64-bit processor that supports hardware-assisted virtualization (Intel VT or AMD-V), as well as at least 4 GB of RAM and 50 GB of free storage space.

To check if your system meets these requirements, do the following:

1. Press the Windows key + R to open the Run dialog box.
2. Type “msinfo32” and press Enter to launch the System Information window.
3. Look for the System Type and check if it says “x64-based PC.” If it is, your system is 64-bit and compatible with Hyper V.
4. Check for the Processor section and look for “Virtualization Enabled in Firmware.” If it is, your CPU supports hardware-assisted virtualization.

If your system meets these requirements, you can proceed to the next step.

## Step 2 – Install Hyper V Using Command Prompt

To install Hyper V on Windows 11 Home, you need to use Command Prompt as an administrator. Here’s how:

1. Right-click on the Start menu and select “Windows PowerShell (Admin)” from the list.
2. In the PowerShell window, type “dism.exe /online /enable-feature /featurename:Microsoft-Hyper-V –All” and press Enter.
3. Wait for the installation to complete. Depending on your system’s speed, this may take up to 10-15 minutes.
4. Once the installation is complete, restart your system.

That’s it! You have successfully installed Hyper V on your Windows 11 Home system. You can now create virtual machines and start using them to run different operating systems on your device.

## Conclusion

Installing Hyper V on Windows 11 Home is a bit tricky compared to Pro or Enterprise versions, but it is not impossible. By following the steps above, you can easily install Hyper V on your system and start running virtual machines in just a few clicks.

Remember to check your system’s compatibility before you start, as Hyper V requires specific hardware requirements to work correctly. If you face any issues during the installation or have any questions, you can always refer to the Microsoft documentation or seek help from online forums. Happy virtualizing!

{{< youtube ExZIQj-DvI8 >}} 



The Microsoft Hyper-V feature to run virtual machines is only available on Windows 11 Pro, but there’s a way to install it on Windows 11 Home, and in this guide, you will learn how.
 
On Windows 11, Hyper-V allows you to create and manage virtual machines to run other instances of Windows 11 and older versions of the operating system, such as Windows 10, 8.1, or 7, or other platforms like Linux alongside the main installation.
 
The only caveat is that Microsoft reserves the feature only for the Pro and higher editions of Windows 11. However, if you use the Home edition and don’t want to use other virtualization alternatives, such as VirtualBox, it’s possible to install Hyper-V on your Windows 11 home computer.
 
This guide will teach you the steps to enable or disable Hyper-V on Windows 11 Home.
 
- Enable virtualization on Windows 11 Home
 - Install Hyper-V on Windows 11 Home
 - Disable Hyper-V on Windows 11 Home

 
## Enable virtualization on Windows 11 Home
 
Before enabling Hyper-V on the Home edition of Windows 11, the device must have virtualization support enabled on the UEFI (Unified Extensible Firmware Interface). If you don’t have this feature enabled, check with your manufacturer to find the specific details to complete this task.
 
### Check virtualization support
 
To check whether the UEFI firmware has virtualization enabled on Windows 11 Home, use these steps:
 
- Open Start.
 - Search for Task Manager and click the top result to open the app.
 - Click on Performance.
 - Confirm that “Virtualization” reads “Enabled” next to the system stats.

 
If virtualization is disabled, then continue with the steps below.
 
Open Start.
 
Search for Task Manager and click the top result to open the app.
 
Click on Performance.
 
Confirm that “Virtualization” reads “Enabled” next to the system stats.
 

 
### Enable virtualization on Windows 11 Home
 
To enable virtualization on Windows 11 Home, use these steps:
 
- Open Settings.
 - Click on System.
 - Click on Recovery.
 - Under the “Recovery options” section, click the Restart now button for the “Advanced startup” setting.
 - Click on Troubleshoot.
 - Click on Advanced options.
 - Click the UEFI Firmware Settings option.
 - Click the Restart button.
 - Open the Configuration, Security, or Advanced page (the page’s name will depend on your manufacturer).
 - Select the Virtualization Technology, Intel Virtual Technology, or SVM Mode option (the feature name will depend on your manufacturer).
 - Enable the virtualization feature.
 - Save the UEFI (BIOS) settings (usually press F10).

 
After you complete the steps, you can proceed to enable the Microsoft hypervisor to run virtual machines on Windows 11.
 
Open Settings.
 
Click on System.
 
Click on Recovery.
 
Under the “Recovery options” section, click the Restart now button for the “Advanced startup” setting.
 
Click on Troubleshoot.
 
Click on Advanced options.
 
Click the UEFI Firmware Settings option.
 
Click the Restart button.
 
Open the Configuration, Security, or Advanced page (the page’s name will depend on your manufacturer).
 
Select the Virtualization Technology, Intel Virtual Technology, or SVM Mode option (the feature name will depend on your manufacturer).
 
Enable the virtualization feature.
 
Save the UEFI (BIOS) settings (usually press F10).
 
## Install Hyper-V on Windows 11 Home
 
Since the Home edition doesn’t have the virtualization feature, you must install the components manually through a simple script. Although the script works as intended, you should always create a temporary full backup of your computer since you will modify the system files, which Microsoft doesn’t support.
 
To install Hyper-V on Windows 11 Home, use these steps:
 
- Open Start.
 - Search for Notepad and click the top result to open the app.
 - Copy and paste the following script into the text file:
 - pushd "%~dp0"
 - dir /b %SystemRoot%\servicing\Packages\*Hyper-V*.mum >hv-home.txt
 - for /f %%i in ('findstr /i . hv-home.txt 2^>nul') do dism /online /norestart /add-package:"%SystemRoot%\servicing\Packages\%%i"
 - del hv-home.txt
 - Dism /online /enable-feature /featurename:Microsoft-Hyper-V -All /LimitAccess /ALL
 - pause
 - Click on File and choose the “Save as” option.
 - Confirm a name and use the .bat extension. For example, hyperv-home.bat.
 - Click the Save button.
 - Right-click the hyperv-home.bat file and select the Run as administrator option.
 - Press the Y key to restart the computer.

 
After you complete the steps, the Hyper-V Management Tool and Platform will install on your Home edition of Windows 11.
 
Search for Notepad and click the top result to open the app.
 
Copy and paste the following script into the text file:
 
pushd "%~dp0"

dir /b %SystemRoot%\servicing\Packages\*Hyper-V*.mum >hv-home.txt

for /f %%i in ('findstr /i . hv-home.txt 2^>nul') do dism /online /norestart /add-package:"%SystemRoot%\servicing\Packages\%%i"

del hv-home.txt

Dism /online /enable-feature /featurename:Microsoft-Hyper-V -All /LimitAccess /ALL

pause
 
Click on File and choose the “Save as” option.
 
Confirm a name and use the .bat extension. For example, hyperv-home.bat.
 
Click the Save button.
 
Right-click the hyperv-home.bat file and select the Run as administrator option.
 
Press the Y key to restart the computer.
 
## Disable Hyper-V on Windows 11 Home
 
Once you have installed the virtualization feature, you can enable or disable it from the system feature settings like Windows 11 Pro.
 
To disable Hyper-V on Windows 11 Home, use these steps:
 
- Open Settings.
 - Click on Apps.
 - Click the Optional features tab.
 - Under the “Related settings” section, click the “More Windows features” setting.
 - Clear the Hyper-V feature.
 - Click the OK button.
 - Click the Restart now button.

 
Once you complete the steps, Microsoft Hyper-V will be disabled on Windows 11 Home.
 
Click on Apps.
 
Click the Optional features tab.
 
Under the “Related settings” section, click the “More Windows features” setting.
 
Clear the Hyper-V feature.
 
Click the OK button.
 
Click the Restart now button.




