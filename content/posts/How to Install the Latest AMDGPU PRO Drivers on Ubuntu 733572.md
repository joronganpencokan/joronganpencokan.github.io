---
title: "You Won't Believe How Easy It Is To Get The Latest AMDGPU Pro Drivers Installed On Ubuntu!"
ShowToc: true 
date: "2023-06-16"
author: "Kathryn Harris"
---
*****
## You Won't Believe How Easy It Is To Get The Latest AMDGPU Pro Drivers Installed On Ubuntu!

If you're an Ubuntu user and you want to take advantage of the latest graphics drivers from AMD, you might be wondering how you can do it with minimal hassle. Thankfully, the process is much easier than you might expect, and in this article, we'll show you step-by-step how to get the latest AMDGPU Pro drivers installed on your Ubuntu machine.

## What Are AMDGPU Pro Drivers?

In case you're not familiar, AMDGPU Pro drivers are AMD's proprietary graphics drivers that provide advanced features and performance optimizations for AMD Radeon graphics cards. These drivers are designed to work specifically with Linux distributions, including Ubuntu, and they are updated regularly to ensure compatibility with the latest hardware and software.

Installing the latest AMDGPU Pro drivers on Ubuntu can be a bit tricky, but if you follow these steps carefully, you should be up and running in no time.

## Step 1: Download the AMDGPU Pro Driver Package

The first step is to download the latest AMDGPU Pro driver package from the AMD website. Go to the AMD website's download page and choose your graphics card model and the version of Ubuntu you're running. You should see a list of available downloads. Click on the one that corresponds to your system, and the download should begin automatically.

## Step 2: Install the Required Dependencies

Before you can install the AMDGPU Pro driver package, you need to make sure that you have all the required dependencies installed. Open a terminal and run the following command:

```
sudo apt-get install libdrm2 libdrm-amdgpu1 libdrm-intel1 libdrm-radeon1 libgl1-mesa-dri libgl1-mesa-glx libglapi-mesa libgles2-mesa libllvm9 libpciaccess0 libwayland-client0 libwayland-server0 libx11-6 libx11-xcb1 libxcb-dri2-0 libxcb-dri3-0 libxcb-glx0 libxcb-present0 libxcb-sync1 libxcb1 libxdamage1 libxfixes3 libxshmfence1 libxxf86vm1
```

This command will install all the libraries and dependencies required to run the AMDGPU Pro driver package.

## Step 3: Install the AMDGPU Pro Driver Package

Now that you have all the required dependencies installed, it's time to install the AMDGPU Pro driver package. Navigate to the directory where you saved the driver package, and then run the following command:

```
sudo dpkg -i amdgpu-pro-XX.XX-XXXXXX.deb
```

Replace "XX.XX-XXXXXX" with the version number of the driver package you downloaded. This command will install the driver package on your system.

## Step 4: Restart Your System

After the installation is complete, you'll need to restart your system for the changes to take effect. Run the following command to reboot your system:

```
sudo shutdown -r now
```

## Step 5: Verify Your Installation

Once your system has rebooted, you can verify that the AMDGPU Pro drivers are installed and working properly. Open a terminal and run the following command:

```
sudo apt install clinfo
clinfo
```

This command will install the clinfo package and then run it to display information about your GPU. If the output shows your GPU model and the AMDGPU Pro driver version, then the installation was successful!

## Conclusion

As you can see, installing the latest AMDGPU Pro drivers on Ubuntu is a relatively simple process that can be done in just a few steps. Follow the steps outlined in this article, and you'll be up and running with the latest drivers in no time. So go ahead and give it a try, and see what kind of performance improvements you can get on your system!

{{< youtube BoGYR3JiH-A >}} 



AMDGPU-PRO is AMD’s proprietary driver for its latest graphics cards. That means that it mainly covers the Polaris cards, the RX 4XX series and the RX 5XX series. It does work with older cards too, but they won’t see as much continual improvement and development.
 
Like its name suggests, AMDGPU-PRO is intended for professional use. Don’t worry. You can absolutely game with these drivers. AMD branded them for workstation users. As a result, AMD only releases the AMDGPU-PRO drivers for long-term support (LTS) releases and “Enterprise” distributions. For Ubuntu this means that you can only install these drivers on the latest LTS release. In this case, it’s 16.04.2.
 
Running an LTS release has some drawbacks. For starters, you won’t get the latest releases of new software on your system. You will get security fixes and some backports. You can get around a lot of these constraints in other ways, like importing applications such as Firefox from other releases, but it can be a pain to do so.
 
If you don’t want to run the LTS release or you already aren’t, you can always install the open-source AMDGPU drivers. In the latest releases of Ubuntu, they may even work out of the box, depending on your card. The open-source drivers don’t get all the new features of the proprietary ones, though, and are lacking in Vulkan support.
 
## Getting the Packages
 
So you’ve chosen the Pro drivers. How do you get them? Since these drivers are AMD’s territory, they aren’t available in the Ubuntu repositories. You have to go to AMD’s website to download them.
 

 
Open your browser and head over to the release notes on AMD’s website. Once you’re there, scroll down to the section that starts with, “The AMDGPU-Pro Driver can be downloaded…” The link for Ubuntu will be right below. Click it to download the drivers in a tar archive.
 
Navigate into your download folder and unpack the archive.
 
Your version number may be different depending on when you’re reading this, so make sure to use the right one.
 
Unpacking the archive will give you a folder with the same name. Change into the folder and get ready to install.
 
## Installing AMDGPU-PRO
 
Once you’re in the folder, take a look around.
 
There are a lot of .deb packages in there. AMDGPU-PRO is odd when it comes to proprietary drivers on Linux. In the past proprietary graphics drivers just contained some Linux kernel modules to interact directly with the kernel and the drivers themselves. This is still the way that NVIDIA does it.
 
AMD took a very different approach recently. All of AMD’s drivers are tightly integrated with the open-source software that makes graphical displays on Linux possible. There are a number of parts in that chain including the kernel itself, the Xorg Server, and direct rendering managers. AMDGPU-PRO is the open-source AMDGPU but with added bits that AMD doesn’t want to open-source yet.
 
Because AMD doesn’t want to open-source all of this code, they had to take over maintaining their own versions of the open-source packages that the drivers rely on to ensure that everything works well. That’s why there are so many packages with the driver. When you install the AMDGPU-PRO drivers, you are replacing the Ubuntu versions of your graphics packages with the AMD ones. They’re essentially the same, but this gives AMD a controlled environment to ensure that the drivers work perfectly.
 
Now for the simple part: AMD has included a convenient script to install everything for you in the folder. Just run the script with sudo.
 
The script will run and install all of the packages that are required for your system. If you want it to ask you questions during the install, leave the “-y” off the end. That’s just there for convenience, and it’ll work fine most of the time.
 
When the script is done, restart your computer and enjoy your new drivers!
 
Nick is a freelance tech. journalist, Linux enthusiast, and a long time PC gamer.
 
Our latest tutorials delivered straight to your inbox




