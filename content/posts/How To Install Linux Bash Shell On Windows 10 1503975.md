---
title: "Revolutionize Your Computer! Learn How to Install Linux Bash Shell on Windows 10 Today!"
ShowToc: true 
date: "2022-11-18"
author: "Eunice Musick"
---
*****
---
title: "Revolutionize Your Computer! Learn How to Install Linux Bash Shell on Windows 10 Today!"
date: 2021-07-20T20:51:26-04:00
draft: false
---

The Windows 10 operating system has come a long way since its initial release. It is now considered one of the most stable and robust operating systems in the market. However, there is one thing that Windows has always lacked – a powerful command-line shell. The Linux Bash shell, on the other hand, is known for its power and versatility. It is a favorite among developers and system administrators.

Did you know that you can install the Linux Bash shell on your Windows 10 computer? Yes, you read that right! With the Windows Subsystem for Linux (WSL), you can run your favorite Linux applications and tools right from your Windows desktop. Here’s how you can do it:

### Step 1: Enable the Windows Subsystem for Linux

The first thing you need to do is enable the Windows Subsystem for Linux. Here are the steps:

1. Open the Windows Start Menu and type “PowerShell” in the search bar.
2. Right-click on the “Windows PowerShell” option and select “Run as administrator.”
3. In the PowerShell window, type the following command and hit Enter:

   ```powershell
   dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
   ```

4. Wait for the command to complete, and then reboot your computer.

### Step 2: Install a Linux Distribution

Now that you have enabled the Windows Subsystem for Linux, it’s time to install a Linux distribution. There are several distributions available, such as Ubuntu, Debian, and Kali Linux. You can choose the one that best suits your needs.

To install a Linux distribution, follow these steps:

1. Open the Microsoft Store on your Windows 10 computer.
2. Search for the Linux distribution you want to install. For example, type “Ubuntu” in the search bar.
3. Select the Linux distribution and click on the “Get” button.
4. Wait for the installation process to complete.

### Step 3: Launch the Linux Bash Shell

Once you have installed a Linux distribution, you can launch the Linux Bash shell. Here are the steps:

1. Open the Windows Start Menu and type “bash” in the search bar.
2. Select the “Bash on Ubuntu on Windows” option to launch the Linux Bash shell.
3. Wait for the shell to initialize.

Congratulations! You have successfully installed the Linux Bash shell on your Windows 10 computer. You can now run Linux applications and tools directly from your Windows desktop. Here are some of the things you can do with the Linux Bash shell:

- Use the powerful Linux command-line tools, such as grep, awk, and sed, to process text files.
- Install and run web servers, databases, and other server applications.
- Build and compile software using popular programming languages such as Python, Java, and Ruby.
- Use Linux container technologies such as Docker and Kubernetes for application deployment and management.

In conclusion, installing the Linux Bash shell on your Windows 10 computer is a great way to revolutionize the way you work. It gives you access to a powerful command-line shell that is highly versatile and flexible. With the ability to run Linux applications and tools on your Windows desktop, you can take your productivity to the next level. So go ahead and give it a try – you won’t be disappointed!

{{< youtube 1ap3hL-UR9I >}} 



Bash Shell is simply a command-line utility that has been a part of Linux for a very long time and now, Microsoft has directly added it into Windows 10. This is neither a virtual machine nor any container or any software compiled for Windows. Instead, it is a full Windows Subsystem intended for running the Linux software, based on Microsoft’s discontinued Project Astoria for running Android apps on Windows.
 
Now, we all know what a dual-mode operating system is. What will you do if you want to use the Windows operating system and the Linux operating system but your PC is not strong enough to handle the dual-mode operating systems? Does it mean you have to keep two PCs, one with the Windows operating system and another with the Linux operating system? Obviously, not.
 

 
Microsoft has made it possible to use a dual operating system mode without actually having two operating systems in your PC. Microsoft in partnership with Canonical, which is the parent company of Ubuntu, announced that now, you can run RalinkLinuxClient on Windows using a Bash shell i.e. you will be able to perform all the functions of Linux on Windows without having a Linux operating system in your PC.
 
And, with the up-gradation of Windows 10, it has become very easy to get a Bash shell on Windows. Now, this question arises, how to install the Linux Bash shell on Windows 10? In this article, you will get an answer to this.
 
