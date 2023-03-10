---
title: "Revamp Your Windows 10 Experience: Learn How to Install Updates Like a Pro!"
ShowToc: true 
date: "2022-12-07"
author: "Marilyn Hartwig"
---
*****
Title: Revamp Your Windows 10 Experience: Learn How to Install Updates Like a Pro!

Introduction:

As Windows 10 is the most popular operating system globally, it is essential to know how to install updates like a pro. Windows operating systems are known for their bundle of features, functionalities, and security releases. However, all of them require updates to ensure that users can use them without any glitches. Thus, if you wish to revamp your Windows 10 experience and learn how to install updates, read on!

Step 1: Know your Windows 10 version

The first step is to determine which version of Windows 10 you are using. You can find it out by going to Start Menu > Settings > System > About. Once you know it's version, you can download relevant updates to keep the system up to date.

Step 2: Check for updates

To check for updates, go to Start Menu > Settings > Update & Security. The Update & Security option provides the details of the last time Windows was updated to the latest version and security updates. If it shows the latest version, you need not do anything further.

Step 3: Download Updates

If the update is available, download it immediately to keep Windows 10 safe and secure. Once you click on the Check for Updates option, the computer starts scanning for the latest updates, including security upgrades. Microsoft releases these upgrades frequently for the users to keep their computer's protection up-to-date.

Step 4: Install updates

After downloading the updates, install them on your computer. The computer prompts you to either "Update Now" or "Schedule the Restart" option. If you wish to continue with the update process immediately, click the Update Now button. It takes around 15-20 minutes to install the updates.

Step 5: Restart your computer

Once the installation is done, restart your computer to make the updates effective. You can let the computer restart automatically, or you can schedule it as per your convenience.

Step 6: Check for successful update installation

After restarting the computer, go to Start Menu > Settings > Update & Security > Windows Update. Once there, click on the Check for Updates option again to ensure that all the updates have been successfully installed.

Conclusion:

Windows 10 updates are crucial to get the latest features and security updates. By following the above steps, you can ensure that your computer is updated regularly to make your computing experience faster, secure, and reliable. Install the updates like a pro to revamp your Windows 10 experience and make the most out of it!

{{< youtube mc4d7ewuqiM >}} 



On Windows 10, cumulative updates (or quality updates) are essential to fix bugs, patch security vulnerabilities, and improve system performance. Although the Windows Update service regularly applies updates automatically, sometimes, you may still need to check and install them manually for many reasons.
 
For example, after performing a clean install of Windows 10 or when the device hadn’t been online for a long time, it missed some important improvements. If the Windows Update service is not working and you need to apply the latest patches to resolve the issue. You need to install a newer driver update for a device. Or you want to upgrade to a new version of the operating system.
 
Whatever the reason it might be, on Windows 10, there are at least four ways to update the system using the Windows Update settings, manual download, Command Prompt, and PowerShell.
 
Microsoft offers three main types of updates, quality, optional, and features updates. Quality updates are available every month, and they include security and non-security fixes and improvements. Optional updates are not critical but necessary, and they include drivers and product updates. Finally, feature updates are new versions of Windows 10 (such as version 21H1). They include new features, changes, and fixes. Windows 10 receives two feature updates per year, and they usually require reinstallation and multiple restarts.
 
In this guide, you will learn the different ways to download and install cumulative updates on Windows 10. In addition, we will outline the steps to install optional and feature updates.
 
- Install updates on Windows 10 via Windows Update
 - Install updates on Windows 10 via Microsoft Update Catalog
 - Install updates on Windows 10 via Command Prompt
 - Install updates on Windows 10 via PowerShell
 - Install optional updates on Windows 10
 - Install feature updates on Windows 10

 
## Install updates on Windows 10 via Windows Update
 
To download and install updates with Windows Update, use these steps:
 
- Open Settings on Windows 10.
 - Click on Update & Security.
 - Click on Windows Update.
 - Click the Check for updates button.
 - Windows Update settings
 - (Optional) Click the Download and install option to apply a preview update of Windows 10.
 - Quick note: A preview is an optional update that includes all the non-security patches that Microsoft plans to release in the next Patch Tuesday rollout. You are not required to download these updates.
 - Click the Restart now button.

 
