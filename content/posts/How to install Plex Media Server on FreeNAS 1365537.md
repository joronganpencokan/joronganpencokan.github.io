---
title: "Unlock Your Inner Media Mogul: The Ultimate Guide to Installing Plex Media Server on Freenas!"
ShowToc: true 
date: "2023-01-31"
author: "Errol Willis"
---
*****
# Unlock Your Inner Media Mogul: The Ultimate Guide to Installing Plex Media Server on Freenas!

Are you tired of streaming media content from various websites and different devices? Do you want to have all your media files in one spot? How about creating your media streaming service, accessible from anywhere in the world? If these sound like a dream, then you need to install Plex Media Server on Freenas.

Plex Media Server is a powerful streaming server that allows users to stream movies, TV shows, music, and pictures across different devices. Freenas, on the other hand, is a free and open-source network-attached storage (NAS) operating system based on FreeBSD. Freenas provides a platform to store and access your media content while providing you with advanced features, such as encryption, replication, and snapshots.

In this guide, we will walk you through how to install Plex Media Server on Freenas.

## Step 1: Install Freenas

Before you can install Plex Media Server, you need to have Freenas up and running on your system. Freenas is free to use, and you can download the latest version from the official website. Once downloaded, follow the installation process to set up Freenas on your system.

## Step 2: Configure Freenas

After installing Freenas, you need to configure it to access your media content. To do this, create a dataset for your media files. A dataset is a storage location created on Freenas for storing files. To create a dataset, navigate to Storage > Pools > Add. Here, select the type of pool you need and add the desired disks.

After creating a dataset, create a share to allow remote access to the data. To do this, go to Sharing > Windows (SMB) Shares > Add Windows (SMB) Share. Here, select the newly created dataset and specify the share name.

## Step 3: Install Plex Media Server Plugin

Now that you have configured Freenas, it is time to install Plex Media Server. To install Plex, you need to have the Plugins service up and running on Freenas.

To install the Plugins service on Freenas, navigate to Services > Plugins and install the “freenas-plugin-plex” plugin. This will install the latest Plex Media Server version available.

## Step 4: Configure Plex Media Server

Once you have installed Plex Media Server, you need to configure it to access your media content.

To do this, open Plex Media Server from the Freenas GUI by navigating to Jails > Plex Media Server > Shell. Here, type “service plexmediaserver stop” to stop the server. Then, navigate to “/usr/local/plexdata-plexpass/Plex Media Server/” and create a new folder called “Library.”

Next, navigate to “/etc/rc.d/” and create a new file called “plexmediaserver,” which will contain the configuration for your server. Open the file and copy the following code:

```
#!/bin/sh

# PROVIDE: plexmediaserver
# REQUIRE: LOGIN DAEMON NETWORKING
# KEYWORD: shutdown

. /etc/rc.subr

name="plexmediaserver"
rcvar="plexmediaserver_enable"

load_rc_config $name

: ${plexmediaserver_enable:="NO"}

command="/usr/local/bin/plexmediaserver"
command_args="--daemon --nocolor"

pidfile="/var/run/${name}.pid"

start_precmd="${name}_prestart"

plexmediaserver_prestart()
{
  # Create the necessary directory structure for Plex
  if [ ! -d "/config/Library/Application Support" ]; then
    mkdir -p "/config/Library/Application Support"
    ln -s "/data/Library/Application Support/Plex Media Server" "/config/Library/Application Support"
  fi
}

run_rc_command "$1"
```

Next, edit the file and replace `/config` with the path to your Plex data folder, which is `/usr/local/plexdata-plexpass/Plex Media Server/`. Save the file and exit.

Finally, start Plex Media Server by typing “service plexmediaserver start” in the shell.

## Step 5: Accessing Your Plex Server

Now that you have installed and configured Plex Media Server on Freenas, you can access your media streaming service from anywhere in the world.

To access your Plex Server, open a web browser and go to “http://<your-freenas-ip-address>:32400/web”. Here, you can log in and start streaming your media content.

## Conclusion

Plex Media Server and Freenas are powerful tools that can help you manage and stream your media content. By following the steps in this guide, you can easily install and configure Plex Media Server on Freenas and create your media streaming service. With Plex, you can easily access your media content from different devices, and Freenas provides advanced features to keep your data safe and secure. So, what are you waiting for? Unlock your inner media mogul and start streaming today!

{{< youtube -1m_nGNUglM >}} 



Plex is perhaps one of the best media server application designed to organize and stream videos, music, and pictures to any Windows 10, macOS, and Linux machines as well as other devices, such as Xbox One, smart TVs, streaming boxes (for example, Roku), mobile devices using the Plex client or web application. You can think of this client-server solution as your private version of Netflix.
 
Although you can set up a standalone Plex server, if you already have a FreeNAS server to share files in the network, you can simply set up a plugin to convert the file server into a media streaming service for your home. However, before you can start streaming your media files, you must install the Plex plugin using the Jails system on FreeNAS, configure the storage, and set up your Plex library.
 
In this guide, you’ll learn the steps to install and set up the Plex Media Server plugin on FreeNAS version 11.2 or higher.
 
## How to install Plex plugin on FreeNAS
 
To install and set up Plex on FreeNAS, you need to configure the Jails system, storage to store media files, and Plex library. If this is the first time adding a plugin, FreeNAS will take some additional time to download and configure the Jails system.
 
### Installing Plex plugin
 
Use these steps to install Plex on FreeNAS:
 
