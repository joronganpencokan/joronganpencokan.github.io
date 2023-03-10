---
title: "Revolutionize Your M1 Mac: Learn How to Install Asahi Linux in 5 Simple Steps!"
ShowToc: true 
date: "2022-12-13"
author: "Irving Paladino"
---
*****
Revolutionize Your M1 Mac: Learn How to Install Asahi Linux in 5 Simple Steps!

The Apple M1, Apple's first-ever custom-designed system-on-a-chip for Mac, received a lot of buzzes since its launch in November 2020. The M1 chip packs a punch when it comes to speed, power efficiency, and graphics performance. The chip also integrates various cutting-edge technologies, including a custom-designed CPU, GPU, and the Neural Engine. With the M1 chip, Apple has set a new standard in Mac performance and power efficiency. 

However, like any new technology, there are some limitations to the M1 Mac. For example, some users may find the current macOS operating system limiting, or they may need to run Linux-based software or development tools. Luckily, with Asahi Linux, an open-source effort to port Linux to the Apple Silicon platform, you can revolutionize your M1 Mac experience. Here's how you can install Asahi Linux in five simple steps:

Step 1: Check Your M1 Mac's Compatibility

The first step in installing Asahi Linux on your M1 Mac is to check the compatibility of your Mac. To do this, you need to ensure that your Mac's firmware is compatible with Asahi Linux. You can check your firmware version by going to the Apple logo menu > About This Mac > System Report > Software > Firmware Version. 

Step 2: Create A Bootable USB Drive

Next, you need to create a bootable USB drive to install Asahi Linux on your Mac. To do this, download the Asahi Linux installer from the project's website and follow the instructions to create a bootable USB drive. 

Step 3: Boot Your M1 Mac Into Recovery Mode

Once you've created your bootable USB drive, you need to boot your M1 Mac into recovery mode. To do this, turn off your Mac and hold down the power button until the startup options window appears. 

Step 4: Install Asahi Linux Using The Terminal

With your M1 Mac in recovery mode, you can now install Asahi Linux using the Terminal. To do this, follow the instructions provided by the installer on how to run the installation commands. Once the installation is complete, your Mac will boot into Asahi Linux. 

Step 5: Configure and Enjoy Your Asahi Linux M1 Mac

Congratulations! You've successfully installed Asahi Linux on your M1 Mac. You can now enjoy the full benefits of Linux on your Mac, including running Linux-based software and development tools. But before you start using your Asahi Linux M1 Mac, take some time to configure it to your liking by following the instructions provided by the project's documentation. 

In Conclusion 

Asahi Linux is a fantastic open-source project that allows you to run Linux on Apple Silicon devices. By following the five simple steps outlined in this article, you can revolutionize your M1 Mac experience and enjoy Linux on your Mac. Whether you're a developer or a Linux enthusiast, Asahi Linux is worth exploring. So why not give it a try today?

{{< youtube SoszrV0TG3U >}} 



While M1 Macs are great, they cannot run a Linux distro natively until recently. Asahi Linux, an Arch-based distro, is the first Linux distro specially made for M1 machines, and you can run it natively on Macs with the M1, M1 Pro, and M1 Max chips. Moreover, you can dual boot Asahi Linux to use it without replacing your macOS. In this tutorial, we cover everything, including how to download, install, and even uninstall Asahi Linux.
 
## Before You Start
 
Asahi Linux is still in its Alpha release. As of now, you can’t run it on Mac Studio. Some of the features, like DisplayPort, GPU acceleration, and Touch Bar (for 13” MacBook Pro), don’t work yet.
 
You can get the complete list of “What doesn’t” work on the official announcement page. Although, in my usage, I found that Bluetooth works just fine, but the official announcement page said it is not working.
 
## Installing Asahi Linux
 
Asahi Linux has a self-explanatory installer. As long as you understand and answer the on-screen prompts, you are good to go.
 
Note: make sure to keep a backup of your important data before starting the installation process.
 
- To install Asahi Linux, open the terminal on your macOS and run:

 
This will download and execute the shell script to install Asahi Linux. 
 
- Enter your sudo password when prompted. (Your sudo password is your Mac’s user password.) The terminal will prompt you to make sure that you have read the documentation. Press Enter to continue.A prompt will ask you if you want to enable expert mode or not. You can choose either one. In my case, I am pressing N and Enter to continue with the normal mode. This will show you your username and the basic information about the partitions.

 
### Resizing Your macOS Partition
 
- When it asks you to “Choose what to do,” press r and Enter to resize your existing partition and make space for the Linux distro.

 
- A prompt will ask you to set a new size for your macOS. You can use a percentage, storage size, or enter min (which will shrink your macOS to the minimum possible size). For example, you can enter 70% to set your macOS size to 70% of the total space. I am entering “230GB” to make my macOS shrink to 230GB.

 
You will see how much space you will have freed up after resizing.  Press y and Enter to continue and start resizing your partition.
 
