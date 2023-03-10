---
title: "You Won't Believe How Easy it is to Control Your Wi-Fi Network using Linux - Learn How Now!"
ShowToc: true 
date: "2023-05-21"
author: "Kathryn Bray"
---
*****
Title: You Won't Believe How Easy it is to Control Your Wi-Fi Network using Linux - Learn How Now!

Do you know that you can control your Wi-Fi network using Linux? Yes, you heard it right! With the help of Linux, you can easily manage and customize your Wi-Fi network without any hassle. In this article, we will guide you through the process of controlling your Wi-Fi network using Linux, and we promise you won't believe how easy it is.

Linux is an open-source operating system that is widely used by developers and enthusiasts worldwide. It is known for its flexibility, scalability, and stability, making it an ideal choice for networking and system administration tasks. So, let's dive into the steps to control your Wi-Fi network using Linux.

Step 1: Install Linux on your computer

First and foremost, you need to install Linux on your computer. There are various Linux distributions available, such as Ubuntu, Fedora, CentOS, and more. Choose the one that suits your needs and preferences and install it on your desktop or laptop.

Step 2: Install Network Manager

Network Manager is an excellent tool that allows you to manage and configure your network connections easily. It is pre-installed in most Linux distributions, but if you don't have it, install it using the following command:

sudo apt-get install network-manager-gnome

Step 3: Connect to Wi-Fi

With Network Manager, it's effortless to connect to a Wi-Fi network. Click on the Network icon on your desktop, select Wi-Fi, and choose the network you want to connect. Enter the password if required, and voila! You're now connected to the internet.

Step 4: Check Wi-Fi Status

To view the status of your Wi-Fi connection, open the terminal and run the following command:

nmcli dev wifi

You will see a list of all the available Wi-Fi networks, their signal strength, and connected status.

Step 5: Control Wi-Fi Network

Now that you're connected to your Wi-Fi network, it's time to customize it. Network Manager allows you to configure various settings such as IP addresses, DNS servers, SSID, security type, and more. To access the Wi-Fi network properties, click on the Wi-Fi icon on your desktop, select Wi-Fi Settings, and click on the gear icon next to your network. Here, you can modify the settings according to your requirements.

Step 6: Create Hotspot

Are you tired of paying for expensive mobile data plans? With Linux, you can create your own hotspot and share your internet connection. To create a hotspot, open the terminal and run the following command:

nmcli dev wifi hotspot ifname wlp2s0 ssid "Hotspot-Name" password "password"

Replace Hotspot-Name and password with your preferred SSID and password. Now, connect to the hotspot from your phone, tablet, or any other device, and enjoy the internet without any extra cost.

Conclusion

Controlling your Wi-Fi network using Linux is not as difficult as you might think. With Network Manager, it's effortless to manage your network connections and customize your Wi-Fi settings. We hope this guide has helped you learn how to control your Wi-Fi network using Linux. Try it out and see the difference for yourself.

{{< youtube Ezy1KTNF6dw >}} 



Is your Wi-Fi connection too slow? Are you having constant network problems while surfing the ‘Net? Chances are your wireless network is handling more traffic than it should. Luckily, it is quite easy to control your Wi-Fi network in Linux. You can use the open-source application evillimiter for monitoring and controlling device bandwidth. This guide illustrates how to do this using a step-by-step approach.
 
## What is Evillimiter?
 
Evillimiter is a free, open-source monitoring tool that can limit bandwidth usage for devices connected to a LAN. It runs on Linux and Windows and can work without administrative access to the network. Note: you should not use this tool on other people’s networks, avoiding possible legal challenges.
 
## How to Install Evillimiter
 
You need to install evillimiter before using it. Fortunately, the installation is straightforward if you have the dependencies installed already. It requires Python 3, which should be available on most Linux installations by default. To install evillimiter, fire up your terminal and type in the below commands:
 
## How to Control Your Wi-Fi Network Using Evillimiter
 
Once the installation finishes, you can start monitoring devices connected to your personal Wi-Fi. To do this, first start the application by running the following command:
 
Note that you will need sudo/root privileges to run and use evillimiter. This is because it handles the network controller and needs access to low-level kernel parameters. When you first run evillimiter, it will display some information about your Wi-Fi network. This includes the interface name, gateway IP, MAC, and netmask.
 
The interactive console is where you type in commands for monitoring bandwidth usage. Evillimiter offers a handful of commands for ease of control. You can view a list of available commands by entering ? or help in the interactive console.
 
You need to scan the local network before you can monitor connected devices. Use the scan command of evillimiter to do this.
 
This will scan for all hosts connected to your Wi-Fi and report the number of active devices. Now you can view the hosts and limit their bandwidth usage. Use the hosts command for viewing all active hosts.
 
This will display a list of devices that are connected to your Wi-Fi network. Evillimiter will assign an ID to each device and display its IP and MAC information. The status field shows whether bandwidth has already been limited for a device. 
 
You can now limit the bandwidth for a device by using the limit command.
 
This command limits the bandwidth of the second device(ID=2) to 100 kilobits. You can limit many devices at once using a comma-separated list.
 
This command will limit the bandwidth of the second and third devices to 50 kbit. 
 
The bandwidth limitation is set for both upload and download speeds. But you can also limit upload/download speeds separately. The next command limits the second device’s download speed to 100 kbit per second.
 
You can also block the Internet connection for a host device using the block command. That way, you can control Wi-Fi users directly from the terminal.
 
This command will block the second device from using network resources. Use the --upload and --download flags for blocking one-way traffic.
 
Say you want to stream gaming sessions. You can block all other Wi-Fi devices using the below command.
 
So far, we’ve shown how to scan, limit, and block devices using evillimiter in Linux. However, don’t forget to free these devices once you’re done. Use the free command followed by the host ID to do this.
 
To quit the interactive console, type in quit or exit in the command window.
 
It will exit the current session and bring back the terminal prompt. 
 
Next up are two more features of evillimiter. Since the interactive console is colored, it may not run properly in some environments. You can install the packages needed for color-coding or use the --colorless option in such cases.
 
If you run this in the terminal, it will start a colorless interactive session for evillimiter. People can use this mode whenever facing problems with ASCII colors. 
 
Finally, the -f option helps resolve issues with Linux iptables configuration or network parameters.
 
## Tips About Using Evillimiter
 
Evillimiter uses ARP spoofing and traffic shaping to cut users from LAN connections. Thus, it’s not a good idea to run this application in the background for too long. This can throttle network resources and may result in frequent kernel panics.
 
We recommend you use such tools only when it’s essential. Plus, the tool doesn’t work at all for IPv6 connections. Also, if you’re facing problems regarding network interfaces, try flashing the configuration.
 
## Wrapping Up
 
As you can see, you can easily control your Wi-Fi network in Linux using evillimiter. It’s effortless to install and works well even without admin access. If you want to learn more about Wi-Fi security, try reading the complete guide to home Wi-Fi security.
 
Rubaiat is a CS graduate who possesses hands-on experience with Unix Administration, Web Programming, DevOps, and Virtualization. He has a strong passion for enlightening people in open-source technologies.
 
Our latest tutorials delivered straight to your inbox




