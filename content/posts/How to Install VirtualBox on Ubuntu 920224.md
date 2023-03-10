---
title: "Unleash the Full Potential of Ubuntu with this Simple Trick to Install Virtualbox!"
ShowToc: true 
date: "2022-11-21"
author: "Philip Taylor"
---
*****
Unleash the Full Potential of Ubuntu with this Simple Trick to Install Virtualbox!

Ubuntu, one of the most popular operating systems in the world and the go-to for many developers, can be extremely powerful when utilized to its full potential. However, even the most experienced Ubuntu users might not know that by installing VirtualBox, they can unleash the full power of this OS. With VirtualBox installed, Ubuntu users can run multiple operating systems in a virtualized environment within Ubuntu itself.

This simple trick of installing VirtualBox not only boosts your productivity but also expands your application capabilities. You might be wondering why you need to run a virtual machine when you already have a fully functional operating system. The answer is quite simple - having multiple operating systems running simultaneously in one machine increases your productivity and efficiency.

VirtualBox is a free and open-source virtualization software created by Oracle. It allows users to create as many virtual machines as they want, running different operating systems such as Windows, Mac OS, and Linux variants. Users can configure each virtual machine with varying properties, such as the amount of RAM, hard disk size, and operating system version.

So, how do you get started with getting VirtualBox up and running on Ubuntu? The process is simple and involves just a few clicks.

Firstly, open the Terminal by pressing Ctrl+Alt+T or by typing Terminal in the search bar. Once the Terminal is open, enter the following command:

```
sudo apt install virtualbox
```

This command will install the latest version of VirtualBox on your system. Once this command finishes, you should see VirtualBox in your Ubuntu applications.

Next, you need to create a new virtual machine. Launch the VirtualBox application and click on the "New" button in the top left corner. Follow the prompts for creating a new virtual machine, including selecting the operating system and choosing the amount of memory and hard disk space you want to allocate.

Once you've created your virtual machine, you can start it up and begin using it just like you would a physical machine. This is incredibly useful for running software that only works on certain operating systems, for testing code on different platforms, and for keeping your development environment organized and efficient.

Overall, installing VirtualBox on Ubuntu is a simple but powerful trick to unlock the full potential of your operating system. With this tool, you can increase your productivity and expand your capabilities, allowing you to achieve more in less time. So what are you waiting for? Install VirtualBox today and unleash the full potential of your Ubuntu machine!

{{< youtube v1JVqd8M3Yc >}} 



Since it is a cross-platform program, VirtualBox can be run on multiple operating systems. This means that it will work perfectly fine on Linux, just as it does on Windows. Furthermore, the graphical user interface should be almost identical on all platforms.
 
Let’s see how we can install and run virtual machines on Ubuntu with VirtualBox.
 
## Install VirtualBox
 
Install VirtualBox through Ubuntu’s Software Center application. However, use the terminal here. It’s more universal, works the same way anywhere and you can see what is going on.
 
After opening a terminal emulator, you can easily install virtualbox with this command:
 

 
Normally, “virtualbox-qt” should install automatically alongside other dependencies. This is the package that shows us a graphical user interface for VirtualBox. If, for some reason, you find it missing, you can install it manually with sudo apt install virtualbox-qt.
 
VirtualBox should now appear in the applications menu. In Ubuntu’s default desktop environment, just press the Super key (usually the one with the Windows logo). Type “virtualbox” and click on the icon to launch the program. In other desktop environments, such as LXDE (Lubuntu), VirtualBox appears under the “System Tools” category.
 
## Create a New Virtual Machine
 
After launching the utility, you’ll see a button labeled “New” in the top-left corner.
 
After clicking on this button, you are guided through a few easy steps to create your first virtual machine. First, though, you need to download a bootable ISO file. For example, from this link you can download a Debian live image with your favorite desktop environment. “Live” means you can try it even without, or before, installing.
 
If time and Internet bandwidth don’t allow a download of a few gigabytes, you can download a very small Ubuntu ISO image for a quick test.
 
After naming your new virtual machine and selecting the operating system type and version, click on “Next.”
 
Operating systems that include a graphical user interface will need at least 2GB of RAM. Text-based server distributions can run with 1GB of RAM. Keep in mind, though, that if you move the slider past the green line, things can dramatically slow down.
 
In the next step you can create the new virtual disk where the operating system will be installed. When you just want to test a live operating system, without installing, you can skip this step and choose “Do not add a virtual hard disk.”
 
If you do create a virtual disk, you’ll have to choose the disk file format. You can leave the default answer checked if you don’t plan to use this virtual disk with other virtualization software.
 
When asked about virtual hard disk allocation type, you should choose “Fixed size.” This offers the best read/write performance. Though if you prefer your VM disk size to start small and grow as you use it, then select the “Dynamically allocated” option.
 
Afterwards choose the name for the file that will host your virtual disk. After deciding its size, click on “Create” and finish setting up the virtual machine.
 
Finally, click on the green arrow labeled “Start” to boot your machine.
 
When first launching a virtual machine, you will be prompted to select a startup disk. This is the step where you click on the small folder icon with a green arrow (lower-right side of window). After browsing and selecting the ISO file you have downloaded, you can boot the machine.
 
## Alternate Way to Add Bootable ISO to Virtual Machine
 
If you accidentally close this prompt, it won’t be shown again. In this case the procedure to add a bootable ISO is different. Right-click on the virtual machine and click on “Settings -> Storage” in the first column. In the middle column, under “Controller: IDE,” we can see a small CD icon labelled “Empty.” In the third right column you’ll see “Optical Drive,” and at the far right of that, a small CD icon. Click on it and browse to the ISO file. When done, click OK to save the settings. The machine will now boot from the ISO image.
 
## Conclusion
 
At this point you can run almost any operating system on our Ubuntu host. You can even install Android in VirtualBox.
 
Fell in love with computers when he was four years old. 27 years later, the passion is still burning, fueling constant learning. Spends most of his time in terminal windows and SSH sessions, managing Linux desktops and servers.
 
Our latest tutorials delivered straight to your inbox




