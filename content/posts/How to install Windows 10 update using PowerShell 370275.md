---
title: "Unleash the Power of Windows 10: Install the Latest Update with These Insanely Simple Powershell Hacks!"
ShowToc: true 
date: "2023-04-15"
author: "Norma Lowder"
---
*****
# Unleash the Power of Windows 10: Install the Latest Update with These Insanely Simple Powershell Hacks!

Are you tired of outdated operating systems, slow response times, and frequent crashes? Fortunately, Windows 10 provides a reliable and secure platform for your daily computing needs. However, to take advantage of the latest features and benefits, you need to regularly update your system. By using these simple PowerShell hacks, you can easily install the latest Windows 10 update and supercharge your computer's performance.

## What is PowerShell?

PowerShell is a command-line shell and scripting language developed by Microsoft for system administration purposes. It allows you to automate complex tasks and manage Windows-based machines more efficiently. PowerShell is built on top of the .NET framework and supports object-oriented programming concepts.

PowerShell provides a rich set of commands (called cmdlets) that enable you to perform various tasks, such as creating and deleting files, managing network connections, retrieving system information, and more. You can run PowerShell commands from the command-line interface (CLI) or write PowerShell scripts to automate repetitive tasks.

## How to Install the Latest Windows 10 Update using PowerShell?

Before you start, make sure you have an active internet connection and enough storage space on your hard drive to download and install the latest Windows 10 update. Follow these steps to install the update using PowerShell:

1. Open PowerShell as an administrator. You can do this by right-clicking the Start button and selecting "Windows PowerShell (Admin)" from the context menu.

2. Type the following command and press Enter to check for available updates:

```
Get-WindowsUpdate -Install -AcceptAll
```

This command checks for available updates and installs them automatically. You might see a progress bar indicating the status of the update installation.

3. Wait for the update to finish installing. This may take several minutes or even hours, depending on the size of the update and the speed of your internet connection.

4. Restart your computer to apply the changes. After the restart, you should have the latest version of Windows 10 installed.

## How to Optimize Your Windows 10 Performance using PowerShell?

After installing the latest Windows 10 update, you can use PowerShell to optimize your computer's performance further. Here are some simple PowerShell hacks you can use:

1. Clean up your temporary files: Over time, your computer tends to accumulate temporary files that consume disk space and slow down the system. You can use the following command to remove temporary files:

```
Remove-Item -Path "$env:LOCALAPPDATA\Temp" -Recurse -Force
```

This command deletes all temporary files from your computer's local app data folder.

2. Disable unnecessary startup programs: Some programs start automatically when you log in to your Windows account, consuming system resources and slowing down the startup process. You can use the following command to disable some of these programs:

```
Set-ItemProperty -Path 'HKCU:\Software\Microsoft\Windows\CurrentVersion\Explorer\StartupApproved\Run' -Name '{Program name}' -Value '0'
```

Replace '{Program name}' with the name of the program you want to disable. This command modifies the Windows registry to prevent the program from starting automatically.

3. Disable Windows animations: Windows provides various animations and visual effects that enhance the user experience, but they also consume system resources and slow down the system. You can use the following command to disable animations:

```
Set-ItemProperty -Path 'HKCU:\Control Panel\Desktop' -Name 'UserPreferencesMask' -Value ([byte[]](0x90, 0x12, 0x03, 0x80, 0x10, 0x00, 0x00, 0x00))
```

After running this command, you need to log out and log in again to apply the change.

## Conclusion

PowerShell provides a powerful and flexible way to manage your Windows 10 system and optimize its performance. By using these simple PowerShell hacks, you can install the latest Windows 10 update and make your computer faster and more efficient. With a little bit of practice and experimentation, you can discover many more PowerShell tips and tricks to unlock the full potential of your Windows 10 machine.

{{< youtube ZdhU2-TPj7o >}} 



Windows 10 updates happen automatically or manually through the Windows Update settings. However, if you try to patch a new installation or create a custom script to automate the process, you can use commands to download and install missing patches with “PSWindowsUpdate” on PowerShell.
 
PSWindowsUpdate is a community module by Michal Gajda, available through the PowerShell Gallery. It includes the components to make it easy to check, download, and install quality updates on Windows 10.
 
In this guide, you’ll learn the steps to check and install updates for Windows 10 using PowerShell.
 
- Update Windows 10 from PowerShell
 - Manage updates with PowerShell

 
## Update Windows 10 from PowerShell
 
To check and install updates with PowerShell, use these steps:
 
- Open Start on Windows 10.
 - Search for PowerShell, right-click the top result, and select the Run as administrator option.
 - Type the following command to install the module to run Windows Update and press Enter:
 - Install-Module PSWindowsUpdate
 - Quick note: After installing the module, you no longer need to repeat step No. 3 to use the module and manage updates.
 - Type A and press Enter to confirm.
 - Type the following command to check for updates with PowerShell and press Enter:
 - Get-WindowsUpdate
 - Type the following command to install the available Windows 10 updates and press Enter:
 - Install-WindowsUpdate
 - Type A and press Enter to confirm.

 
Once you complete the steps, the latest cumulative updates will download and install on your computer.
 
Open Start on Windows 10.
 
Search for PowerShell, right-click the top result, and select the Run as administrator option.
 
Type the following command to install the module to run Windows Update and press Enter:
 
Install-Module PSWindowsUpdate
 

 
Type A and press Enter to confirm.
 
Type the following command to check for updates with PowerShell and press Enter:
 
Get-WindowsUpdate
 
Type the following command to install the available Windows 10 updates and press Enter:
 
Install-WindowsUpdate
 
## Manage updates with PowerShell
 
The PSWindowsUpdate module includes many options that you can use to manage updates. You can always use the Get-Command –Module PSWindowsUpdate command to query a list of the available commands.
 
For example, the following steps will download, install, and then reboot the computer to complete the update process:
 
- Open Start.
 - Search for PowerShell, right-click the top result, and select the Run as administrator option.
 - Type the following command to download and install all the available updates and reboot the system, and press Enter:
 - Get-WindowsUpdate -AcceptAll -Install -AutoReboot

 
After completing the steps, Windows 10 will download and install all the available updates, rebooting the computer to apply the changes automatically.
 
Open Start.
 
Type the following command to download and install all the available updates and reboot the system, and press Enter:
 
Get-WindowsUpdate -AcceptAll -Install -AutoReboot
 
### Install specific update command
 
To download and install a specific update on Windows 10 from PowerShell, use these steps:
 
- Open Start.
 - Search for PowerShell, right-click the top result, and select the Run as administrator option.
 - Type the following command to list the available updates along with their KB numbers with PowerShell and press Enter:
 - Get-WindowsUpdate
 - Type the following command to download, install a specific update, reboot the system, and press Enter:
 - Get-WindowsUpdate -Install -KBArticleID 'KB5021233'
 - In the command, replace “KB5021233” with the KB name of the update you want to install.

 
Once you complete the steps, in this case, Windows 10 will download and install update KB5021233 on your device.
 
Type the following command to list the available updates along with their KB numbers with PowerShell and press Enter:
 
Get-WindowsUpdate


 
Type the following command to download, install a specific update, reboot the system, and press Enter:
 
Get-WindowsUpdate -Install -KBArticleID 'KB5021233'
 
In the command, replace “KB5021233” with the KB name of the update you want to install.
 
Windows 10 comes with the Windows Update Provider, but it has limited options compared to the PSWindowsUpdate module, and it’s more complicated to use.




