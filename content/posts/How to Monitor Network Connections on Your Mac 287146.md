---
title: "Uncover the Secret Connections Hiding on Your Mac with this Network Monitoring Trick!"
ShowToc: true 
date: "2023-06-20"
author: "Joseph Johnson"
---
*****
# Uncover the Secret Connections Hiding on Your Mac with this Network Monitoring Trick!

Have you ever wondered what connections are being made from your Mac to other devices, servers or websites? It’s easy to check your recent network activity through your Mac’s built-in activity monitor, but this doesn’t give you a comprehensive overview of all the connections that your Mac is making. In this article, we’ll teach you a trick to uncover the secret connections that are hiding on your Mac using network monitoring.

First, let’s start with the basics. When your Mac is connected to a network, it’s constantly communicating with other devices, servers and websites. These connections can either be incoming or outgoing, and they’re often used for things like sending and receiving data, checking for software updates, and syncing your files with cloud services.

However, not all of these connections are beneficial or harmless. Hackers and malware can use hidden connections to steal your information, take control of your Mac, or use it as a bot to send spam or launch cyber-attacks. That’s why it’s crucial to monitor your network activity and investigate any suspicious connections.

So, how can you monitor your Mac’s network activity? One way is to use a third-party network monitoring tool. There are many options available, both free and paid, that can give you real-time insights into your Mac’s network traffic, including the IP addresses, ports, protocols and data transmissions. Some popular tools include Little Snitch, Wireshark, and Charles Proxy.

However, if you’re looking for a quick and easy way to get started with network monitoring, you can use a built-in utility in your Mac called Terminal. Terminal is a command-line interface that allows you to interact with your Mac’s operating system and run various commands.

To check your network connections in Terminal, follow these steps:

1. Open Terminal by searching for it in Spotlight or navigating to Applications -> Utilities -> Terminal.

2. Type in the following command and press Enter:

    `sudo lsof -i -P | grep -i "listen\|established"`

This command will display a list of all the network connections that your Mac is currently making, both inbound (listen) and outbound (established). The output will include the process ID (PID), protocol type (TCP or UDP), local and remote IP addresses, and corresponding ports.

3. Take a closer look at the connections to identify any suspicious or unknown IP addresses or ports. You can use online resources like IP address lookup tools or port scanners to learn more about the endpoints and their reputation.

4. If you want to see the network activity in real-time, you can use the `top` command to display the active processes that are using the most network bandwidth. Type in `top -o recv` to sort the processes by the amount of data they’re receiving, or `top -o sent` to sort them by the amount of data they’re sending.

With this network monitoring trick, you can unveil the secret connections that are hiding on your Mac and protect yourself from potential security threats. Just remember to practice safe browsing habits, keep your software up to date, and use a trusted antivirus program to stay one step ahead of the bad guys. Happy monitoring!

{{< youtube AOHI9U8phDw >}} 



Sometimes your Mac’s network activity can seem like a black box. There aren’t that many system tools for analyzing network activity, and Terminal commands like netstat vomit a ton of data that’s hard to sort through and understand. Fortunately, you’re not the only one that wants to find and control the apps using your network connection on macOS. You can check out these following options for managing your network connection on your Mac.
 
## Using Activity Monitor
 
If you want an extremely rough overview of the apps using your network connection, you can find that under the Network tab in Activity Monitor.
 
1. Open Activity Monitor from “/Applications/Utilities/Activity Monitor.app” or type “Activity Monitor” into Spotlight.
 

 
2. Click the “Network” tab at the top of the Activity Monitor window.
 
3. To see the most active processes, click the column titled “Sent Bytes” to see the processes sorted in order of amount of data sent.
 
4. You can also click on other column titles to sort by data received and packets sent and received.
 
## Using Loading
 
Loading is a free menu bar application that monitors the applications currently using your Internet connection. It also displays the apps that have recently used your Internet connection and has options for detailed breakouts of traffic. All this lives in a tiny menu bar app, and it’s free, too!
 
1. Download and install Loading from the developer’s website.
 
2. If your Internet connection is currently active, you’ll notice a new addition to your menu bar: a spinning loading icon. This indicates that there is traffic on your network.
 
3. Click on the Loading icon to reveal a dropdown menu. Under “Loading” you’ll see applications currently loading content over your Internet connection. Under “Loaded,” on the other hand, you’ll see apps that recently finished downloading content.
 
4. Hold the Alt/Option key on your keyboard while clicking the Loading menu bar icon to reveal a much more detailed dropdown menu. This shows the process identifier (PID) for each application as well as each application’s resource path.
 
5. You can use the PID to kill a misbehaving application with a Terminal command like kill 410. That particular command would kill Spotify, which is PID 410 at the moment. Replace that with the process number of the app you want to kill.
 
## Using Radio Silence
 
Radio Silence is a paid app that allows you to block Internet access for specific applications and processes. It also allows for real-time monitoring of Internet traffic. A trial is available, but the app only costs $9.
 
1. Download and install Radio Silence from the developer’s website.
 
2. Open Radio Silence.
 
3. Click the “Network Monitor” tab.
 
4. At first the tab will be blank. But after a couple seconds, applications connecting to the Internet will appear.
 
5. In addition to this list you’ll see the number to active connections next to each application in a gray bubble. Next to that is a button that blocks an application from connecting to the Internet. This “Block” button will add an application to Radio Silence’s blacklist, prohibiting any future incoming or outgoing network connections.
 
## Using Little Snitch
 
For total insight into and complete control over your Mac’s Internet connection, you’ll want to use Little Snitch. It’s a paid app, but it provides enormous control, allowing you to block or allow traffic on a process-by-process basis.
 
1. Download and install Little Snitch from the developer’s website. You’ll need to reboot your Mac during the installation process for Little Snitch to insert its network monitoring daemons.
 
2. Little Snitch’s tutorial is helpful, so click through it to learn how the app works. We care most about the Network Monitor, which should launch automatically when the tour finishes. If you need to launch the monitor manually, click on the Little Snitch icon in the menu bar and choose “Show Network Monitor” from the dropdown menu.
 
3. The Network Monitor will display all the active connections and their associated applications.
 
4. Click on an application or process name to learn more about what the process does.
 
5. To block a process, click the “X” next to the process’s name.
 
## Conclusion
 
While macOS doesn’t offer many built-in tools to monitor the network connection in a useful way, there are a number of third-party applications that fill in the void. If you need serious management of your Internet connectivity, you’ll want to use Little Snitch. If you have a casual interest in your network activity, Loading will be less of an investment.
 
Alexander Fox is a tech and science writer based in Philadelphia, PA with one cat, three Macs and more USB cables than he could ever use.
 
Our latest tutorials delivered straight to your inbox




