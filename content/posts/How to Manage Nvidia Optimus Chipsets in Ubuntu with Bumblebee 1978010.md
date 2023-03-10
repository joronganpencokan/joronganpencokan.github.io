---
title: "Revolutionize Your Ubuntu Gaming Experience: Learn How to Master Nvidia Optimus Chipsets with Bumblebee!"
ShowToc: true 
date: "2023-06-27"
author: "Fernando Cisneros"
---
*****
Revolutionize Your Ubuntu Gaming Experience: Learn How to Master Nvidia Optimus Chipsets with Bumblebee!

Are you a Ubuntu user and a gaming enthusiast? Do you have an Nvidia Optimus chipset on your Ubuntu machine that has been causing you problems when gaming? If yes, then you need to learn how to master Nvidia Optimus chipsets with Bumblebee to revolutionize your Ubuntu gaming experience.

Nvidia Optimus is a technology that allows laptops to switch between integrated and discrete graphics seamlessly. This sounds like a great idea in theory, but in practice, it can be quite problematic, especially for Ubuntu users. The problem with Nvidia Optimus chipsets on Ubuntu is that it doesn't work out-of-the-box. Ubuntu doesn't recognize which graphics card to use, resulting in poor gaming performance, screen tearing, and other annoying issues.

Enter Bumblebee. Bumblebee is an open-source project that provides support for Nvidia Optimus technology on Linux. It works by allowing applications to use the Nvidia graphics card when necessary and switch back to the integrated graphics card when not in use. This ensures a seamless and smooth gaming experience without the usual issues associated with Nvidia Optimus technology.

To get started with Bumblebee, you first need to ensure that your machine has an Nvidia Optimus chipset. You can check this by running the following command in your terminal:

$ lspci | grep -i nvidia

If you see a result, then you have an Nvidia Optimus chipset. Next, you need to install the Bumblebee package on your Ubuntu machine. You can do this by running the following command in your terminal:

$ sudo apt-get install bumblebee bumblebee-nvidia primus

Once installed, you need to configure Bumblebee to work correctly with your machine. To do this, open the Bumblebee's configuration file using your favorite text editor:

$ sudo nano /etc/bumblebee/bumblebee.conf

In this file, you need to change the following settings:

1. Change the 'Driver=' line to 'Driver=nvidia'
2. Change the 'KernelDriver=nvidia-current' line to 'KernelDriver=nvidia-VERSION'
3. Change the 'LibraryPath=' and 'XorgModulePath=' lines to match the paths on your system.

Once you have made the necessary changes, save the file and exit your text editor. Next, you need to test that Bumblebee is working correctly by running the following command in your terminal:

$ optirun glxgears

If everything is configured correctly, you should see the glxgears application running on your Nvidia Optimus chipset. Congratulations! You have successfully mastered Nvidia Optimus chipsets with Bumblebee.

In conclusion, Bumblebee is an essential tool for Ubuntu users who want to revolutionize their gaming experience. It provides support for Nvidia Optimus technology and ensures a seamless and smooth gaming experience without the usual issues associated with Nvidia Optimus technology. By following the steps outlined above, you too can master Nvidia Optimus chipsets with Bumblebee and enjoy uninterrupted gaming sessions on your Ubuntu machine.

{{< youtube VP-R7LNSJXA >}} 



Bumblebee is a software tool for Linux with the aim to provide support for NVIDIA Optimus laptops for GNU/Linux distributions. Optimus is a hybrid display technology where the integrated GPU renders the display while the dedicated GPU (in this case, an nVidia graphic card) does all the processing and sends the output to the integrated GPU. When the laptop is running on battery supply, the dedicated GPU is turned off to save power and prolong the battery life.
 
Bumblebee tries to mimic the Optimus technology behavior by using the dedicated GPU for rendering when needed and to power it down when not in use.
 
Ubuntu systems already come with Nvidia Prime which provides a way for users to switch between Nvidia and Intel GPUs. The problem with this is that it only works for the whole desktop and does not allow a user to set the GPU for a certain application. In some systems there have been reports of excessive heating and malfunctions to the system when Nvidia GPU is set for the whole desktop. Using Bumblebee would be a better option in this case.
 
## Installing Bumblebee
 
Before you start installing Bumblebee, I am going to assume that you already have the Nvidia graphics installed. If you have not installed them, you can do so by opening the terminal and running the following command:
 
You can also run this command so that it uses the Intel graphics card:
 
Installing Bumblebee will now be determined by the Nvidia graphics that you want to use it with. The following are the options:
 
### nVidia-361
 
To use it with nvidia-316, you can run this command to install Bumblebee:
 
### nVidia-370
 
If you want to use it with the nvidia-370 and are running Ubuntu 16.04 or earlier, you can use Bumblebee Development PPA for installation:
 
If you are using Ubuntu 16.10 or later, you will not need the Bumblebee Development PPA, as the patches are already in the official Ubuntu repository. Running the following command will install it:
 
In my case I am installing it on Ubuntu 16.04.
 

 
## Configuration and Usage
 
After successfully installing Bumblebee, you will need to configure it to run well. The Bumblebee configuration file is at “/etc/bumblebee/bumblebee.conf.” Open it using a text editor of your choice. Open the configuration file and scroll down to the area shown on the screenshot below.
 
If you are using nvidia-361, change the following options from the above screenshot to set it up:
 
- Set the Driver to “nvidia”
 - Set the KernelDriver to “nvidia-361”
 - Set the LibraryPath to “/usr/lib/nvidia-361:/usr/lib32/nvidia-361”
 - Set the XorgModulePath to “/usr/lib/nvidia-361/xorg,/usr/lib/xorg/modules”

 
Save the file.
 
If using nvidia-370:
 
- Set Driver to “nvidia”
 - Set the KernelDriver to “nvidia-370”
 - Set the LibraryPath to “/usr/lib/nvidia-370:/usr/lib32/nvidia-370”
 - Set the XorgModulePath to “/usr/lib/nvidia-370/xorg,/usr/lib/xorg/modules”

 
If you have installed a different version of nVidia graphics, remember to change the configuration file to match the version.
 
The final step to get Bumblebee working is to reboot your computer. The discrete card will now be turned off. If you want to run Bumblebee with an application, run this command where some_app_or_game is the name of the application or the game:
 
## Conclusion
 
Bumblebee is very important for people who run graphic intensive applications on their machines. With it you can switch between the dedicated and integrated graphics as necessary, and it will allow you to maintain the performance of your machine without sacrificing the battery life.
 
I am an intelligent and presentable individual with a degree in Computer Science and over four years experience in Management, Software Development, Information Technology Support and Tech article/tutorial writing. I possess a fresh, modern approach to the industry, employing creative and enthusiastic methods to problem-solving and would like to realize my full potential through practice, effectiveness, and innovation.
 
Our latest tutorials delivered straight to your inbox




