---
title: "Revolutionize Your Windows 11 Experience: Install Multiple Apps in Seconds with This Game-Changing Trick!"
ShowToc: true 
date: "2023-06-23"
author: "Alfred Waite"
---
*****
Revolutionize Your Windows 11 Experience: Install Multiple Apps in Seconds with This Game-Changing Trick!

If you're one of the millions of people rocking the latest and greatest operating system from Microsoft, Windows 11, then you'll know that one of the best things about it is its app ecosystem. With the Microsoft Store now fully baked into the OS and third-party options now easily accessible via snap packages, it's easier than ever to discover and install new apps that can improve your daily workflow and make your life that little bit better.

However, for power users and those who are constantly seeking out new tools and applications to try, the entire process of downloading and installing apps can become a bit of a chore. Even if you're using the Windows Store to discover new apps, there's still the issue of having to manually register and sign in to each app, dealing with multiple installation wizards, and dealing with the inevitable restarts and updates that come with new software.

Thankfully, there's a game-changing trick that can help you revolutionize your Windows 11 experience and install multiple apps in seconds - and it's all thanks to a little tool called Windows Package Manager (WPM).

What Is Windows Package Manager?

In a nutshell, Windows Package Manager is a command-line tool that allows you to easily install and manage apps from the Microsoft Store and third-party providers. It's part of the Windows Package Manager Manifest Schema, which is an open-source project that aims to create a standard format for describing packages across different platforms.

With WPM, you can use simple commands in the Windows Terminal to search, install, update, and uninstall apps with ease. And because it's command-line-based, you can easily script and automate the installation of multiple apps at once, simplifying the entire process and saving you precious time and effort.

How to Install Windows Package Manager

Before you can start using WPM, you'll need to install it on your Windows 11 PC. Thankfully, the process is straightforward:

1. First, make sure you have Windows 11 Build 22000.168 or later. If you're running an older version of Windows, you'll need to update your OS first.

2. Next, open the Windows Terminal app. You can do this by pressing the Win + X keys on your keyboard and selecting Windows Terminal.

3. In the Windows Terminal, type in the following command and press Enter:

winget install Microsoft.Windows.PackageManager

4. Wait for the installation to complete. Once finished, you can start using WPM to install apps from the command line.

How to Use Windows Package Manager

Using WPM to install apps is very easy, and you can do it entirely from the command line. Here's a quick overview of the commands you'll need:

1. To search for an app, use the following command:

winget search <app-name>

For example, if you're looking for the VLC media player, type in:

winget search VLC

2. To install an app, use the following command:

winget install <app-name>

Using the VLC example again, type in:

winget install VLC

3. To update an app, use the following command:

winget update <app-name>

For example:

winget update VLC

4. To uninstall an app, use the following command:

winget uninstall <app-name>

For example:

winget uninstall VLC

And that's it! With these simple commands, you can easily search, install, update, and uninstall apps from WPM. But what makes this tool truly game-changing is its ability to install multiple apps at once.

How to Install Multiple Apps with Windows Package Manager

To install multiple apps with WPM, all you need to do is create a list of the apps you want to install and save them as a text file. Then, use the following command to install them:

winget install -i <filename>.txt

For example, if you have a list of apps saved as apps.txt, type in:

winget install -i apps.txt

WPM will then install all the apps listed in the file, one after the other, without any further intervention required.

Conclusion

Windows Package Manager is a game-changing tool that can save you time and effort when it comes to app installation on Windows 11. By using simple command-line commands, you can search, install, update, and uninstall apps with ease. And with its ability to install multiple apps at once, you can streamline the entire process and get back to doing what you do best - using your favorite apps to get things done. So give WPM a try and see how it can revolutionize your Windows 11 experience today!

{{< youtube 9rWvE4Uyh2A >}} 



On Windows 11, you can use the Windows Package Manager (winget) to quickly install multiple apps on your computer.
 
The Windows Package Manager is a tool that allows you to search, install, and update apps on your computer through command lines without having to go through the extra steps of searching online, downloading, and installing multiple apps manually. 
 
In this guide, you will learn the steps to leverage the Windows Package Manager to install multiple apps on Windows 11 quickly.
 
## Install multiple apps using winget on Windows 11
 
To use winget to install multiple apps, use these steps:
 
- Open Start on Windows 11.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to search for the app to install on Windows 11 and press Enter:
 - winget search "APP NAME"
 - In the command, replace “APP NAME” with the name of the app you want to install. The quotation marks are only required when the name has a space, for example, “Visual Studio Code.”
 - Confirm the ID of the app.
 - Repeat steps No. 3 and 4 to find out the ID of all the apps you want to install.
 - Type the following command to build a syntax to install multiple apps with winget on Windows 11 and press Enter:
 - winget install --id=App.1.ID -e && winget install --id=App.2.ID -e && winget install --id=App.3.ID -e
 - In the command, make sure to change the ID for the app you want to install. The “-e” option is optional to match the query exactly, even case-sensitive.
 - For example, this command installs the developer build of Edge, Firefox, and Chrome on Windows 11:
 - winget install --id=Microsoft.Edge.Dev -e && winget install --id=Mozilla.Firefox -e && winget install --id=Google.Chrome.Dev -e

 
Once you complete the steps, the apps will download and install on your computer. Using this command, you can install as many apps as you need.
 
Open Start on Windows 11.
 
Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 
Type the following command to search for the app to install on Windows 11 and press Enter:
 
winget search "APP NAME"
 

 
In the command, replace “APP NAME” with the name of the app you want to install. The quotation marks are only required when the name has a space, for example, “Visual Studio Code.”
 
Confirm the ID of the app.
 
Repeat steps No. 3 and 4 to find out the ID of all the apps you want to install.
 
Type the following command to build a syntax to install multiple apps with winget on Windows 11 and press Enter:
 
winget install --id=App.1.ID -e && winget install --id=App.2.ID -e && winget install --id=App.3.ID -e
 
In the command, make sure to change the ID for the app you want to install. The “-e” option is optional to match the query exactly, even case-sensitive.
 
For example, this command installs the developer build of Edge, Firefox, and Chrome on Windows 11:
 
winget install --id=Microsoft.Edge.Dev -e && winget install --id=Mozilla.Firefox -e && winget install --id=Google.Chrome.Dev -e




