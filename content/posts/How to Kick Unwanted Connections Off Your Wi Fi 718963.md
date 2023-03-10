---
title: "Say Goodbye to Wi-Fi Leeches Forever with This One Simple Trick!"
ShowToc: true 
date: "2023-01-13"
author: "Marcel Silva"
---
*****
Say Goodbye to Wi-Fi Leeches Forever with This One Simple Trick!

Are you fed up with slow and sluggish Wi-Fi speeds? Do you find your internet connection constantly dropping out or buffering? Chances are that you have some Wi-Fi leeches in your vicinity. These are the people who piggyback on your Wi-Fi without your permission, causing your internet speeds to slow down significantly. But don't worry, we have a simple trick to solve this problem once and for all.

Step 1: Log into your router

First things first, you need to log into your router to access its settings page. Usually, you can do this by opening a web browser and typing in your router's IP address (e.g. 192.168.1.1) in the address bar. You will then be prompted to enter your username and password, which should be located on the underside of your router.

Step 2: Change your Wi-Fi password

Once you've logged into your router, look for the "Wireless Settings" or "Wi-Fi Settings" page. Here, you will find your current Wi-Fi network name (SSID) and password, along with other settings. To get rid of Wi-Fi leeches, simply change your Wi-Fi password to a strong, unique password that only you know. This will prevent anyone from accessing your Wi-Fi network without your permission.

Step 3: Enable MAC address filtering

If you want to take things a step further, you can enable MAC address filtering on your router. MAC address filtering is a security feature that allows you to create a whitelist of devices that are allowed to connect to your Wi-Fi network. To do this, you need to find the "Wireless MAC Filter" or "MAC Address Filtering" page on your router settings. From here, you can add the MAC addresses of all the devices that you want to allow on your Wi-Fi network. Any device that is not on this list will be automatically blocked from accessing your Wi-Fi network.

Step 4: Restart your router

After making these changes, don't forget to restart your router to apply the new settings. This will ensure that all the changes you've made take effect immediately.

By following these simple steps, you can say goodbye to Wi-Fi leeches forever. Not only will this improve your internet speeds, but it will also give you peace of mind knowing that your Wi-Fi network is secured. So why wait? Take action now and enjoy lightning-fast internet speeds!

{{< youtube jpw2ebhTSKs >}} 



If you are trying to surf the Web and experiencing slow network speed due to bandwidth congestion, it’s probably due to too many devices connected to your router. Chances are, some of these devices are not yours. Once you share your Wi-Fi password with someone or log on to your Wi-Fi on someone else’s device, the password remains with them. It opens up the possibility to log back in to your Wi-Fi connection without your permission. Unwanted connections can pose several security and privacy threats, so it is a good practice to keep filtering the connected devices on your Wi-Fi.
 
## Why Disconnecting People from Your Wi-Fi Is a Good Idea
 
Having unwanted people sharing your Wi-Fi connection has the potential to whip up some serious problems. Someone with the wrong intent and skillset could steal your personal information if they gain access to your private network.
 
It also opens up the potential risk of compromising your webcam and microphone, which can put your privacy at risk.
 
Also, having more people connected to your network can cause bandwidth congestion, which can slow down your Internet speed. Additionally, if you are on a limited data plan, you might suffer unwanted charges for the data they have consumed.
 
## Find Your Router’s IP Address
 
Before doing anything, you need to know the address to access your Wi-Fi router’s admin panel. In most cases, it’s one of the following:
 
- 192.168.1.1192.168.0.1192.168.2.1192.168.1.254192.168.10.1192.168.11.1192.168.123.254192.168.3.110.0.0.1192.168.8.1

 
However, to find out which one’s yours:
 
- Search for “CMD” and run Command Prompt as admin.

 
- Enter the following command: ipconfig

 
- Command Prompt will print out a bunch of information about your network. Find and copy the default gateway address from here.

 
- Enter the default gateway address in your browser’s search bar to be redirected to the admin panel of your Wi-Fi router.

 
## 3 Ways to Remove Unwanted Connections from Your Wi-Fi Network 
 
Now that you know your IP address, you can remove unwanted connections from your network with one of the three methods below:
 
## 1. Use MAC Filtering
 
Every device that connects to the Internet has a 48-bit address associated with it, which is known as a MAC address. Use this MAC address to identify and block certain devices to connect to your Wi-Fi network. 
 
To do that, you need to access your Wi-Fi’s admin panel and navigate to the tab where all the connected devices are listed. You can see all the connections, along with their details. In some cases, these details also include the MAC address of the connected devices.
 
### Find Your MAC Address
 
