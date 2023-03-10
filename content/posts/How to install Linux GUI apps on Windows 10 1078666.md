---
title: "Revolutionize Your Windows Experience: Learn How to Enjoy Linux GUI Apps on Windows 10 Now!"
ShowToc: true 
date: "2023-05-24"
author: "Gail Schepker"
---
*****
# Revolutionize Your Windows Experience: Learn How to Enjoy Linux GUI Apps on Windows 10 Now!

Are you tired of using the same old Windows apps? Are you in need of a change but don't want to leave your beloved Windows 10 operating system behind? Well, there is a solution that can revolutionize your Windows experience - Linux GUI apps.

That's right, you can now enjoy the best of both worlds by being able to run Linux graphical user interface (GUI) apps seamlessly on your Windows 10 PC. Thanks to Windows Subsystem for Linux (WSL), you can easily install and run Linux GUI apps on Windows with minimal setup.

So how exactly do you get started with running Linux GUI apps on Windows 10? It's quite simple - just follow these steps:

## Step 1: Enable WSL

The first step is to enable WSL on your Windows 10 PC. To do this, open up the Start menu and search for "Turn Windows features on or off". Click on the result that appears and look for "Windows Subsystem for Linux" in the list of features. Check the box next to it and click "OK" to save the changes. 

## Step 2: Install a Linux Distribution

After enabling WSL, you need to install a Linux distribution, such as Ubuntu or Debian. You can do this by opening the Microsoft Store app on your Windows 10 PC and searching for the distribution you want to install. Click on "Get" and wait for the installation to complete.

## Step 3: Install a Linux GUI App

Now that you have a Linux distribution installed, you can install a Linux GUI app. This is where the fun really begins. You can browse through the Linux app store or search for specific apps, such as GIMP (a photo editing app) or LibreOffice (an office productivity suite). Once you've found the app you want to install, open up a terminal (or command prompt) and type in the following command:

`sudo apt-get install <app-name>`

Replace <app-name> with the name of the app you want to install.

## Step 4: Launch the Linux GUI App on Windows

After the app is installed, you can launch it by opening up the Start menu and searching for "Ubuntu" (or whichever Linux distribution you installed). Click on the result that appears and an Ubuntu terminal window will open. Type in the following command:

`<app-name>`

Replace <app-name> with the name of the app you installed in Step 3. 

Voila! Your Linux GUI app should now launch on your Windows 10 PC seamlessly.

## Conclusion

There you have it - a quick and easy guide to revolutionizing your Windows experience by running Linux GUI apps on Windows 10. Not only do you get access to new and exciting apps, but you also get to keep the familiar Windows environment you've grown accustomed to. So why not give it a try and see what Linux GUI apps can do for you?

{{< youtube DooJlOPpNTI >}} 



- Linux GUI apps are installed using the sudo apt-get install command inside the WSL distro.
 - Once the GUI app is installed, you can launch it from the Start menu or use a command.
 - The feature requires installing WSL2 with the wsl --install command on build 21364 or higher.

 
On Windows 10, you can now install Linux GUI apps (almost natively) through Windows Subsystem for Linux (WSL), and these instructions will show you how.
 
Although you could run Linux apps on Windows 10 with WSL for a long time, the system was limited to command-line tools and applications. However, starting with build 21364 and higher releases (with a special update to the WSL integration), Microsoft is finally bringing GUI (graphical user interface) support to run your favorite Linux applications with the mouse and keyboard.
 
The new feature is to develop and test your applications on Linux without needing a virtual machine, but you can use it for anything. The implementation even includes support for speakers and microphones, so if you install a media app, the peripherals will pass through and appear in the app. GPU accelerated 3D graphics are also supported to run any app that needs to do complex 3D rendering leveraging OpenGL.
 
When using this feature, there is no need to start an X server manually since WSL automatically starts a “companion system distro,” which includes a Wayland, X server, pulse audio server, and all the required components. Then after you close the app and the WSL session, the system distro will end automatically.
 
This guide will teach you the steps to download and install graphical Linux applications on Windows 10. You can also watch this video tutorial with the step-by-step to complete this process.
 
- Install Linux GUI apps via WSL on Windows 10
 - Install or update WSL on Windows 10

 
## Install Linux GUI apps via WSL on Windows 10
 
