---
title: "You Won't Believe How Easy It Is To Reduce Your Internet Bill: Learn How To Limit Windows Update Bandwidth During Specific Hours!"
ShowToc: true 
date: "2023-02-08"
author: "John Granger"
---
*****
Introduction

As technology continues to evolve, internet usage has become a significant part of our daily lives. However, with this increased usage comes the increasing cost of internet bills. One major factor that contributes to high internet bills is excessive data usage caused by Windows updates. Fortunately, there is an easy way to reduce your internet bill and limit your computer's bandwidth during specific hours to prevent excessive data usage caused by Windows updates. In this article, we will show you how to limit Windows update bandwidth during specific hours.

Step One: Access the Windows Updates Settings

The first step to limit Windows update bandwidth is to access the Windows Updates settings. You can do this by clicking on the “Start” menu and searching for “Windows Update Settings” or by typing “Windows Update Settings” into the search bar.

Step Two: Click on “Advanced Options”

Once you have accessed the Windows updates settings, click on the “Advanced Options” button. Here, you will find the settings that allow you to limit Windows update bandwidth.

Step Three: Limit the Bandwidth During Specific Hours

In the “Advanced Options” section, scroll down to the “Delivery Optimization” tab. Here, you will find the option to limit the bandwidth usage during specific hours. Check the box next to “Limit how much bandwidth is used for downloading updates in the background” and then use the slider to set the time during which you want the download limit to be applied.

Step Four: Enable “Active Hours”

Another way to limit Windows update bandwidth during specific periods is by enabling the “Active Hours” feature. This feature allows you to set specific hours during which your computer is in use, thereby disabling any automatic Windows updates that may run in the background. To enable this feature, go back to the “Windows Update” section and click on the “Change Active Hours” button. From here, you can set the times during which your computer is in use.

Conclusion

Limiting Windows update bandwidth is an easy and effective method of reducing your internet bill. By following the above steps, you can easily limit the amount of data used by Windows updates during specific hours, resulting in significant savings on your internet bill. Take advantage of these simple settings and start reducing your data usage today!

{{< youtube Fg03d5A-0gY >}} 



Windows 10 lets you set limits on how much bandwidth it can use to download Windows and Store app updates. In most cases this is sufficient for most users. However, there are times when you just need to limit the bandwidth to specific hours of the day. Here is how to do that.
 
## Check Windows Version
 
This tip will only work if you are using Windows 10 with the April 2018 update. To know whether you’ve installed the April 2018 update or not, press Win + R, type winver and press Enter.
 
On the second line you will see the current Windows version number. It should be “1803” or higher.
 

 
## Set Background Download Limit
 
To set a background download limit in Windows 10, we need to configure some group policy settings.
 
1. First, press Win + R, type gpedit.msc and press Enter to open the Group Policy Editor. Once opened, go to “Computer Configuration -> Administrative Templates -> Windows Components -> Delivery Optimization.”
 
2. On the right panel scroll all the way down, find the “Set Business Hours to Limit Background Download Bandwidth” policy and double-click on it.
 
3. In the policy settings Windows select the “Enabled” option. This will enable a few options under the “Options” category.
 
Configure them as follows:
 
- Select the “From” and “To” times under “Set business hours to limit background download bandwidth.” In my case I’m selecting the time as 8AM to 10PM. That way I can restrict Windows from downloading in the background all day.
 - Enter the maximum bandwidth percentage you would like Windows to use during the restricted hours. I’m allowing Windows to use twenty-five percent of the total bandwidth available to my system. You can set yours depending on your Internet connection speed.
 - Leave the third input as “0” so that Windows can download updates in the background without any bandwidth restrictions outside the restricted hours. But, if need be, enter a percentage value to restrict background downloading outside restricted hours.

 
4. Click on the “OK” button to save changes and restart the system to make the changes take effect.
 
## Set Foreground Download Limit
 
1. To set restrictions of foreground downloads, open Group Policy Editor and go to “Computer Configuration -> Administrative Templates -> Windows Components > Delivery Optimization.” Find “Set Business Hours to Limit Foreground Download Bandwidth,” and double-click on it.
 
2. Select “Enabled” and notice the same options as in the previous policy settings. Set the From and To times, maximum bandwidth you would like to allow during restricted hours, and maximum bandwidth you would like to allow outside restricted hours.
 
3. Once you are done setting this up, click on the “OK” button to save changes.
 
Finally, restart your system, and Windows will limit all background and foreground downloading activities based on your settings.
 
To revert the changes, open the policy settings, and either select “Not configured” or “Disabled.” This action will remove the download restrictions.
 
Using the above settings you can restrict Windows from hogging all the bandwidth while you are working or gaming. Comment below sharing your thoughts and experiences regarding using the above methods to limit background and foreground Windows updates.
 
Vamsi is a tech and WordPress geek who enjoys writing how-to guides and messing with his computer and software in general. When not writing for MTE, he writes for he shares tips, tricks, and lifehacks on his own blog Stugon.
 
Our latest tutorials delivered straight to your inbox




