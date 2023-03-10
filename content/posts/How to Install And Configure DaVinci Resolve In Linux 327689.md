---
title: "Unleash Your Inner Spielberg: Unlock the Secrets to Installing and Configuring DaVinci Resolve in Linux!"
ShowToc: true 
date: "2023-02-10"
author: "Kelly Galindo"
---
*****
Unleash Your Inner Spielberg: Unlock the Secrets to Installing and Configuring DaVinci Resolve in Linux!

If you're looking to take your video editing game to a whole new level, DaVinci Resolve is hands-down one of the best tools out there. Not only is it a top-of-the-line editing suite that can handle everything from basic cuts to complex visual effects, but it's also available for free!

However, getting DaVinci Resolve up and running on Linux can be a bit of a challenge. Fortunately, with a bit of technical know-how, you can unleash your inner Spielberg and start creating stunning videos in no time.

Here's a step-by-step guide to installing and configuring DaVinci Resolve on Linux.

Step 1: Check System Requirements 

The first thing you need to do is make sure your system can handle DaVinci Resolve. The minimum hardware requirements are as follows:

- CPU: Intel i7 or AMD Ryzen 7
- GPU: NVIDIA CUDA with at least 4GB of VRAM or AMD OpenCL with at least 4GB of VRAM
- RAM: 16GB minimum (32GB recommended)
- Storage: SSD or other high-speed drive with at least 256GB of free space

You'll also need to be running Linux Mint 18.3 or later, Ubuntu 16.04 or later, or CentOS/RHEL 7.3 or later.

Step 2: Download DaVinci Resolve 

Next, head over to the Blackmagic Design website and download the DaVinci Resolve Linux installation package. 

Step 3: Install Required Dependencies 

Before you can install DaVinci Resolve, you'll need to install a few required dependencies. Open up a terminal window and type the following command:

sudo apt-get install ocl-icd-opencl-dev fakeroot

Step 4: Install DaVinci Resolve 

Once you have the dependencies installed, navigate to the directory where you saved the DaVinci Resolve installation package and run the following command:

sudo dpkg -i davinci-resolve_<VERSION>.deb

