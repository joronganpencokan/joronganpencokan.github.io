---
title: "You won't believe the one registry tweak that drastically improves Surface S touch responsiveness! Click now to upgrade your device's performance!"
ShowToc: true 
date: "2023-05-10"
author: "Pat Simmons"
---
*****
You Won't Believe the One Registry Tweak That Drastically Improves Surface S Touch Responsiveness

If you're a proud owner of Microsoft Surface S, you know how important touch sensitivity is to an optimal user experience. However, all too often, touch responsiveness can falter, causing frustration and annoyance. If this is something you've experienced, you're not alone. Fortunately, there's a single registry tweak that can drastically improve the touch responsiveness of your Surface S. 

Before we dive into the registry tweak, it's necessary to understand what's causing the faltering responsiveness. As an electronic device, the Surface S relies on various processes to function optimally. One such process, called the "Polling Rate," is responsible for how frequently the device detects and responds to touch. The default Polling Rate on the Surface S is set to 100Hz, which, while adequate for everyday use, can result in sluggishness and delayed responsiveness in high-pressure situations. 

The registry tweak that we'll be discussing today involves adjusting the Polling Rate to a higher frequency. This process can be daunting at first, but if followed carefully, you can improve touch sensitivity without much trouble. 

If you are not familiar with the registry system of your computer, it is advisable to back up your registry before following the procedure. You do not want to cause problems that could affect your machine negatively. 

Now, to begin, press the "Windows" key and "R" key simultaneously. Type "regedit" and press enter. Navigate to "HKEY_LOCAL_MACHINE > SYSTEM > CurrentControlSet > \Control\Class\{745A17A0-74D3-11D0-B6FE-00A0C90F57DA}\0000."

Inside the folder, you will see several values, but the one of interest for us is "PollingInterval." By default, it's set to 1000 milliseconds. Double click on it and then set its value anywhere between 0 and the maximum range. A value between 1 and 99 is recommended for optimal performance. 

Once you've inputted the desired value, save, and then reboot your Surface S. Upon booting up, you should notice a significant improvement in touch sensitivity. Congratulations, you've successfully improved your Surface S touch responsiveness! 

In conclusion, the Surface S is an excellent device for productivity and entertainment. However, it's not uncommon to experience touch sensitivity issues that can be remedied with a simple registry tweak. By following the steps outlined above, you can positively impact the way you interact with your Surface S. Go ahead, give it a try, and experience an even more responsive device today!

{{< youtube x74eu7mQAnA >}} 



When it comes to improving your PC in some way, sometimes simple tweaks are just worth trying. This is the case of a recently uncovered method that allows to make Microsoft Surface tablet more touch responsive by simply modifying the Windows 8 Registry.
 
The finding appeared at the XDA Developers Forum by user tamarasu, and it involves the modification of a registry key. So far, many people found that the tweak works and it is something easy to do. If you want to give it a try, here are the step-by-step:
 
## Instructions
 
1. While in the Start screen, do search for regedit, right-click it and click or tap Run as administrator from the app command.
 
2. Locate the following registry key:
 
3. Change the Latency value (DWORD) from 8 to 2.
 
4. Change the SampleTime value (DWORD) from 8 to 2.
 

 
5. Restart Surface and test.
 
Be aware that Microsoft has spent countless hours fine-tuning its tablet and while the community is finding that the tweak indeed helps to increase the touch responsiveness, it could also affect the battery life of the device, even more on power-users, as the XDA forum member, GooDayToDie, points out  “the system must poll the touchscreen more often”.
 
If it works for you too, let us know in the comments, we’d like to know. And I am also curious how this works with any touch-enabled devices running Windows 8; that would be something really interesting.
 
Source XDA Developers forum | header image Microsoft