- Open FreeNAS in your web browser.
 - Sign into your root account.
 - Click on Plugins from the left pane.
 - Select the Plex Media Server plugin (or Plex Media Server (PlexPass) if you have a paid license).
 - Click the settings (three-dotted) button next to the Plex plugin and select the Install option.
 - Plex Media Server plugin on FreeNAS
 - Select the DHCP option if you’re planning to configure your router to use the dynamically assign TCP/IP address as the permanent configuration for the server. Or clear the DHCP option to specify a static IP address configuration selecting the network interface, IPv4 address, and netmask.
 - Plex IP configuration on FreeNAS
 - Click the Save button.
 - Click the Close button.
 - Plex plugin installation complete

 
Once you complete the steps, don’t try to open Plex, instead jump to the following set of instructions to configure the storage for the media files.
 
Open FreeNAS in your web browser.
 
Sign into your root account.
 
Click on Plugins from the left pane.
 
Select the Plex Media Server plugin (or Plex Media Server (PlexPass) if you have a paid license).
 
Click the settings (three-dotted) button next to the Plex plugin and select the Install option.
 
Plex Media Server plugin on FreeNAS

 
Select the DHCP option if you’re planning to configure your router to use the dynamically assign TCP/IP address as the permanent configuration for the server. Or clear the DHCP option to specify a static IP address configuration selecting the network interface, IPv4 address, and netmask.
 
Plex IP configuration on FreeNAS

 
Click the Save button.
 
Click the Close button.
 
Plex plugin installation complete

 
### Configuring Plex media storage
 
After installing Plex, you need to mount the storage that you’re planning to use to store your media files. You can use a folder already available in one of your FreeNAS shared folders, or you can create a new dataset to use as storage for your Plex media.
 
Use these steps to mount a FreeNAS folder to the Plex server:
 
- Open FreeNAS in your web browser.
 - Sign into your root account.
 - Click on Plugins from the left pane.
 - Click on Installed.
 - Click the settings (three-dotted) button next to the Plex plugin and select the Stop option.
 - Stop Plex on FreeNAS
 - Click on Jails from the left pane.
 - Click the settings (three-dotted) button next to the Plex jail and select the Mount points option.
 - Plex mount points option on FreeNAS
 - Click the Actions button.
 - Click the Add Mount Point option.
 - Add new mount point to Plex
 - In “Source,” click the folder icon, navigate, and select the folder or dataset where your media library will be stored.
 - In “Destination,” click the folder icon, navigate, and select the media folder.
 - Plex configure source and destination mount point
 - Quick tip: If you’re a tech-savvy user, you can also use the FreeNAS terminal to create a new folder to map as the destination inside of Plex.
 - Click the Save button.
 - Click on Plugins from the left pane.
 - Click on Installed.
 - Click the settings (three-dotted) button next to the Plex plugin and select the Start option.
 - Start Plex on FreeNAS

 
After you complete the steps, the Plex server will be ready for the initial setup.
 
Click on Installed.
 
Click the settings (three-dotted) button next to the Plex plugin and select the Stop option.
 
Stop Plex on FreeNAS

 
Click on Jails from the left pane.
 
Click the settings (three-dotted) button next to the Plex jail and select the Mount points option.
 
Plex mount points option on FreeNAS

 
Click the Actions button.
 
Click the Add Mount Point option.
 
Add new mount point to Plex

 
In “Source,” click the folder icon, navigate, and select the folder or dataset where your media library will be stored.
 
In “Destination,” click the folder icon, navigate, and select the media folder.
 
Plex configure source and destination mount point

 
Click the settings (three-dotted) button next to the Plex plugin and select the Start option.
 
Start Plex on FreeNAS

 
### Initial Plex setup
 
Use these steps to add a folder to the Plex library to access media files stored on FreeNAS:
 
- Open FreeNAS in your web browser.
 - Sign into your root account.
 - Click on Plugins from the left pane.
 - Click on Installed.
 - Click the settings (three-dotted) button next to the Plex plugin and select the Management option.
 - Open Plex on the web from FreeNAS
 - Quick tip: If the Plex web access doesn’t open in a new tab, then you may need to access the service manually with this address: 10.1.2.192:32400 (just make sure to replace the IP address with the address of your Plex jail).
 - Sign in with your Plex account.
 - Click the Got it button.
 - Initial Plex server setup
 - Specify a name for the Plex server. (The default name should be fine.)
 - Clear the Allow me to access my media outside my home option if you won’t use this feature.
 - Click the Next button.
 - Click the Add library button.
 - Plex add library option
 - Select the media type you’re about to include. For example, Movies.
 - Select Plex library type
 - Click the Next button.
 - Click the Browse for media folder button.
 - Plex add folders to library option
 - Select the folder icon, navigate, and select the media folder.
 - Plex select media folder from FreeNAS
 - Click the Add button.
 - Click the Add library button.
 - Complete Plex adding folder to library setup
 - Click the Next button.
 - Click the Done button.

 
Once you complete the steps, you can start streaming the media you added using Plex.
 
Click the settings (three-dotted) button next to the Plex plugin and select the Management option.
 
Open Plex on the web from FreeNAS

 
Sign in with your Plex account.
 
Click the Got it button.
 
Initial Plex server setup

 
Specify a name for the Plex server. (The default name should be fine.)
 
Clear the Allow me to access my media outside my home option if you won’t use this feature.
 
Click the Next button.
 
Click the Add library button.
 
Plex add library option

 
Select the media type you’re about to include. For example, Movies.
 
Select Plex library type

 
Click the Browse for media folder button.
 
Plex add folders to library option

 
Select the folder icon, navigate, and select the media folder.
 
Plex select media folder from FreeNAS

 
Click the Add button.
 
Complete Plex adding folder to library setup

 
Click the Done button.