Once you complete the steps, if an update is available, it will download and install automatically.
 
Open Settings on Windows 10.
 
Click on Update & Security.
 
Click on Windows Update.
 
Click the Check for updates button.
 
Windows Update settings

 
(Optional) Click the Download and install option to apply a preview update of Windows 10.
 
Click the Restart now button.
 
## Install updates on Windows 10 via Microsoft Update Catalog
 
To download and apply the update package manually, use these steps:
 
- Open Microsoft Update Catalog website.
 - Search for the knowledge base number of the update – for example, KB5001391.
 - Quick tip: If you do not know the latest update reference number, you can check the update history tracker.
 - Click the Download button for the cumulative update you want to install.
 - Microsoft Update Catalog
 - Quick note: The page usually lists four versions of a particular package, including ARM64, x64, x86, and the one for Windows Server. The download you need will depend on the system you have. However, most of the time, you want to download the x64 version, which is the 64-bit version of the update. Of course, if you have a 32-bit version of Windows 10, then download the x86 option.
 - Click the link to download the .msu package.
 - Click the Close button.
 - Double-click the .msu file.
 - Click the Yes button to install the update.
 - Standalone installer
 - Click the Restart now button.

 
After you complete the steps, the cumulative update will apply to the computer.
 
Open Microsoft Update Catalog website.
 
Search for the knowledge base number of the update – for example, KB5001391.
 
Click the Download button for the cumulative update you want to install.
 
Click the link to download the .msu package.
 
Click the Close button.
 
Double-click the .msu file.
 
Click the Yes button to install the update.
 
Standalone installer

 
## Install updates on Windows 10 via Command Prompt
 
While Command Prompt does not have a mechanism to check for updates, you can use the console to install a .msu package to update the system with the latest fixes.
 
To install updates of Windows 10 using Command Prompt, use these steps:
 
- Open Microsoft Update Catalog website.
 - Search for the knowledge base number of the update – for example, KB5001391.
 - Click the Download button for the cumulative update you want to install.
 - Microsoft Update Catalog
 - Click the link to download the .msu package.
 - Click the Close button.
 - Open Start.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to install a new update on Windows 10 and press Enter:
 - wusa c:\PATH\TO\UPDATE.msu /quiet /norestart
 - In the command, update the path with the location and name of the .msu update package.
 - This example installs the KB5001391 update:
 - wusa c:\Users\USERACCOUNT\Downloads\windows10.0-kb5001391-x64.msu /quiet /norestart
 - Windows Update in Command Prompt
 - Type the following command to confirm the update was installed correctly and press Enter:
 - wmic qfe list brief /format:table
 - Quick note: Updates can take a long time to install. As a result, you should allow around five to ten minutes before running this command. Once the update appears in the list, you can proceed to restart the device.
 - Type the following command to restart the device and press Enter:
 - shutdown /r /t 00

 
After you complete the steps, the quality update will install quietly, and the device will restart to finish applying the changes on Windows 10.
 
Microsoft Update Catalog

 
Open Start.
 
Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 
Type the following command to install a new update on Windows 10 and press Enter:
 
wusa c:\PATH\TO\UPDATE.msu /quiet /norestart
 
In the command, update the path with the location and name of the .msu update package.
 
This example installs the KB5001391 update:
 
wusa c:\Users\USERACCOUNT\Downloads\windows10.0-kb5001391-x64.msu /quiet /norestart
 
Windows Update in Command Prompt

 
Type the following command to confirm the update was installed correctly and press Enter:
 
wmic qfe list brief /format:table
 
Type the following command to restart the device and press Enter:
 
shutdown /r /t 00
 
## Install updates on Windows 10 via PowerShell
 
Alternatively, you can also install a PowerShell module to manage updates on Windows 10.
 
To check and install Windows 10 updates with PowerShell, use these steps:
 
