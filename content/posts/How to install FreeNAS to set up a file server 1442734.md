---
title: "Unlock the Ultimate Guide to Setting Up Your Own File Server with Freenas - No Tech Skills Needed!"
ShowToc: true 
date: "2023-02-19"
author: "John Wilson"
---
*****
# Unlock the Ultimate Guide to Setting Up Your Own File Server with FreeNAS - No Tech Skills Needed!

If you're looking for a way to store and share files easily and safely, building your own file server with FreeNAS might be the solution you're looking for. FreeNAS is a free and open-source operating system based on FreeBSD that allows you to turn any computer into a powerful file server. In this article, we'll guide you through the process of setting up your own FreeNAS file server, step by step, even if you don't have any advanced technical skills.

## Why Build a File Server with FreeNAS?

Having your own file server at home or in your office has many benefits. First and foremost, it's an easy way to store all your files, documents, photos, videos, and music in one central location that you can access from any device and anywhere. You won't have to rely on cloud services with limited storage space or worry about the privacy and security of your data. Additionally, having a file server can help you organize and manage your files more efficiently, allowing you to share and collaborate with others easily.

FreeNAS is a great choice for a file server because it's free, reliable, and easy to use. It comes with a user-friendly web interface that allows you to configure and manage your server from any computer or mobile device. FreeNAS also supports a wide range of file sharing protocols, including Samba (for Windows), NFS (for Linux), and AFP (for Mac). Plus, it can act as a backup server, media center, or even a virtualization host.

## What You'll Need

Before you start building your own FreeNAS file server, you'll need to gather some hardware and software components. Here's a list of what you'll need:

- A compatible computer or server: FreeNAS can run on almost any computer hardware, but it's recommended that you use a dedicated machine with at least 8GB of RAM, a multi-core CPU, and plenty of storage space (ideally, four or more hard drives).
- Hard drives: You'll need one or more hard drives to store your files. FreeNAS supports different types of drives, such as SATA, SAS, and SSD, and you can mix and match them in different configurations (e.g., RAID).
- A USB drive: You'll need a USB drive to install FreeNAS on your computer. Make sure it's at least 8GB in size and empty.
- A network connection: Your file server will need to be connected to your local network using an Ethernet cable. You'll also need to configure your router to forward the necessary ports to your file server.
- A computer or mobile device with a web browser: You'll use your computer or mobile device to access the FreeNAS web interface and manage your server.

## Step-by-Step Guide to Setting Up Your Own File Server with FreeNAS

Now that you have everything you need, it's time to start building your file server. Here's a step-by-step guide to setting up your own FreeNAS file server:

