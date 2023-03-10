---
title: "Unveiling the Secret: The Ultimate Guide to Tracking Any Application's Internet Activity on Windows!"
ShowToc: true 
date: "2022-11-15"
author: "Amanda Wiggins"
---
*****
# Unveiling the Secret: The Ultimate Guide to Tracking Any Application's Internet Activity on Windows!

In today's digital world, almost every application connects to the internet. Whether it’s your favorite social media app or your annual tax filing software, all applications transmit data to and from the internet. As a user, it is essential to understand what kind of data is being transmitted and to whom. This can be achieved by tracking the internet activity of applications on your Windows device.

But, can you track the internet activity of any application on your Windows device? The answer is yes, and in this guide, we will take you through the ultimate process of tracking any application's internet activity on Windows.

## Step 1: Using Resource Manager

Windows Resource Manager is a built-in tool that provides an overview of the real-time usage of your device. The tool can also help track the internet activity of individual applications. To access Resource Manager:

1. Press the shortcut keys “Ctrl + Shift + Esc” to open the Task Manager.

2. Click “More details” to open the full-screen Task Manager window.

3. Navigate to the “Performance” tab and click on “Open Resource Monitor” at the bottom.

4. In the Resource Monitor window, navigate to the “Network” tab.

5. Under the “Processes” section, you can see the list of applications' internet activity.

## Step 2: Using Command Prompt

Command Prompt is a Windows command-line tool that allows you to execute commands on your device. With Command Prompt, you can view the internet activity of an application in real-time by following these steps:

1. Type “cmd” in the Run box (accessible by pressing the Windows key + R).

2. Type “netstat -ab 5 > activity_report.txt” in the Command Prompt window (without quotes).

3. This command will create a report of all the internet activity on your device in real-time and save it in a text file named “activity_report” on your desktop.

4. To view the internet activity of an individual application, perform the following steps:

- Open the activity_report.text file.
- Use the “Ctrl + F” shortcut, type the name of the application you want to track, and click the “Find” button.
- You will see all the internet activity details of that application in the text file.

## Step 3: Using Third-Party Software

If you want a more user-friendly and comprehensive solution to track internet activity, there are many third-party software options available. Some of the popular ones include NetBalancer, Wireshark, and GlassWire. These tools are designed to monitor internet activity and provide detailed reports on bandwidth utilization, data usage, and individual application activity.

In summary, tracking internet activity is crucial as it helps keep your data safe and secure online. With the above steps, you can easily track the internet activity of any application on your Windows device. So, go ahead and try out the different methods to uncover the secret behind your application's internet activity!

{{< youtube XaT2UZ_sanw >}} 



Windows comes with built in performance monitors which can be used to track down different performance problems. For example, you can go to the Resource Monitor tool (from Windows Task Manager) which will give you a deeper look at which application are using which resource. You can easily identify the apps and close problematic apps if required. However, when it comes to detailed monitoring and reporting on which network resources are being requested and opened by a specific process, Windows default tools are unable to go into deeper analysis. You can see that Firefox or Internet Explorer is using the most Internet bandwidth but you will not know exactly which web pages and web components are being requested and opened by the application. This is where Fiddler comes in.

 
## Fiddler is the solution to complete Internet traffic analysis
 
If you are looking for an Internet/network traffic analysis tool, Fiddler is the perfect solution for you. Fiddler is a free application which can analyze and debug the Internet traffic and can do this for every single process. It comprehensively monitors, debugs and logs the Internet traffic (HTTP traffic). It will track all the communication and data exchanges between the local computer and the Internet servers. Setting up break points enable the users to see exactly what is being downloaded and uploaded from each application.
 
Fiddler can monitor any kind of Internet connection including HTTP, HTTPS, Proxy connections.
 
## Installation and usage
 
You can download Fiddler and then install it on your Windows computer. Installation is pretty easy and does not require any complex configurations. If you are using Fiddler in Windows 8, you will need to install “Enable Loopback” utility for Windows 8. The basic operations of Fiddler are easy to understand. When you start the program, you will get a two column window. The left column will show the web sessions and current connections which keep on scrolling as the new connections are logged. The right hand column will display detailed information about the selected connections from the left hand column. The right hand column also makes use of different tabs for additional details about the processes being monitored.
 

 
By default, Fiddler will monitor all the supported applications which are opened while Fiddler is running. To start monitoring a specific application, you will need to drag the “Any Process” icon from the toolbar and drop it to the application which needs to be monitored. In this way, Fiddler will filter out all the Internet traffic and will only display only the traffic of that specific application.
 
Let’s take an example to understand this concept clearly. I have opened Internet Explorer and am browsing through a site and downloading some files. I also have other browsers like Firefox and Google Chrome open but I only want to monitor the traffic from Internet Explorer. I will need to point my cursor to “Any Process” icon and then drop it to the Internet Explorer window. Please note that Fiddler will only log the traffic from that specific Internet Explorer window. If we look at the backend, we come to know that Fiddler monitors traffic from a specific process. If there are multiple processes of Internet Explorer (windows), then Fiddler will treat them as separate. If there is a single Internet Explorer process (tabs), then Fiddler will treat all open tabs in the single Internet Explorer window as one process.
 
## Final analysis
 
Fiddler is a great application for monitoring Internet traffic and troubleshoot any problems in the Internet usage. The basic operations of Fiddler can be used by technology professionals as well as normal computer user. The only problem with Fiddler is that we cannot specify a process by giving the Process ID. We will always need to use the drag n drop functionality in order to select a specific application for monitoring. This means that Fiddler can only be used for application which have a window but can not be used for those background processes that are using the Internet.
 
Download Fiddler
 
Fiddler comes with various addons in order to extend and enhance the functionality of the app.
 
Download Fiddler Addons
 
Usman is a technology enthusiast and loves tweaking Microsoft products. In addition to MakeTechEasier, he contributes regularly to iTechtics.com.
 
Our latest tutorials delivered straight to your inbox




