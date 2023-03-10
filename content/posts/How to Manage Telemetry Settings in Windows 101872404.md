---
title: "Is Windows 10 Spying On You? Learn How To Protect Your Privacy By Managing Telemetry Settings!"
ShowToc: true 
date: "2023-03-26"
author: "Kimberly Wilson"
---
*****
Is Windows 10 Spying On You? Learn How To Protect Your Privacy By Managing Telemetry Settings!

Windows 10 is one of the most popular operating systems out there. It has been praised for many features that make it comfortable and convenient to use. These features, however, come with a cost: privacy. Some people worry that Windows 10 might be spying on them, collecting data without their knowledge. In this article, we will look at what telemetry is and how you can manage it to protect your privacy.

What is Telemetry?

Telemetry is a feature in Windows 10 that collects diagnostic and usage data from your computer. This data is then sent to Microsoft to help improve the operating system. Telemetry is not unique to Windows 10, but it has become a hot topic because of the way it has been implemented in this particular operating system.

Is Telemetry Spying?

Telemetry is not necessarily spying. It is a standard feature found in many modern operating systems, and it is used to help software developers better understand how their products are being used. The issue that some people have with Windows 10's telemetry is its level of invasiveness. Some users may feel uncomfortable with how much data is being collected and sent to Microsoft.

How to Manage Telemetry Settings

Fortunately, Microsoft has provided users with a way to manage their telemetry settings. Here's how you can do it:

Step 1: Open the Settings app by clicking the Start button and then clicking the gear icon.

Step 2: Click on Privacy.

Step 3: Scroll down and click on Feedback & diagnostics.

Step 4: You will see three options: Basic, Enhanced, and Full. Basic is the least invasive, while Full is the most invasive. You can choose which setting you are most comfortable with.

Step 5: If you want to turn off telemetry completely, you can use a third-party tool like O&O ShutUp10.

Conclusion

In conclusion, Windows 10's telemetry is not necessarily spying. It is a tool that helps software developers improve their products. However, some users may feel uncomfortable with how much data is being collected and sent to Microsoft. Fortunately, there are ways to manage your telemetry settings to protect your privacy. Give it a shot and see if it makes you feel better!

{{< youtube O1SfdjeWVSk >}} 



Windows 10 has many new features like the Edge browser, Cortana, new and improved Start menu, improved security, etc. In fact, Windows 10 is one of the best releases to date. Besides  all the new features, Windows 10 collects a lot of data using the new Telemetry feature. The Telemetry feature in Windows 10 is enabled and set to “Full” by default. Unless you are using the Enterprise version of Windows 10, you cannot disable the Telemetry feature completely using the default options. However, you can certainly restrict the telemetry feature using the methods shown below.
 
## Manage Telemetry Levels
 
Generally, you can manage the telemetry settings directly from the Windows 10 Settings app. To do that click on the Notifications icon on the taskbar and then click on the “All Settings” button.
 

 
Once the settings panel has been opened, select the option “Privacy.”
 
Here in the privacy window navigate to “Feedback and diagnostics,” and select the telemetry level from the drop-down menu under “Send your device data to Microsoft.” “Basic” is the lowest possible setting.
 
If you are managing multiple systems, then it is a good idea to use the group policy editor. To start, press “Win + R,” type gpedit.msc and press the Enter button.
 
In the Group Policy Editor, navigate to “Computer Configuration -> Administrative Templates -> Windows Components -> Data Collection And Preview Builds” and double-click on the policy “Allow Telemetry” appearing on the right pane.
 
Here in this window select the “Enabled” checkbox. This action will enable a drop-down box in the Options panel. From the drop-down menu select the “Basic” option if you want to set the telemetry to the lowest level possible, and click on the “Ok” button to save the changes.
 
Note: the “Security” option in the drop-down menu is only applicable to the enterprise version of Windows. For non-enterprise versions the telemetry settings will default to “Basic” even if you select the “Security” option.
 
If you don’t have access to the group policy editor, then you can do the same using the Windows Registry Editor. To start, press “Win + R,” type regedit and press the Enter button.
 
Navigate to the following key:
 
On the right pane right-click and select the “New” option and then “DWORD (32-bit Value).”
 
The above action will create a new value. Name the new value “AllowTelemetry,” and press the Enter button.
 
Now, double-click on the newly created value, and enter a value data of “1” for the lowest possible telemetry settings for Pro and Home users. Below are the additional settings that you can set.
 
- 0 – Security (Enterprise version only)
 - 1 – Basic
 - 2 – Enhanced
 - 3 – Full

 
That’s it. Just restart your system to make the changes take effect.
 
## Disable Telemetry in Windows 10
 
If you want to completely disable the Windows 10 telemetry then you can do that by simply disabling the relevant service from starting at every Windows startup. You can do that using Windows Services. Press “Win + R,” type services.msc and press the Enter button.
 
The above action will open the Services window. Here, find and double-click on the service “Connected User Experiences and Telemetry.”
 
In the services properties window, click on the “Stop” button to stop the running service, select the option “Disable” from the drop-down menu next to “Startup type” and then click on the “Ok”  button to save the changes.
 
Do comment below sharing your thoughts and experiences about using the above methods to manage telemetry in Windows 10.
 
Vamsi is a tech and WordPress geek who enjoys writing how-to guides and messing with his computer and software in general. When not writing for MTE, he writes for he shares tips, tricks, and lifehacks on his own blog Stugon.
 
Our latest tutorials delivered straight to your inbox




