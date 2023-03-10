---
title: "Unlock the Power of Linux on Your Windows Machine - Learn How to Install Linux with WSL Now!"
ShowToc: true 
date: "2022-11-18"
author: "Sean Stephens"
---
*****
# Unlock the Power of Linux on Your Windows Machine - Learn How to Install Linux With WSL Now!

Are you looking for a way to unleash the power of Linux on your Windows machine? Then look no further than Windows Subsystem for Linux (WSL).

WSL is a powerful tool that allows you to run your favorite Linux distributions alongside your Windows operating system. It’s a groundbreaking feature that’s easy to install and use, and it’s revolutionizing the way developers and IT professionals use their machines.

In this article, we’ll show you how to install Linux with WSL so you can start using the open-source operating system on your Windows machine today.

## What is WSL?

WSL is a feature that allows you to run Linux distributions natively on Windows 10. It’s not a virtual machine or an emulator. WSL integrates the Linux kernel into Windows, meaning you can run Linux applications alongside your Windows applications without the need for dual-boot or virtualization.

WSL supports most Linux distributions, including Ubuntu, Debian, and Kali Linux. By running Linux within Windows, you can streamline your workflow and take advantage of the extensive Linux developer and IT toolset, all while maintaining the familiar Windows environment.

## How to Install Linux with WSL

Installing Linux on your Windows 10 machine with WSL is a quick and straightforward process. Follow these simple steps, and you’ll be running Linux in no time.

### Step 1: Enable WSL in Windows 10

Before you can install Linux with WSL, you need to enable the feature on your Windows machine. Here’s how to do it:

1. Open the **Control Panel** from the Start menu.
2. Click **Programs**.
3. Under **Programs and Features**, click **Turn Windows features on or off**.
4. Scroll down to **Windows Subsystem for Linux** and click the checkbox to enable the feature.
5. Click **OK** and restart your computer. 

### Step 2: Install a Linux Distribution on WSL

Once you’ve enabled WSL on your machine, the next step is to install your chosen Linux distribution.

1. Open the Microsoft Store from the Start menu.
2. Search for your preferred Linux distribution, such as Ubuntu or Debian.
3. Click on the distribution and click **Install**.
4. Once the installation is complete, you’ll see the distribution listed as an installed app.

### Step 3: Launch Your Linux Distribution

Now that you’ve installed your Linux distribution, it’s time to launch it and start using Linux on your Windows machine.

1. Open your Start menu and type the name of your Linux distribution.
2. Click on the Linux distribution to launch it.
3. The Linux distribution will open in a command-line interface. You can begin using Linux right away, using familiar Linux commands and tools.

## Conclusion

With WSL installed on your Windows machine, you can take advantage of the vast array of Linux tools and applications without the need for a separate machine or virtualization. By following the simple steps outlined in this article, you can install Linux with WSL and unlock the full power of open-source computing on your Windows machine.

So why wait? Get started on your Linux journey today and start exploring all the possibilities of open-source computing.

{{< youtube j_fd0SApJD0 >}} 



For a full Linux experience, there’s no substitute for a full install. But if you’re a Windows user wishing to install Linux, Windows Subsystem for Linux (WSL) is a great place to start. Getting a Linux distro up and running on your Windows machine is pretty easy, whether you’re just learning Linux or want to use a Linux development environment, so it’s worth a shot if you’re at all curious. Here you’ll learn how to install Linux on Windows with WSL.
 
## What Is Windows Subsystem for Linux (WSL)?
 
Windows Subsystem for Linux (WSL) is an installable feature in Windows that lets you run a Microsoft Store-supported Linux distro on a Windows 10 or Windows 11 device. Microsoft has partnered with Canonical (the publisher of Ubuntu) to bring its bash command line capabilities to a typical Windows desktop so that you can integrate both Linux and Windows into your workflow.
 
WSL supports Linux file systems using commands for Bash but cannot offer a full Linux desktop experience, which is only possible with a virtual machine or dual-boot procedure. From Windows 11 onward, WSL supports native Linux GUI applications, such as Gedit, GIMP, and Nautilus in conjunction with Bash.
 
To a Linux user who likes using the command line tools, WSL feels very natural and normal. It’s quite useful for Windows developers, too, who want to deploy Windows applications to Linux server environments.
 
## Linux Distros That Work with WSL 
 
To work with your favorite Linux distro in WSL, first ensure it can be downloaded from the Microsoft Store. Supported examples include:
 
- UbuntuDebianKali LinuxSUSE Linux Enterprise Server  Fedora Remix for WSL (Paid version)openSUSE LeapAlpine Linux

 
## WSL Benefits: What You’ll Get
 