All routers do not use the same software, so you may only be given the device’s IP address. Luckily, we can easily find the MAC address of a device using its IP address and a few commands. Follow the steps below: 
 
- Log in to your router’s admin panel and navigate to the list of connected devices by clicking on “Parental Controls.” Copy the IP address of the device in question.

 
- Right-click on the Start button and open the Windows Terminal app as administrator.

 
- Type the following command: ping "IP address"

 
- After a few print statements are displayed, enter the second command arp -a

 
- The ARP command lists detailed information about the device you targeted via its IP address. The MAC address will be mentioned next to the device’s IP address. In this example, the IP address is 192.168.0.1, and the MAC address is 50-2b-73-87-a3-20.

 
### Use the MAC Address to Block Unwanted Connections
 
Now that you have the MAC address of the device you want to block from your Wi-Fi network, head back to the router’s admin panel and follow the steps below to blacklist it.
 
- Navigate to the MAC address filtering section. Where you will find these settings depends on your admin panel’s UI. Most of the time they will be in the Security or Advanced settings tab. In our case, it was in the Advanced tab.

 
- Set your Filter Mode as “Blacklist” (at the top).Enter the MAC address of the device you want to blacklist in the “Blacklisted MAC Address” field and add it to the list by pressing on the “+” button underneath “Operation.”

 
- Make sure to save your changes before closing the tab by pressing “OK.”

 
## 2. Only Enable Whitelisted Devices
 
While blacklisting a device completely bans it from connecting to your network, hackers can always join back in using another device. To prevent such a situation, a much more secure approach would be to whitelist the MAC addresses of select devices.
 
Basically, you can tell your router to only allow certain devices and automatically block any other connection requests. Here’s how to whitelist your trusted devices.
 
- Navigate to MAC address filtering options on your router’s admin panel and select the whitelist option instead of blacklist. This step may not be the same for you, as every router has a different UI, but the concept remains the same. With some routers like those of D-Link, you get another section of settings dedicated to whitelisting devices instead of a switch between the two functions.

 
- Just as we added a MAC address in the field below to blacklist it, enter the MAC address of the device you want to whitelist and add it to the list by pressing on the “+” button on the right. Alternatively, you can select the “Whitelist all the online devices” option.

 
- Finally, save the changes you’ve made, and only the devices added to this list will be able to access your Wi-Fi network.

 
## 3. Change Wi-Fi Password or SSID
 
If you don’t want to go through the hassle of blacklisting or whitelisting a device, you can simply change your Wi-Fi’s name or password. All the devices connected to your network will be automatically logged out. Reconnect your trusted devices by entering the new password.
 
- Head to your router’s admin panel and navigate to the settings menu to find the option to change your Wi-Fi’s name or password. In most cases, these settings are in the Security tab or the WLAN settings section.To change your Wi-Fi’s name, simply enter a new name in the Wi-Fi name box. You can set different names for your 2.4GHz and 5GHz band.

 
- Similarly, to change your Wi-Fi’s password, enter a new password in the Wi-Fi password box. Make sure to set a strong new password that is a mixture of both upper case and lower case letters, numbers, and symbols, to make it harder for people to guess or software to crack. Click “OK.”

 
- Save your settings to finalize your changes by pressing “OK.”

 
## Frequently Asked Questions
 
### 1. What is the best security encryption for my Wi-Fi?
 
WPA3 is the latest and most secure Wi-Fi encryption protocol available in 2022. Do note that many Wi-Fi routers don’t yet support it.
 
### 2. How can I identify if someone is using my Wi-Fi without going through the router admin panel?
 
There are many ways to tell if someone has unauthorized access to your Wi-Fi network:
 
- If you are experiencing poor speed, it could mean that your broadband is being stretched over multiple devices. If the speed doesn’t increase even after you disconnect all the devices from your end, it could very well mean that someone else is using your Wi-Fi network.High latency while playing online multiplayer games or connecting over a video call.If your Wi-Fi is rebooting multiple times by itself, it could mean that someone else is trying to brute-force their way into hacking your network.If your Wi-Fi network does not display WPA protection anymore, it could mean that it has been compromised and that someone is already inside your network.

 
### 3. Is there software that I can use to monitor the devices connected to my network?
 
There are many software you can use to kick an unknown device off your Wi-Fi networks, such as JamWiFi or Netcut. But these apps are only temporary solutions and the same as executing a simple Wi-Fi de-authentication attack, which does not permanently ban someone. However, it can log them off temporarily.
 
Image credits: Unsplash
 
Ojash has been writing about tech back since Symbian-based Nokia was the closest thing to a smartphone. He spends most of his time writing, researching, or ranting about bitcoin.
 
Our latest tutorials delivered straight to your inbox