To install a Linux GUI app on Windows 10, use these steps:
 
- Open Start on Windows 10.
 - Search for Ubuntu (or another distro) and click the top result to open the Linux distro.
 - Type the following command to update the package distribution and press Enter:
 - sudo apt-get update
 - Type the following command to install a Linux GUI app on Windows 10 and press Enter:
 - sudo apt-get install APP-NAME -y
 - In the command, replace APP-NAME with the graphical app you want to install.
 - This example installs the gedit text editor app:
 - sudo apt-get install gedit -y
 - Confirm your Linux account password and press Enter (if applicable).

 
Once you complete the steps, the app will install and register in the Start menu, which means that you can launch the app by running the app’s name in the Windows Subsystem for Linux (WSL) console or from the Start menu.
 
Open Start on Windows 10.
 
Search for Ubuntu (or another distro) and click the top result to open the Linux distro.
 
Type the following command to update the package distribution and press Enter:
 
sudo apt-get update
 
Type the following command to install a Linux GUI app on Windows 10 and press Enter:
 
sudo apt-get install APP-NAME -y
 
In the command, replace APP-NAME with the graphical app you want to install. 
 
This example installs the gedit text editor app:
 
sudo apt-get install gedit -y
 

 
Confirm your Linux account password and press Enter (if applicable).
 
The above instructions outline the steps to install a simple app from known repositories, but depending on the app, the instructions may differ. The good news is that the installation process is the same as any other Linux application. You can follow the developer steps to install virtually any application, such as VLC, Audacity, web admin, etc.
 
If you launch the Linux GUI app from the Windows 10 Start menu, you will find the entries in the “Recently added” list, or you can also find them inside the (distro name) folder below the Linux distro entry.
 
As you launch the app, the virtual machine will spin, and it will run (in a few seconds) without needing to open the WSL console. You will also notice that the taskbar will show the icon with a Linux logo, indicating that you are not running a Windows 10 application.
 
The experience of using a graphical Linux app on Windows 10 feels native, but it’s not. The app renders with all the Linux visual styles for the frame, menus, and other elements, and there is even a shadow around the edge, and every window works independently.
 
However, it is a remote desktop connection, which Microsoft is leveraging with the RemoteApp feature built into the operating system.
 
## Install or update WSL on Windows 10
 
The ability to run Linux GUI apps requires the Windows Subsystem for Linux 2 integration, which means you must have the latest feature and distribution version to install and run your applications.
 
If you have WSL2 already installed, then you will need to update the feature.
 
Before installing or updating WSL2, the device must have the Windows 10 build 21364 or higher release.
 
Also, as a prerequisite, you must install the driver to enable a virtual GPU (vGPU) to use hardware-accelerated OpenGL rendering before installing applications. Here are the download links:
 
- NVIDIA GPU driver.
 - Intel GPU driver.
 - AMD GPU driver.

 
### Install WSL2 on Windows 10
 
These instructions will show you how to install WSL2 and the Ubuntu Linux distribution to get started running GUI apps.
 
To install WSL2 components to run Linux GUI apps, use these steps:
 
- Open Start.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to install the WSL 2 and press Enter:
 - wsl --install

 
Once you complete the steps, the required Linux components will install automatically, and the command will also download the latest version of the Ubuntu Linux distro.
 
Open Start.
 
Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 
Type the following command to install the WSL 2 and press Enter:
 
wsl --install
 
After the installation, you only need to open the distro from the Start menu and continue with the on-screen directions to complete the setup.
 
You can use these instructions if you want to install a different distro to run apps instead of Ubuntu.
 
### Update WSL2 on Windows 10
 
If you already have the Windows Subsystem for Linux 2 installed, confirm the system has the latest updates to run GUI apps.
 
To update WSL2 to download the GUI support for Linux apps, use these steps:
 
- Open Start.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to update the Windows Subsystem for Linux 2 and press Enter:
 - wsl --update
 - Type the following command to force restart WSL2 and press Enter:
 - wsl --shutdown

 
After you complete the steps, the latest version of WSL will download automatically. Then you can use the above instructions to install Linux GUI apps.
 
Type the following command to update the Windows Subsystem for Linux 2 and press Enter:
 
wsl --update
 
Type the following command to force restart WSL2 and press Enter:
 
wsl --shutdown




