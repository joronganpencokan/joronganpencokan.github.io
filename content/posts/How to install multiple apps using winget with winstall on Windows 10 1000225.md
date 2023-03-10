---
title: "Revolutionize Your Windows 10 Experience: Learn How To Install Multiple Apps Simultaneously with Winget and Winstall!"
ShowToc: true 
date: "2022-11-16"
author: "Doris Nebarez"
---
*****
Revolutionize Your Windows 10 Experience: Learn How To Install Multiple Apps Simultaneously with Winget and Winstall!

Installing applications on your Windows 10 device can sometimes be a daunting task, especially when you have to install multiple apps simultaneously. With the help of Winget and Winstall, you can simplify the process and revolutionize your Windows 10 experience. In this article, we will guide you on how to install multiple apps simultaneously with Winget and Winstall.

What Is Winget?

Winget is a command-line tool that allows you to install, uninstall, and manage applications on Windows 10 devices. It is a package manager that helps you to automate the process of installing multiple applications simultaneously with a single command.

How To Install Winget?

To install Winget on your Windows 10 device, follow these simple steps:

1. Open the Microsoft Store.
2. Search for "winget" in the search bar.
3. Click "Get" to install Winget on your device.

Once Winget is installed, you can proceed to install multiple apps simultaneously with ease.

What Is Winstall?

Winstall is a GUI (Graphical User Interface) frontend for Winget that allows you to install multiple applications simultaneously with a simple click. It is a free and open-source application that simplifies the process of installing applications on Windows 10 devices.

How To Install Winstall?

To install Winstall on your Windows 10 device, follow these simple steps:

1. Open your browser.
2. Search for "Winstall" on GitHub.
3. Click on the "Download" button on the Winstall repository.
4. Extract the downloaded zip file to any directory of your choice.
5. Double-click "Winstall.exe" to launch the Winstall application.

Once Winstall is installed, you can now go ahead and install multiple applications simultaneously with a simple click.

How To Install Multiple Apps Simultaneously With Winget and Winstall?

To install multiple applications simultaneously with Winget and Winstall, follow these simple steps:

1. Open the Winstall application.
2. Click on the "Add" button to add the apps you want to install.
3. Search for the apps you want to install in the search bar.
4. Select the apps you want to install and click the "Add" button.
5. Click on the "Install" button to install all the selected apps simultaneously.

Conclusion

Installing multiple applications on your Windows 10 device can sometimes be a daunting task. But with the help of Winget and Winstall, you can simplify the process and revolutionize your Windows 10 experience. These tools allow you to install, uninstall, and manage applications on your Windows 10 device with ease. We hope this guide has been useful in helping you understand how to install multiple apps simultaneously with Winget and Winstall.

{{< youtube dp-0hVjEo6A >}} 



Microsoft has built a Windows Package Manager (winget) that lets you discover, install, upgrade, remove, and set up one or multiple applications on Windows 10 using command lines.
 
Although using winget to install one app is easy, when you need download and install multiple apps the required command can be complex, and this is when “winstall” comes in handy.
 
winstall is a web app started by Mehedi Hassan on GitHub that connects to the Microsoft’s app repository and allows you to visually select apps you want to install, and it generates a script automatically, which you can then use to bulk install apps on Windows 10 using winget.
 
In this guide, you’ll learn the steps to use winstall to generate a script to install multiple apps using winget on Windows 10.
 
## How to install multiple apps using winstall and winget
 
To install multiple apps using winstall and winget, use these steps:
 
- Open winstall on the web.
 - Click the View All button.
 - Select the apps that you want to install by clicking them twice.
 - winstall select apps
 - Quick tip: You’ll know the item is selected when it has a purple border. You can click the app to deselect it or click the Clear Selections button.
 - Click the Generate script button.
 - winget script
 - Click the Copy to clipboard button.
 - Quick note: The default output is to use winget with Command Prompt, and you must turn on the Show PowerShell script toggle switch to modify the script to use it on PowerShell. Also, you can even download a “.bat” file to automate the installation process on your device.
 - Open Start.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Right-click and paste (Ctrl + V) the winget script to install the apps and press Enter.
 - winget command multiple apps install
 - For example, this script installs Atom, VLC, and 1Password:
 - winget install --id=AgileBits.1Password -e && winget install --id=twinkstar.browser -e && winget install --id=VideoLAN.VLC -e

 
Once you complete the steps, the apps will download and install on your Windows 10 device automatically.
 
Open winstall on the web.
 
Click the View All button.
 
Select the apps that you want to install by clicking them twice.
 
Click the Generate script button.
 
winget script

 
Click the Copy to clipboard button.
 
Open Start.
 
Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 
Right-click and paste (Ctrl + V) the winget script to install the apps and press Enter.
 
For example, this script installs Atom, VLC, and 1Password:
 
winget install --id=AgileBits.1Password -e && winget install --id=twinkstar.browser -e && winget install --id=VideoLAN.VLC -e
 
You can use the Windows Package Manager without administrator privileges, but you’ll be prompted to elevate, and if you choose not to elevate, the installation will fail.
 
The Windows Package Manager still in preview, which means that you’ll need to be part of the Windows Insider Program with a machine enrolled in the Fast ring to access the tool.
 
You may also be able to install a preview of the App Installer on Windows 10 version 2004 from the Microsoft Store.