- Press Enter when the resizing is completed.

 
### Installing Asahi Linux on the New Partition
 
- When prompted with “Choose what to do” again, press f and Enter to install the Asahi Linux in the free space.

 
- You will see the prompt “Choose an OS to install.” Choose the one that suits you best. I am choosing “1” to install Asahi Linux with all the preinstalled apps. Type your chosen number and press Enter.

 
- You will be prompted with the question “How much space should be allocated to the new OS?” As before, you can enter a storage size or percentage of the free space. Entering min and max will allocate the minimum and maximum possible space for the Linux distro. I am entering “max” to allocate all the free space to Asahi Linux. Enter a name for your OS, press Enter and the script will download and set up everything for you. If it asks for the admin credentials, enter your macOS user password.

 
- When everything is configured, you will be asked to press Enter to read the instructions. Read the instructions carefully, which are crucial for successfully booting into Asahi Linux.

 
- Press Enter to shut down your Mac.

 
- Wait 15 seconds for the system to fully shut down, then press and hold your power button until you see “Entering startup options” or a spinner.

 
- You will see a list of volumes on the startup options. Select the volume with your previously-set OS name and select “Continue.”

 
- This will boot into the macOS Recovery screen. On the recovery screen, select your username, click “Next” and enter your macOS user password to open a terminal window.

 
- On the terminal, press Enter to continue the installation process.

 
- You will be asked to enter the password for your username. Use the same username and password if you are prompted again.

 
- Press y and Enter if you are asked whether you want to continue.

 
- Press Enter to reboot, then select Arch Linux from the grub menu to boot into Asahi Linux.

 
### Completing Asahi Linux Setup Screen
 
- Once you boot into Asahi Linux, you will see a setup page for Asahi Linux. Set your language, region, time zone, and keyboard layout as you would do with any other Linux distro.

 
- Enter a username, computer name, and password (These can be different from your macOS credentials) and press “Next.”

 
- On the summary screen, press “Set up” to finish the setup. Press “Done” on the Finish screen, which will take you to the login screen.

 
- Use your previously-set password to log in.

 
## Installing Packages on Asahi Linux
 
You can use pacman to install any package for arm64 architecture from official Arch Linux repositories. Learn all about pacman here.
 
For example, to install node.js, run:
 
and press Y and Enter to confirm.
 
You can also build a package from the source and install it if you want to. 
 
## Using macOS and Asahi Linux Together
 
Asahi Linux is made to run alongside your macOS. However, when you turn your Mac on, it will boot by default into Asahi Linux. To boot into macOS, press and hold your power button until you see “Entering startup options” or a spinner, then select Macintosh HD and press “Continue.”
 
## Uninstalling Asahi Linux
 
You can uninstall Asahi Linux by deleting the partitions for Asahi Linux. 
 
- Run diskutil list in your macOS terminal and copy the volume identifier from the line with “EFI” and your Linux OS’s name in it.

 
In my case, the line is “EFI EFI – MINIX,” and the identifier is “disk0s4.”
 
- To delete the volume, run:

 
Make sure to replace “YourDiskIdentifier” with the actual disk identifier.
 
- Now open the Disk Utility app. Select “Partition” from the top border and delete the first three consecutive partitions at the end of your Macintosh HD partition.

 
To delete a partition, select the partition and press the “–” button. Make sure to delete the correct partitions. The first partition’s name will be your Linux OS’s name. The second partition is named “drive,” which is around 500MB. The third partition is the partition for Asahi Linux’s home directory, which will display the home directory’s size of Asahi Linux. (It will be closer to the size of your total allocated storage for Asahi Linux.)
 
Click “Apply” to apply the changes you just made to your partitions.
 
This will open a new window with the partition names you are going to delete. Select “Partition.”
 
It will take some time, and your Mac may temporarily appear to be frozen, which is totally normal.
 
Select “Done” when the process completes. 
 
### Fixing the Boot Screen
 
- Now that you are done with Disk Utility, restart your Mac. On the boot screen, you will see a “Custom kernel failed to boot” warning. Select “Startup disk.”

 
- On the next screen, select “Macintosh HD” and click “Restart.”

 
Your Mac will continue to start as usual.
 
## Frequently Asked Questions
 
### Do I need a USB drive to install Asahi Linux?
 
No. You can complete the installation process without using any external USB drive.
 
### Can I install x86 architecture-based packages on Asahi Linux?
 
No. Asahi Linux is an Arm architecture-based distro, and you can only install packages that have a build for Arm.
 
### Can dual-booting macOS and Asahi Linux slow down my macOS?
 
No. Your Mac will run and allocate resources like CPU and memory for one operating system at a time, so there shouldn’t be a performance drop on macOS.
 
Muhammad Munna is an Electrical Engineering student who is passionate about technology and writing. He loves to experiment with different techs and dig deep into them. In his free time, he can be found fiddling with his smartphone camera.
 
Our latest tutorials delivered straight to your inbox