The following are the main benefits of using WSL on your Windows device:
 
- Having Linux on top of Windows: you’ll end up with a Linux virtual machine you can run on Windows. You can have any of your favorite distro installed and running at the same time. Run Linux apps as standalone Windows applications: whether you want to launch Linux apps from the Windows Start menu or pin them to the Windows taskbar, WSL lets you access them from your Windows desktop.Switch between Windows and Linux: you can switch quickly between Linux and Windows and, perhaps most importantly, access your Windows files and programs from inside the Linux shell. WSL is perhaps the only software that allows Cut and Paste across Windows and Linux apps.Support for cross-platform languages and services: with WSL in place, you can run advanced programs between two integrated operating systems. These include vim, emacs, NodeJS, Python, Ruby, C/C++, Rust, Go, MySQL, Apache, and MongodB.Supports Windows applications for Linux user habits: are you a frequent Linux user? Now you can bring your favorite Linux commands to a Windows desktop without having to deal with its user interface. Whether you want to edit a Word file or run Notepad++, you can easily do it the Linux way.

 
On the other hand, if you’re a Windows user who has never used Linux before, you’ll need to learn some basic Linux commands to get started. Don’t worry. There aren’t too many of them for a Windows user’s needs.
 
## Installing and Setting Up WSL in Windows 10
 
You’ll need to be running an up-to-date version of Windows 10 for this to work, but that’s just about the only requirement apart from knowing how to use Windows PowerShell or Command Prompt.
 
The instructions below will set you up with the most recent version of Windows Subsystem for Linux (WSL2, Build 21354 as of September 2021).
 
- On your Windows 10 device, search for a Control Panel feature called “turn Windows features on or off.”

 
- When the Windows Features menu screen opens, check the options for “Windows Subsystem for Linux” and “Windows PowerShell.”

 
- Open PowerShell or (Command Line). Make sure you run it as an administrator.Paste in the following script:

 
- If it prompts you to restart, do so; otherwise, move on.Open the Microsoft Store and search for “Linux” to see all your available options. Here, we are installing Ubuntu.

 
- Click the “Install” button from within the Store app. It will download your desired Linux distro.

 
- You will get a notification once the Linux distro has been installed on your Windows 10 desktop. In the future, you can open this directly from your Start Menu.

 
- Once the Linux bash window opens, choose a username. It doesn’t have to be the same as your Windows login.

 
- Enter a password and retype it.

 
Note: the password is invisible, so make sure you store it in a safe place. If you forget your password, you’ll have to uninstall the Linux distro, which will delete all your Linux files.
 
- Update your installation using:

 
- Wait for the updates to complete, then check for any upgradable versions in your Linux distro using:

 
- Once you find all the available upgrades, enter the following to ensure all of them are applied to your system:

 
- The updates take some time, as templates are extracted from Linux packages, followed by a pre-configuration and the settings being applied. Be patient as this process is automatic.

 
- If you want to install any specific Ubuntu packages, such as npm, groovy, impish, or hirsuit, you can use:

 
- Wait for the updates to finish, when the  green progress bar goes all the way to 100 percent. If there are any errors due to your PC misconfiguration, the progress bar will turn red and suggest remedial actions.

 
## Using WSL with Windows  
 
If you want, you can use your Linux installation as its own system on Windows, with totally separate files and programs. You may want some files stored on Linux for its speed advantages, but one of the big perks of WSL is that you can interact with your Windows files and folders by effectively mounting the drive to your Linux system. This enables you to use Linux with anything you have on Windows, thus keeping all your stuff in the same place.
 
Now that you’ve learned how to install Linux using WSL on your Windows 10 device, it’s time to familiarize yourself with its basic commands.
 
### Basic Linux Commands
 
If you’re familiar with Linux command line navigation, you can skip down a little bit. Otherwise, the following are some basic commands you’ll need to know to move around in a Linux command line.
 
Using Linux commands in a Windows shell like PowerShell or command prompt is easy. Just use:
 
- For example, here’s the command for “print working directory,” which shows you the path of the current directory from the root.

 
- If you want to list all the contents of your current directory using the Linux command, just enter:

 
This will execute the Linux command on Windows without opening the actual operating system.
 
- Sometimes you will need to create directories in Linux. For that, use:

 
- To change the default path file to your newly created directory, use:

 
Check the below screenshot to see all the above highlighted commands in action.
 
- If you want to start the entire operating system from inside PowerShell or Command Prompt, that’s also easy. Just run:

 
or
 