## How to install the Linux Bash shell on Windows 10
 
In order to use the Linux Bash shell on Windows 10, first of all, you have to install the Linux Bash shell on your Windows 10, and before installing the Bash shell, there are some prerequisites.
 
Contents
 
- How to install the Linux Bash shell on Windows 10
 - Alternative: Install Linux distros using Microsoft Store

 
- You must be running the Windows 10 anniversary update on your machine.
 - You must be using the 64-bit version of Windows 10 as the Linux Bash shell does not work on the 32-bit version.

 
Once all the prerequisites are fulfilled, start installing the Linux Bash shell on your Windows 10.
 
To install the Linux Bash shell on Windows 10, follow these steps:
 
1. Open the Settings.
 
2. Click on the Update & Security option.
 
3. Click on the Developer options from the menu at the left panel.
 
4. Under the developer features, click on the Radio button next to Developer mode.
 
Note: Starting with the Fall Creators Update, you don’t need to enable Developer mode. Directly skip to step 9.
 
5. A warning dialogue box will appear asking if you are sure you want to turn on the developer mode. Click on the Yes button.
 
6. It will start installing the Developer Mode package.
 
7. After the installation is finished, you will get a message regarding the developer mode being turned on.
 
8. Restart your PC.
 
Also Read: Fix Bash Syntax Error Near Unexpected Token
 
9. Once your PC is restarted, open the Control Panel.
 
10. Click on Programs.
 
11. Under the Programs and Features, click on Turn Windows features on or off.
 
12. The below dialogue box will appear.
 
13. Check the checkbox next to Windows Subsystem for the Linux option.
 
14. Click on the OK button.
 
15. Changes will start applying. Once the request is completed and the components are installed, you need to restart your PC by clicking on the Restart Now option.
 
16. Once the system restarts, you need to install the Ubuntu distribution for Windows Subsystem for Linux.
 
17. Open Command Prompt (admin) and type the following command and hit Enter:
 
lxrun /install
 
Note: Starting with the Fall Creators Update, you can no longer install or use Ubuntu by using the “bash” command.
 
18. This will successfully install the Ubuntu distribution. Now you just need to set up the Unix username and password (which can be different than your Windows login credential).
 
19. Once finished, you can use the Bash command on Windows by opening the command prompt and using the following command:
 
bash
 
Also Read: Top 14 Best Graphics Card for Linux
 
#### Alternative: Install Linux distros using Microsoft Store
 
1. Open Microsoft Store.
 
2. Now you have the option to install the following Linux distribution:
 
Ubuntu.
OpenSuse Leap
Kali Linux
Debian
Alpine WSL
Suse Linux Enterprise
 
3. Search for any of the above distros of Linux and click on the Install button.
 
4. In this example, we will install Ubuntu. Search for ubuntu then click on the Get (or Install) button.
 
5. Once the installation is complete, click on the Launch button.
 
6. You need to create a username & password for this Linux distribution (which can different than your Windows username & password).
 
7. Now create a new username & password then repeat the password and again press Enter to confirm.
 
8. That’s it, now you can use the Ubuntu distro whenever you want by launching it from the Start Menu.
 
9. Alternatively, you can launch the installed Linux distro by using the wsl command. 
 
As you know, the Linux Bash shell on Windows is not the real Bash shell you find on Linux, so the command line utility has some limitations. These limitations are:
 
- Windows Subsystem for Linux (WSL) is not designed to run the Linux Graphical applications.
 - It will only offer developers a text-based command-line feature to run Bash.
 - Linux applications access the system files and everything that is available on the hard drive so you cannot launch or use the scripts on Windows programs.
 - It also does not support background server software.
 - Not every command-line application works..

 
Microsoft is releasing this feature with a beta label on it, which means that it is still in progress, and not every intended feature is included and sometimes it may not work properly.
 
Recommended:
 
- Fix This Site Has Been Blocked By Your ISP in Windows 10
 - How to Get Among Us on Linux
 - Change Your MAC Address on Windows, Linux or Mac
 - Top 10 Best Kodi Linux Distro

 
But, with the coming times and updates, Microsoft is finding ways to make Linux Bash shell as same as the real Linux Bash shell by focusing on its core functionalities like Bash environment to run tools like awk, sed, and grep, Linux user support, and many more.