- Open Start.
 - Search for PowerShell, right-click the top result, and select the Run as administrator option.
 - Type the following command to install the PowerShell module to update Windows 10 and press Enter:
 - Install-Module PSWindowsUpdate
 - PSWindowsUpdate
 - Type A to accept and install the module and press Enter.
 - Type the following command to check for Windows 10 updates with PowerShell and press Enter:
 - Get-WindowsUpdate
 - Get-WindowsUpdate
 - Type the following command to select, download, and install a specific update and press Enter:
 - Install-WindowsUpdate -KBArticleID KBNUMBER
 - In the command, make sure to replace KBNUMBER with the update number you want to install.
 - This example downloads and applies the KB2267602 update for Microsoft Defender:
 - Install-WindowsUpdate -KBArticleID KB2267602
 - Install-WindowsUpdate KBArticleID
 - Type A to confirm the installation and press Enter.
 - (Optional) Type the following command download and install all available updates and press Enter:
 - Install-WindowsUpdate
 - Install-WindowsUpdate
 - Quick note: When using this command, you will be applying system updates as well as optional updates that may include driver updates.
 - Type A to confirm the installation and press Enter.
 - (Optional) Type the following command to view a list of previously installed updates and press Enter:
 - Get-WUHistory
 - Get-WUHistory

 
Once you complete the steps, the Windows 10 updates will download and install on your device.
 
Search for PowerShell, right-click the top result, and select the Run as administrator option.
 
Type the following command to install the PowerShell module to update Windows 10 and press Enter:
 
Install-Module PSWindowsUpdate
 
PSWindowsUpdate

 
Type A to accept and install the module and press Enter.
 
Type the following command to check for Windows 10 updates with PowerShell and press Enter:
 
Get-WindowsUpdate
 
Get-WindowsUpdate

 
Type the following command to select, download, and install a specific update and press Enter:
 
Install-WindowsUpdate -KBArticleID KBNUMBER
 
In the command, make sure to replace KBNUMBER with the update number you want to install.
 
This example downloads and applies the KB2267602 update for Microsoft Defender:
 
Install-WindowsUpdate -KBArticleID KB2267602
 
Install-WindowsUpdate KBArticleID

 
Type A to confirm the installation and press Enter.
 
(Optional) Type the following command download and install all available updates and press Enter:
 
Install-WindowsUpdate
 
(Optional) Type the following command to view a list of previously installed updates and press Enter:
 
Get-WUHistory
 
Get-WUHistory

 
## Install optional updates on Windows 10
 
Optional updates are not critical to Windows 10, but they may be necessary for other functionalities. Usually, these updates are available for Microsoft and non-Microsoft products, feature updates, and third-party drivers (such as printers, cameras, network adapters, graphics cards, and other USB or Bluetooth peripherals).
 
To download and install optional updates on Windows 10, use these steps:
 
- Open Settings.
 - Click on Update & Security.
 - Click on Windows Update.
 - Click the View optional updates option.
 - Windows 10 view optional updates
 - Quick note: If the option isn’t available, then Windows Update doesn’t have any additional drivers for your device.
 - Click the category to see the optional updates. For example, Driver updates.
 - Check the optional updates you want to install.
 - Windows 10 install optional updates
 - Click the Download and install button.

 
After you complete the steps, Windows Update will download and install the packages on your device.
 
Open Settings.
 
Click the View optional updates option.
 
Click the category to see the optional updates. For example, Driver updates.
 
Check the optional updates you want to install.
 
Windows 10 install optional updates

 
Click the Download and install button.
 
In the previous versions, you were also able to install optional driver updates using Device Manager. However, the option has been removed, and now, all the updates are available through the Windows Update settings page.
 
## Install feature updates on Windows 10
 
Feature updates are technically new versions of Windows 10 that include new features and significant changes. These updates are optional, and you must install them manually to upgrade to a new version.
 
The instructions below provide an overview of the installation process. However, since these updates may cause problems during and after installation, you should create a full backup before proceeding if something goes wrong and you need to roll back.
 
To install a feature update (such as version 20H2 or 2004), use these steps:
 
- Open Settings.
 - Click on Update & Security.
 - Click on Windows Update.
 - Click on Check for updates button (if applicable).
 - Under the “Optional updates available” section, click the Download and Install now button.
 - Windows 10 feature update install
 - Click the Restart now button.

 
In addition to Windows Update, you can also install feature updates using the Media Creation Tool using an in-place upgrade or clean installation. Also, you can use the Update Assistant, which is a tool that allows you to install a new feature update using an in-place upgrade.
 
Click on Check for updates button (if applicable).
 
Under the “Optional updates available” section, click the Download and Install now button.
 
Windows 10 feature update install





