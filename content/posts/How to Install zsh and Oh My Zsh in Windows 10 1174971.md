---
title: "Revolutionize Your Windows 10 Experience with These Easy Steps to Install Zsh and Oh My Zsh!"
ShowToc: true 
date: "2023-01-14"
author: "Waldo Rutledge"
---
*****
# Revolutionize Your Windows 10 Experience with These Easy Steps to Install Zsh and Oh My Zsh!

Are you tired of the traditional Windows 10 command prompt and looking to elevate your user experience by using a powerful terminal emulator? Look no further, as we introduce Zsh and Oh My Zsh, both of which can revolutionize your Windows 10 experience in no time! 

## What is Zsh?

Zsh is a Unix shell that comes packed with more features than the traditional Windows command prompt. Some of its features include advanced command history, stunning theme support, and intelligent completion. 

## What is Oh My Zsh?

Oh My Zsh is a community-driven framework for managing the Zsh configuration. It comes with its own set of plugins, themes, and various features. With Oh My Zsh, you can create your custom command prompts with ease, using different plugins for git, web development, and many more. 

## How to Install Zsh and Oh My Zsh in Windows 10

Installing both Zsh and Oh My Zsh on your Windows 10 machine is straightforward. Follow these simple steps carefully, and you'll be up and running in no time. 

### Step 1: Install the WSL

To begin, ensure that the Windows subsystem for Linux (WSL) is installed on your Windows machine. The WSL is a feature that allows you to run Linux commands on your Windows machine. To install the WSL, follow these steps: 

- Press `Windows Key + X` and select `PowerShell (Admin)`
- Type the following command: 
   ```
   Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
   ```
- Press `Enter` and restart your computer.

### Step 2: Install Ubuntu

With the WSL enabled, the next step is to install Ubuntu. Ubuntu is a popular Linux distro to use with the Windows subsystem. To install Ubuntu, follow these steps:

- Open the Microsoft Store app on your Windows 10 machine.
- Type "Ubuntu" in the search field.
- Click "Install." 

### Step 3: Install Zsh

After installing Ubuntu, the next step is to install Zsh. In the Ubuntu command prompt, type these commands to install Zsh:

- `sudo apt-get update`
- `sudo apt-get install zsh`

### Step 4: Install Oh My Zsh

The final step is to install Oh My Zsh. In the Ubuntu command prompt, type this command to install Oh My Zsh:

- `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

## How to Access Zsh in Windows 10

After installing Zsh and Oh My Zsh, you can access the new terminal by following these simple steps:

- Open a command prompt
- Type `bash`
- Press `Enter`

The Zsh terminal will appear, and you can start customizing your terminal with your chosen theme and plugins. 

## Conclusion

Revolutionizing your Windows 10 experience with Zsh and Oh My Zsh is easy and quick. Follow the above steps to make your terminal smarter, efficient, and aesthetically pleasing. Say goodbye to the traditional command prompt and welcome the new, fresh Windows experience.

{{< youtube 8Ndp5DGr4HA >}} 



If you’re coming to Windows from macOS or Linux, you might miss the powerful functionality of the UNIX command line or “shell.” Windows doesn’t ship with the UNIX shell enabled by default, but you can easily get a shell running on Windows and even extend the shell’s power with zsh.
 
## What Is zsh?
 
zsh, also called the “Z-shell,” is a more powerful version of Bash, the standard shell that ships on Linux and macOS systems. zsh allows users to extend the appearance and functionality of their shell with scripts, plugins and more. There’s a wide community of developers that have made amazingly useful plugins for zsh, and you can code your own extensions and plugins as well. If you spend a lot of time on the terminal, it’s a great way to improve your quality of life.
 
## Turning on Bash
 
Before we can install zsh or Oh My Zsh, we need to first enable the default shell called Bash. This used to require third-party programs like Cygwin, and you can still do it that way. However, Windows 10 now ships with a Linux subsystem that’s turned off by default. If we turn it on, we’ll be able to run Bash on Windows using native software packages.
 
1. Open Settings and click on “Updates & Security.”
 

 
2. Click “For developers” in the sidebar, then click the radio button next to “Developer mode.”
 
3. In the pop-up window, click “Yes” to proceed with enabling developer mode.
 
4. Open Control Panel and navigate to the “Programs and Features” menu.
 
5. Click “Turn Windows features on or off” in the sidebar.
 
6. Scroll down and tick the checkbox next to “Windows Subsystem for Linux (Beta)” to enable the Linux subsystem. Then click the “OK” button.
 
7. Wait for the installer to finish.
 
8. When the installer is finished, click “Restart Now” to restart your computer and complete the installation.
 
9. After you’ve restarted your computer, type “bash” into the Start Menu and launch the bash script.
 
10. This will open a command prompt and finish installing UNIX and Bash. Type the “y” key and press “Enter” to confirm installation of the remaining components.
 
11. Wait while the remaining components are downloaded and configured.
 
12. When prompted, create a username for Bash and UNIX.
 
13. Enter a password you’ll use for Bash and UNIX. You won’t see any characters appear as you type, but they are being saved. Press “Enter.”
 
14. When the installation is finished, you’ll be returned to the command prompt. You can now close this window.
 
## Installing zsh on Windows 10
 
Now that we have a shell on Windows, our next step is to install zsh. We’ll use the “apt-get” package manager to download and install it.
 
1. Open Bash from the Start Menu.
 
2. Type the following command into the command prompt and press “Enter:”
 
3. Enter your Bash/UNIX password when prompted and press “Enter.”
 
4. When prompted, type “Y” and press “Enter” to continue the installation.
 
5. When the installation is complete, you’ll be returned to the command prompt.
 
## Using zsh on Windows 10
 
Now that we’ve installed zsh, we can start using it.
 
2. Type zsh and press “Enter.”
 
3. On first run, you’ll need to go through some zsh configuration options. There’s a bunch there, but we recommend actually looking at all the information and choosing the options you like. If you’re not sure what to choose, you can just press the “2” key to accept the default configuration.
 
4. When the configuration is complete, you’ll be returned to the zsh command prompt.
 
## Installing Oh My Zsh on Windows 10
 
Now that we have zsh installed, we can install Oh My Zsh. If you’re not familiar with Oh My Zsh, the developer says it best: “Oh-My-Zsh is an open source, community-driven framework for managing your zsh configuration.” It also ships with more than 200 plugins and 140 themes for zsh, extending functionality and making your command line easier to customize.
 
1. Open Bash from the Start Menu.
 
2. Use the following command to download and install git, a prerequisite for installing Oh My Zsh:
 
3. Once git is installed, we can download and install Oh My Zsh. To do so, copy and paste the following command into your command line and press “Enter.”
 
Note that you can quickly paste into the zsh command line by selecting the Xsh window and right-clicking.
 
4. Enter your Bash/UNIX password when prompted and press “Enter.”
 
5. When the installation is finished, you’ll see Oh My Zsh’s ASCII art.
 
## Conclusion
 
Once you’ve installed zsh and Oh My Zsh, you can use them both just as you would on a UNIX system. If you want to learn more, you can check out zsh’s online user guide and Oh My Zsh’s wikis.
 
Alexander Fox is a tech and science writer based in Philadelphia, PA with one cat, three Macs and more USB cables than he could ever use.
 
Our latest tutorials delivered straight to your inbox