1. Download FreeNAS and create a bootable USB drive: You can download the latest version of FreeNAS from the official website (https://www.freenas.org/download-freenas-release/). Once you've downloaded the file, use a tool like Rufus or Etcher to create a bootable USB drive from the FreeNAS ISO image.

2. Install FreeNAS on your computer: Insert the FreeNAS USB drive into your computer and boot from it. Follow the on-screen instructions to install FreeNAS on your computer. Make sure you select the right disk(s) and configuration options for your setup.

3. Configure the basic settings: Once FreeNAS is installed, you'll need to configure some basic settings, such as the network interface, the hostname, and the time zone. You can do this from the FreeNAS web interface, which you can access by typing the IP address of your server in a web browser.

4. Create a storage pool: A storage pool is a group of hard drives that you can use to store your files. To create a storage pool, go to Storage > Pools in the FreeNAS web interface and follow the instructions. You can choose different types of pools, such as RAID-Z or RAID-Z2, depending on the level of redundancy and performance you want.

5. Create a dataset: A dataset is a folder or directory within a storage pool where you can store your files. To create a dataset, go to Storage > Datasets in the FreeNAS web interface and follow the instructions. You can set permissions, quotas, and other options for your dataset.

6. Configure file sharing: Once you have your storage pool and dataset, you can configure file sharing protocols, such as Samba, NFS, or AFP, depending on the devices and operating systems you'll be using. You can do this from the FreeNAS web interface under Services > SMB, NFS, or AFP.

7. Set up users and groups: To manage access and permissions for your files, you'll need to create users and groups. You can do this from the FreeNAS web interface under Accounts > Users or Groups. Make sure you set strong passwords and restrict access to sensitive files.

8. Enable remote access: If you want to access your files remotely, you'll need to enable remote access using a VPN or other secure method. You can do this from the FreeNAS web interface under Network > Global Configuration.

## Conclusion

Building your own file server with FreeNAS is a great way to store, share, and manage your files easily and safely. With this step-by-step guide, you can set up your own FreeNAS file server even if you don't have advanced technical skills. Just make sure you follow the instructions carefully, choose the right hardware components, and secure your server properly. Once you have your own file server, you'll wonder how you ever managed without it.

{{< youtube eJvQKLVrmU8 >}} 



FreeNAS is a freely available and open source powerful Network Attached Storage (NAS) OS, which anyone can use to set up a server for home and office to share files and media with Windows 10 (and older versions) as well as with macOS and Linux devices.
 
Also, the OS is based on the robust OpenZFS filesystem, which allows you to access advanced features, such as data integrity, redundancy, early detection of faulty drive, and much more.
 
In this guide, you’ll learn the steps to install FreeNAS version 11.2 or higher on a device using USB, Solid-State Drive (SSD), or Hard Disk Drive (HDD) to share files and media across your home or work network. Actually, the installation process of FreeNAS is simple, you only need compatible hardware and a USB bootable media with the installation files. (After the installation, you can use these instructions to share a folder with Windows 10 devices.)
 
- FreeNAS hardware requirements
 - How to download FreeNAS ISO file
 - How to create FreeNAS USB bootable media
 - How to install FreeNAS on USB, SSD, HDD

 
## FreeNAS hardware requirements
 
FreeNAS is a light-weight solution based on the FreeBSD version of Linux that can run virtually on any computer or server, but they most meet the minimum requirements.
 
Usually, when using this NAS OS, you want to have around 1GB of RAM for each terabyte of storage. However, after 64GB of memory, the performance increase after adding more memory will be minimal.
 
## How to download FreeNAS ISO file
 
Use these steps to download the ISO file with the latest version of FreeNAS:
 
- Open FreeNAS website.
 - Click the Download button for the “current stable release.”
 - Download latest version of FreeNAS

 
After you complete the steps, you can use Rufus to create a USB bootable media.
 
Open FreeNAS website.
 
Click the Download button for the “current stable release.” 
 
Download latest version of FreeNAS

 
## How to create FreeNAS USB bootable media
 
Use these steps to create a USB bootable media to install FreeNAS 11.2:
 
- Open Rufus website.
 - Under the “Download” section, click the download link for the latest version.
 - Double-click the file to launch the tool.
 - Use the “Device” drop-down menu and select the USB flash drive option.
 - Click the Select button.
 - Select the FreeNAS ISO file.
 - Click the Open button.
 - Click the Start button.
 - Rufus app to create FreeNAS USB boot drive

 
Once you complete the steps, before you start your device with the tool, you need to make sure that your device can boot from USB.
 
Open Rufus website.
 
Under the “Download” section, click the download link for the latest version.
 
Double-click the file to launch the tool.
 
Use the “Device” drop-down menu and select the USB flash drive option.
 
Click the Select button.
 
Select the FreeNAS ISO file.
 
Click the Open button.
 
Click the Start button.
 
Rufus app to create FreeNAS USB boot drive

 
Usually, you’ll need to access your device Basic Input/Output System (BIOS) or Unified Extensible Firmware Interface (UEFI) hitting one of the functions key (F1, F2, F3, F10, or F12), the ESC, or the Delete key during boot.
 
Inside the first, look for the Boot section and make sure the boot order is set to the drive that contains the FreeNAS installation files, and save the configuration.
 
The BIOS/UEFI can be different depending on the manufacturer and even per computer model, as such make sure to check your manufacturer support website for more specific instructions.
 
## How to install FreeNAS on USB, SSD, HDD
 
To install FreeNAS on a USB, SSD, or HDD, use these steps:
 
- Start your device with the FreeNAS USB install media.
 - Select the Boot FreeNAS Installer option and press Enter.
 - Boot FreeNAS installer option
 - Select the Install/Upgrade option with the arrow keys and press Enter.
 - FreeNAS console setup
 - Select the drive (USB, SSD, or HDD) to install FreeNAS and press Enter. (You can use one or more drives for redundancy, and you can even install the OS onto a USB drive, but it’s not a requirement.)
 - FreeNAS choose OS installation location
 - Choose the Yes option and press Enter to continue.
 - FreeNAS installation confirmation
 - Specify a root password for installation and press Enter.
 - FreeNAS root password set up
 - Select the Boot via BIOS option whenever possible and press Enter. Otherwise, if you’re using newer hardware, select the Boot via UEFI option.
 - FreeNAS install boot mode
 - Disconnect the FreeNAS USB bootable media and press Enter.
 - FreeNAS installation complete
 - Select the Reboot System option and press Enter.

 
Once you complete the steps, FreeNAS will start, and the “Console setup” will appear with options to manage the server using Linux commands and the TCP/IP address to manage the server using a friendly interface with any modern browser.
 
Start your device with the FreeNAS USB install media.
 
Select the Boot FreeNAS Installer option and press Enter.
 
Boot FreeNAS installer option

 
Select the Install/Upgrade option with the arrow keys and press Enter.
 
FreeNAS console setup

 
Select the drive (USB, SSD, or HDD) to install FreeNAS and press Enter. (You can use one or more drives for redundancy, and you can even install the OS onto a USB drive, but it’s not a requirement.)
 
FreeNAS choose OS installation location

 
Choose the Yes option and press Enter to continue.
 
FreeNAS installation confirmation

 
Specify a root password for installation and press Enter.
 
FreeNAS root password set up

 
Select the Boot via BIOS option whenever possible and press Enter. Otherwise, if you’re using newer hardware, select the Boot via UEFI option.
 
FreeNAS install boot mode

 
Disconnect the FreeNAS USB bootable media and press Enter.
 
FreeNAS installation complete

 
Select the Reboot System option and press Enter.
 
To connect to the FreeNAS web interface, type the IP address of the server on your browser, and login using root as the username and type the password you selected during the installation.