(Note that you'll need to replace <VERSION> with the version number of the installation package you downloaded.)

Step 5: Configure DaVinci Resolve 

After you've installed DaVinci Resolve, you'll need to configure it to work with your system. 

First, open up a terminal and run the following command:

sudo nano /etc/security/limits.conf

Once the file opens, add the following lines to the end of the file:

username soft memlock 261144
username hard memlock 261144

(Note that you'll need to replace "username" with your actual username.)

Save and close the file.

Next, run the following command:

sudo nano /etc/sysctl.d/98-davinci-resolve.conf

Add the following lines to the end of the file:

vm.max_map_count=262144
kernel.sysrq=1

Save and close the file.

Finally, reboot your system to apply the changes.

Step 6: Launch DaVinci Resolve 

Once your system has rebooted, you should be able to launch DaVinci Resolve from the applications menu. When you first launch the application, you'll be prompted to set up a project location and other basic settings.

Congratulations! You've successfully installed and configured DaVinci Resolve on Linux. You're now ready to start creating amazing videos and unleashing your inner Spielberg.

{{< youtube yvuVFj33ypU >}} 



If you are a content creator, especially a video editor, then you have heard about DaVinci Resolve. DaVinci Resolve is known for its color correction capabilities in large film studios and comes with a powerful video and audio editor and composer, like Adobe After Effects, making it a go-to creative software among Linux creators. Unlike other creative software, DaVinci Resolve supports the Linux platform, so you don’t need any windows API translation layer like wine to install DaVinci Resolve.
 
## Download Linux Binaries
 
Go to the DaVinci Resolve release page and download the latest version. At the time of writing, the latest version is version 18. DaVinci Resolve comes in two versions: free and paid. Select and download the Linux binaries and save them in your download folder.
 
## Install Required Drivers
 
DaVinci Resolve is heavily dependent on GPU processing. If you have a recent Intel or AMD APU, then your integrated GPU may run DaVinci Resolve on your device. In most cases, you need an Nvidia GPU to run this software. Install the latest Nvidia drivers and CUDA for your Nvidia GPU in your Linux machine.
 
### Install the Latest Nvidia Driver In Ubuntu
 
For Ubuntu-based distributions, it is very easy to install GPU drivers. Run these commands for rebooting to install the Nvidia GPU for you.
 
### Install the Latest Nvidia Driver in Debian
 
For Debian-based distributions, you have to do something more than run some commands. Open the “/etc/apt/sources.list” file:
 
Add this line in the sources.list file. If it’s already present, append the contrib and non-free component.
 
Save this file and exit. Run the following command in your terminal to install the Nvidia driver.
 
To install Cuda, you only need to run one command:
 
After installation, reboot your device so that the changes can take effect.
 
### Install the Latest Nvidia Driver in Fedora
 
To install the Nvidia driver in Fedora Linux, you first need to enable the RPM fusion repository.
 
Detect the Nvidia GPU and install the required drivers.
 
After installation, reboot your machine and you are good to go.
 
## Build a Deb Package
 
The DaVinci Resolve Linux build was released to run on CentOS, a RedHat-owned distribution. Therefore, If you are using Fedora or another RedHat distribution, you don’t need to follow the build step.
 
For Fedora users, you have to unzip the downloaded file and double-click on the installer. It automatically installs and sets up all the files for you.
 
For Debian and Ubuntu-based distributions, you have to convert the DaVinci Resolve .run file into a .deb file.
 
- To make this conversion possible, download and extract the MakeResolveDeb script.Create a folder and copy the DaVinci Resolve Installer and MakeResolveDeb script into the folder.Before the conversion, install some required dependencies to build and run DaVinci Resolve flawlessly.

 
- Run the following command to convert your .run file to a .deb file, assuming that you put both the script and .run installer into the same folder.

 
It is quite an intensive process, so give your machine some time to extract and build the .deb package for you. When completed, you will be greeted with a .deb file ready to be installed.
 
## Installing Deb Package
 
Installing a .deb file is really easy in Debian and Ubuntu derivatives. Run this command to install the package:
 
If this command runs without any errors, you can see the DaVinci Resolve icon in your app grid. Open the app and you will see a splash screen like the below image.
 
## DaVinci Resolve Free vs. Paid
 
The DaVinci Resolve free version comes with all the basic features you need to edit your video, make motion graphics, color correct and edit your sounds.
 
Along with the free version, DaVinci Resolve studio version (paid) adds features such as a neural engine, stereoscopic 3D tools, dozens of extra Resolve FX filters, and Fairlight FX audio plugins, plus advanced HDR grading and HDR scopes.
 
All the studio features are required if you are working on a huge project, like filmmaking and documentaries. To make simple YouTube videos, the free version is enough for most users.
 
If you buy any Blackmagic gadgets, you get the studio version free of cost. If you are a professional video editor, consider buying the gadgets you may need.
 
## Video Transcode to Use in Davinci Resolve
 
In the free version of DaVinci Resolve, the H264 codec is not supported. Therefore, if you record video using this codec, you have to transcode the video to another format that DaVinci Resolve supports. To transcode our video, we are using FFmpeg.
 
FFmpeg is a very powerful video transcoding and processing library and has many customization options. You can read the documentation to customize FFmpeg. To install it on your device, run the following command:
 
To edit your video inside DaVinci Resolve, you have to convert it to .mov format.
 
In the above command, it’s assumed your input file is “input.mp4” and the output file name is “output.mov.” You can change the names according to your preference.
 
To convert .mkv to .mp4, run the following command.
 
## Set Up OBS Studio for Davinci Resolve
 
If you want to edit your screen recordings using DaVinci Resolve and don’t want to transcode your recorded file every time you want to edit, then you have to change some settings in your OBS application.
 
Inside your OBS settings, navigate to the “output” option and change the output mode to advanced.
 
Switch to the recording tab and change the output type to the custom output option (FFmpeg). Select “MOV” as the container format and “mpeg4” as a video encoder. In the audio encoder option, select the “pcm_s16le” option. You can refer to the settings below and make changes in your OBS software accordingly.
 
Save the settings and restart the OBS software. You can test if the settings are working or not by recording a little clip and importing it into your DaVinci Resolve software.
 
## Transcode for Online Upload and Save Space
 
You can see that when we transcode the files to edit in DaVinci Resolve, the sizes are very big – sometimes hundreds of gigabytes. Therefore, editing and uploading the rendered file of a few hundred gigabytes takes a very long time. Even if you want to store the files on your hard disk, those sizes are very huge compared to their length.
 
To fix this issue, we are using FFmpeg to transcode and compress our file. Run the following command in your terminal:
 
“input.mov” is your .mov file from DaVinci Resolve, and “output.mp4” is your output .mp4 file. You can change these names to your preference.
 
You can change the compression and output quality by adjusting the -crf flag. By default, I set it to 1, the highest quality. You can set this flag up to 25 for maximum compression. It also reduces video quality when -crf is a very high number.
 
## Frequently Asked Questions
 
### Is DaVinci better than Premier?
 
It is about personal choice. If you are familiar with Premier, and your editing workflow revolves around Adobe software, then it is better to use Premier than Resolve. If you are a newbie and want to learn DaVinci Resolve, then you are good to go. If you are an M1 Mac owner, then DaVinci Resolve runs better in Apple M1 Macs.
 
### Is 8GB RAM enough for DaVinci Resolve?
 
You need at least 16 GB of RAM to run DaVinci Resolve smoothly on your device. In addition to RAM, you need a powerful graphic card with 4GB or more VRAM to make your workflow smooth. I recommend that you invest in a desktop rather than a laptop.
 
Developer and writer. Write about linux and web.
 
Our latest tutorials delivered straight to your inbox




