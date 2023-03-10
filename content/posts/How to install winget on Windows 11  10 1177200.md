---
title: "Revolutionize Your Software Game:  Install Winget on Windows 11 & 10 in 5 Minutes Flat!"
ShowToc: true 
date: "2022-11-26"
author: "James Faux"
---
*****
---
title: "Revolutionize Your Software Game: Install Winget on Windows 11 & 10 in 5 Minutes Flat!"
date: 2021-09-30T14:20:23+05:30
description: "Learn how to install Winget on Windows 11 and 10 in just 5 minutes and take your software game to the next level!"

---

Are you tired of wasting time searching for software for your Windows PC? Do you get frustrated with the lengthy process of downloading and installing software from various sources? Well, there's good news for you! Winget, a new tool from Microsoft, can revolutionize your software game and make the installation of software on your Windows 11 & 10 computer easier and faster than ever before. In this article, you will learn how to install and use Winget in just 5 minutes.

**What is Winget?**

Winget is a command-line tool from Microsoft designed to make downloading, installing, updating, and managing software easier and more convenient. With Winget, you can download and install software from the command prompt, without having to go to a website and manually download the software. Winget connects to a repository of software packages maintained by Microsoft and installs the software quickly and efficiently.

**How to Install Winget on Windows 10 and 11**

Here are the steps to install Winget on your Windows 10 or 11 computer:

1. Open the command prompt: Press the Windows key and type "CMD," or press "Windows Key+R" and type "CMD" in the Run dialog box.

2. Update Windows: Type "winget" in the command prompt and hit enter. If Winget is not installed on your computer, the command prompt will display an error message. In this case, you need to update your Windows by typing "winget install" in the command prompt.

3. Install Winget: Once your Windows is updated, you can install Winget by typing the following command in the command prompt: 

```
PowerShell -Command "& {$H='HKCU:\Software\Microsoft\Windows\CurrentVersion\AppModel\Repository\Enabled'; If(!(Test-Path $H)) {New-Item -ItemType Directory -Path $H | Out-Null}; Set-ItemProperty -Path $H -Name 'value' -Value '1' -Type Dword | Out-Null}"
```

4. Verify Winget installation: Once you have installed Winget, you can verify its installation by typing "winget -v" in the command prompt. This command will display the version of Winget installed on your computer.

**How to Use Winget**

Now that you have installed Winget, you can start using it to download and install software on your computer. Here is an example of how to use Winget:

1. Open command prompt: Type "CMD" in the search bar, and click "Command Prompt" in the search results.

2. Search for software: Type "winget search [software name]" in the command prompt window. Replace [software name] with the name of the software you want to install.

3. Install software: Once you see the software you want to install in the search results, type "winget install [software name]" to install the software.

4. Update software: To update software, type "winget upgrade [software name]" in the command prompt window.

**Conclusion**

Winget is a powerful tool that can revolutionize your software game and take your Windows 11 & 10 experience to the next level. With Winget, you can easily search for, download, install, and update software on your computer without ever leaving the command prompt. By following the steps outlined in this article, you can install Winget and start using it in just 5 minutes. So what are you waiting for? Install Winget today and start enjoying a more convenient software installation experience!

{{< youtube YF6_o_qNGeg >}} 



- To install winget on Windows 11, open the “App Installer” page in the Microsoft Store and click the Update button.
 - Alternatively, open the winget page on GitHub, download the “appxbundle” file, and double-click it to install it.

 
On Windows 11 (and 10), you can install the “Windows Package Manager” (winget) in multiple ways, including from the Microsoft Store and GitHub, or wait until the support arrives automatically.
 
On Windows 10, the “Windows Package Manager” is a command-line tool designed to make it easier and automate the process of searching, downloading, installing, upgrading, and configuring apps on your device.
 
If you have ever had to install one or multiple apps, you know how time-consuming it is to find the links, download, and reinstall all your apps. Using the winget client, you can use a simple command to specify which apps you want to get. Then the tool will find and install the latest version automatically.
 
Microsoft makes the tool available through the Microsoft Store on devices running a supported version of Windows 10 and Windows 11. However, you can get it manually without waiting for the update by installing the latest version of the “App Installer.”
 
If you are already running Windows 10 22H2 or Windows 11 22H2, chances are that the command-line tool is already available. You can check by invoking the winget command in Command Prompt or PowerShell. Otherwise, check for updates first and then continue with the steps below.
 
This guide will teach you how to install the winget-CLI client on Windows 10.
 
- Install winget on Windows 11 from Microsoft Store
 - Install winget on Windows 11 from GitHub

 
## Install winget on Windows 11 from Microsoft Store
 
To install the Windows Package Manager on Windows 11 or 10, use these steps:
 
- Open the App Installer page.
 - Click the Get button.
 - Click the Open Microsoft Store button.
 - Click the Update button.
 - Open Start.
 - Search for Command Prompt and click the top result to open the terminal.
 - Type the following command to confirm the Windows Package Manager is already installed and press Enter:
 - winget

 
Once you complete the steps, the winget-CLI will install on the device, and you can begin searching and installing apps using commands.
 
Open the App Installer page.
 
Click the Get button.
 
Click the Open Microsoft Store button.
 
Click the Update button.
 

 
Open Start.
 
Search for Command Prompt and click the top result to open the terminal.
 
Type the following command to confirm the Windows Package Manager is already installed and press Enter:
 
winget
 
## Install winget on Windows 11 from GitHub
 
To install winget with the offline installer without the Microsoft Store, use these steps:
 
- Open the winget GitHub page.
 - Under the “Latest” section, click the “Microsoft.DesktopAppInstaller_8wekyb3d8bbwe.appxbundle” download link.
 - Double-click the file to launch the winget installer.
 - Click the Update button.

 
After completing the steps, the Windows Package Manager will apply to Windows 11 or 10, and you can start using Command Prompt and PowerShell to install apps.
 
Open the winget GitHub page.
 
Under the “Latest” section, click the “Microsoft.DesktopAppInstaller_8wekyb3d8bbwe.appxbundle” download link.
 
Double-click the file to launch the winget installer.
 
Click the Update button.
 
If you get an error on an older version of Windows 10, you may need to install the VC++ v14 Desktop Framework Package.
 
Alternatively, you can also create your private client application. You can find more details on how to do this process on GitHub.