Eventually, though, you’ll probably wonder how to access Windows directories from inside your Linux system itself. The key here is that Windows is essentially mounted as an external drive to the Linux system, so Linux can use it as storage, making it pretty much the same as using your OS to edit files on a flash drive.
 
- Open your Linux terminal (Ubuntu, in this case) as a Windows administrator.

 
- Access your Windows C: drive by entering:

 
- To see some editing in action, create a folder using:

 
- Open File Explorer and check your C: drive to confirm that Ubuntu created a folder there.

 
- Go down to the directory path by typing:

 
- Create a file using:

 
- Check that the newly created text file is available in the chosen directory.

 
- To edit the file, use:

 
- To test, add any dummy text in the command screen. This will add changes to the bash-created file.

 
Enter a few words, then press Ctrl + O to save and Ctrl + X to exit.
 
- Check your Windows file system again. You should see a text file with the content you entered.

 
If you’d like, you can navigate to any other folder or document on your Windows drive and edit it using Ubuntu.
 
- Let’s say you want to access your Linux files in Windows or maybe just want a GUI representation of your filesystem. Navigate to the Linux directory you want to see and enter:

 
The . at the end stands for the current directory, and if you include it, explorer.exe will launch a Windows Explorer window that shows your Linux files.
 
- You can actually launch other Windows apps and run Windows commands from Linux as well. For example:

 
launches Notepad.
 
## Run Linux GUI Apps in Windows 11
 
So far we’ve seen how to run Linux with the command line in Windows 10. From Windows 11 onward, it is now possible to have a limited GUI experience on Windows Subsystem for Linux (WSL). 
 
You have to at least be on a Windows 11 build 22000 or higher to enjoy the GUI apps for Ubuntu or any other supported distro package.
 
- Upgrade from Windows 10 to Windows 11 by following the steps listed in this guide.On your Windows 11 device, go to PowerShell in Administrator mode. To install Ubuntu, enter the following:

 
- You may also want to update the WSL on your device using

 
- Wait for the distro download to complete. To work with the changes, reboot the system once.

 
- After the restart, the feature updates will take effect, and the new distro will be installed on your Windows 11 device. It will automatically launch from here.

 
- Once the target distro has been launched in Windows 11 bash window, you can install any GUI apps such as Gedit, which is a text editor.

 
- After the GUI app gedit is installed, you can launch it using:

 
We have seen how to install and launch GUI apps in your Linux Bash terminal. If you know the relevant Linux commands, you can start trying them out in Windows. 
 
## Frequently Asked Questions
 
### 1. How do I uninstall WSL or Linux distros from my Windows PC?
 
You can uninstall WSL and its distros using PowerShell/Command line or from “Add or remove programs” in Windows 10/“Apps and Features” in Windows 11. 
 
To uninstall any configured Linux distro using PowerShell in a Windows PC, use the following command in Admin mode:
 
To verify that the distro has been uninstalled, use:
 
To differentiate WSL from PowerShell, enter the following which will give a list of installed applications. You can further use wsl –- help to be guided toward the uninstallation.
 
Of course, the easier way to uninstall WSL is to access it in your list of apps and click the Uninstall button. The following screen is for Windows 11.
 
### 2. Where are my WSL files stored on a Windows device?
 
To access WSL files on a Windows 10/11 device for any installed distro, search for the %LOCALAPPDATA% hidden folder in C drive.
 
### 3. Is Windows Linux Subsystem safe to use?
 
Yes. The host Windows system always has full control over the guest Linux subsystem. As long as you have enabled security features in Windows with Windows Defender and corrected the Setting errors in Defender file, your virtual Linux subsystem is safe to use.
 
## What Else Can You Do?
 
Now that you know how to install Linux on Windows 10 and 11 and how it interacts with Windows, you can do just about whatever you want. You can run programming languages, run local servers, use a Windows IDE to work in the Linux shell, run multiple Linux distros at the same time, or just play around with Linux to get comfortable with the command line. The price of failure is pretty low. If you mess something up, resetting or reinstalling your Linux distro is pretty easy.
 
To work with bash prompts, check the best options available. While you’re running a Linux subsystem on Windows, check out some of the best Linux games to play on your Windows PC.
 
Sayak Boral is a technology writer with over eleven years of experience working in different industries including semiconductors, IoT, enterprise IT, telecommunications OSS/BSS, and network security.  He has been writing for MakeTechEasier on a wide range of technical topics including Windows, Android, Internet, Hardware Guides, Browsers, Software Tools, and Product Reviews.
 
Our latest tutorials delivered straight to your inbox




