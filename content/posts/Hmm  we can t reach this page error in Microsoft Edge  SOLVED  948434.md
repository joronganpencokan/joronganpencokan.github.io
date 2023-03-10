---
title: "You won't believe how we solved the 'Hmm, we can't reach this page' error in Microsoft Edge - click to find out!"
ShowToc: true 
date: "2023-05-22"
author: "Judy Jarrette"
---
*****
Title: You won't believe how we solved the 'Hmm, we can't reach this page' error in Microsoft Edge - click to find out!

Are you tired of seeing the dreaded 'Hmm, we can't reach this page' error message on Microsoft Edge when trying to access a website? Don't worry; you're not alone! This error can be frustrating, especially if you need to access important information quickly. But today, we have good news for you. We've come up with a solution to this error that will blow your mind - and it's so simple you won't believe it!

Step 1: Clear your browsing history and cache

The first thing you should try when encountering the 'Hmm, we can't reach this page' error is to clear your browsing history and cache. This usually solves the issue and allows you to access the website you're trying to reach. To clear your cache and history, follow these steps:

1. Click on the three dots in the upper-right corner of your Edge browser window.
2. Select the History option from the dropdown menu.
3. Click on the Clear browsing data option.
4. Choose the time range for which you want to delete history and cache files (e.g., Last hour, Last day, All time).
5. Check the boxes for browsing history, cookies and other site data, and cached images and files.
6. Click on the Clear data button.

Step 2: Disable your VPN or Proxy server

If clearing your browsing history and cache didn't solve the issue, your next step is to disable your VPN or proxy server. Sometimes, these can interfere with your browser and cause the 'Hmm, we can't reach this page' error. To disable your VPN or proxy server, follow these steps:

1. Click on the three dots in the upper-right corner of your Edge browser window.
2. Select the Settings option from the dropdown menu.
3. Scroll down to the System section and click on the Open proxy settings option.
4. In the Proxy settings window, turn off the switch for 'Use a proxy server.'
5. Try accessing the website again to check if the error is fixed.

Step 3: Restart your computer

If the first two steps didn't work, try restarting your computer. This can help refresh your system and clear any temporary glitches that may be causing the error. Once your system restarts, try accessing the website again.

Step 4: Check your internet connection

If the first three steps didn't work, the issue might be due to a problem with your internet connection. Check if your device is connected to the internet and if the signal strength is strong enough. If your settings are correct, try resetting your router, modem, or any other device you're using to connect to the internet.

Conclusion

The 'Hmm, we can't reach this page' error can be annoying, but it doesn't have to ruin your browsing experience. By following these steps, you can easily troubleshoot the error and access the website you need. Remember to clear your cache and history, disable your VPN or proxy server, restart your computer, and check your internet connection. We hope these tips helped you solve the issue and improve your browsing experience on Microsoft Edge!

{{< youtube X17mPLRuUQs >}} 



Fix Hmm, we can’t reach this page error in Microsoft Edge: If you are not able to access any webpage or website in Microsoft Edge because of “Hmm, we can’t reach this page” error and other browsers or apps works fine in Windows 10 then it means there is some serious problem with Microsoft Edge/System. In short, you will be able to access internet on Chrome or Firefox and all the Windows Store apps will work but you won’t be able to use Edge to browse Internet until and unless you fix the underlying issue.
 

 
Now Microsoft is a default Web browser which comes pre-installed with Windows this means you can’t uninstall it or even re-install it. Now the main cause of this error seems to be DNS, if the DNS client is somehow disabled then Edge will definitely respond this way. Anyway, without wasting any time let’s see how to actually Fix Hmm, we can’t reach this page error in Microsoft Edge with the help of below-listed troubleshooting steps.
 
## Hmm, we can’t reach this page error in Microsoft Edge [SOLVED]
 
Make sure to create a restore point just in case something goes wrong.
 
Contents
 
- Hmm, we can’t reach this page error in Microsoft Edge [SOLVED]
 - Method 1: Make sure DNS Client is running
 - Method 2: Use Google DNS
 - Method 3: Disable IPv6
 - Method 4: Run Microsoft Edge without Add-ons
 - Method 5: Change your network from Public to Private or vice verse

 
#### Method 1: Make sure DNS Client is running
 
1.Press Windows Key + R then type services.msc and hit Enter.
 
2.Find DNS Client in the list and then double-click on it to open its properties.
 
3.Make sure the Startup type is set to Automatic and click Start if the service is not already running.
 
4.Click Apply followed by OK.
 
5.Reboot your PC to save changes.
 
#### Method 2: Use Google DNS
 
1.Open Control Panel and click on Network and Internet.
 
2.Next, click Network and Sharing Center then click on Change adapter settings.
 
3.Select your Wi-Fi then double click on it and select Properties.
 
4.Now select Internet Protocol Version 4 (TCP/IPv4) and click Properties.
 
5.Checkmark “Use the following DNS server addresses” and type the following:
 
Preferred DNS server: 8.8.8.8
Alternate DNS server: 8.8.4.4
 
6.Close everything and you may be able to Fix Hmm, we can’t reach this page error in Microsoft Edge.
 
#### Method 3: Disable IPv6
 
1.Right click on WiFi icon on system tray and then click on “Open Network and Sharing Center.“
 
2.Now click on your current connection in order to open settings.
Note: If you can’t connect to your network then use Ethernet cable to connect and then follow this step.
 
3.Click Properties button in the window that just open.
 
4.Make sure to uncheck Internet Protocol Version 6 (TCP/IP).
 
5.Click OK then click Close. Reboot your PC to save changes.
 
#### Method 4: Run Microsoft Edge without Add-ons
 
1.Press Windows Key + R then type regedit and hit Enter to open Registry Editor.
 
2.Navigate to the following registry path:
 
HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft
 
3.Right-click the Microsoft (folder) key then select New > Key.
 
4.Name this new key as MicrosoftEdge and hit Enter.
 
5.Now right-click on MicrosoftEdge key and select New > DWORD (32-bit) Value.
 
6.Name this new DWORD as ExtensionsEnabled and press Enter.
 
7.Double click on ExtensionsEnabled DWORD and set it’s value to 0 in value data field.
 
8.Click OK and reboot your PC to save changes and see if you’re able to Fix Hmm, we can’t reach this page error in Microsoft Edge.
 
#### Method 5: Change your network from Public to Private or vice verse
 
2.Navigate to the following Registry Key:
 
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\NetworkList\Profiles
 
3.Now under Profiles, there would be many subkeys, you need to find your current network connection (you will see the name of your network connection under Description).
 
4.From the left-hand window pane select the subkeys under profiles in the right window pane look under description to find your current network connection.
 
5.Once you have successfully located your network connection profile, double-click on Category DWORD.
 
6.Now if the registry value is set to 1 then change it to 0 or if it’s set to 0 then change it to 1.
 
0 means Public
1 means Private
 
7.Reboot your PC to save changes and again try to access the website in Edge.
 
8.If the error is still there then again follow the same steps to again change your network profile.
 
Recommended for you:
 
- Fix ERR_QUIC_PROTOCOL_ERROR in Chrome
 - Fix The Installation Failed In The First Boot Phase Error
 - How To Fix Windows Update Error 8024402F
 - Fix ERR_NETWORK_CHANGED in Chrome

 
That’s it you have successfully Fix Hmm, we can’t reach this page error in Microsoft Edge but if you still have any queries regarding this guide then feel free to ask them in the comment’s section.




