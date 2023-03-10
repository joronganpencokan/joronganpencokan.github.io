---
title: "STOP Your Screen From Going BLACK! Learn How to Keep Windows 10 Screen On NOW!"
ShowToc: true 
date: "2023-01-29"
author: "Brian Israel"
---
*****
Title: "STOP Your Screen From Going BLACK! Learn How to Keep Windows 10 Screen On NOW!"

Introduction:
If you're like most people, you probably find it frustrating when your Windows 10 screen goes black and locks you out, especially if you're trying to complete an important task or watch a movie. Fortunately, you don't have to endure this inconvenience anymore. In this article, we'll be discussing various ways you can keep your Windows 10 screen on and prevent it from going black.

Method 1: Use the Mouse or Keyboard
One of the easiest ways to prevent your Windows 10 screen from going black is to move your mouse or hit a key on your keyboard periodically. Windows 10 comes with a built-in feature that turns off the screen after a certain period of inactivity. By moving your mouse or typing on your keyboard, you'll be resetting the timer and keeping your screen on.

Method 2: Change Power Settings
If you're not a fan of constantly moving your mouse or pressing keys, you can change your power settings to prevent your screen from going black. Here's how:

Step 1: Type "Power & sleep settings" in the search bar and open the settings app.
Step 2: Click on "Additional power settings" at the bottom of the page.
Step 3: Click on "Change plan settings" beside your selected power plan.
Step 4: Click on "Change advanced power settings."
Step 5: Scroll down to "Display" and click on the plus sign beside it to expand.
Step 6: Expand "Turn off display after" and set the value to "0" for "On battery" and "Plugged in."
Step 7: Click on "Apply" and "OK."

By changing your power settings, your Windows 10 screen will never go black due to inactivity.

Method 3: Install Third-Party Software
In case the above methods don't work for you or you just want to try something different, you can install third-party software to keep your Windows 10 screen on. Some examples of such software are Caffeine, Insomnia, and Mouse Jiggler. These programs work by simulating mouse movements at regular intervals, which keeps your screen on.

Conclusion:
There you have it! Three simple and effective ways to keep your Windows 10 screen on and prevent it from going black. Whether you choose to use the mouse, change power settings, or install third-party software, these methods will save you from the inconvenience of having to constantly wake your screen up. Give them a try and enjoy uninterrupted computer usage.

{{< youtube 6T97zIQ14d8 >}} 



On Windows 10, the default power settings are set to turn off the display automatically after several minutes of inactivity to minimize the power usage. Although it’s a useful feature, especially to laptops and tablets running on battery, it’s not a feature for everyone, since many users prefer to have the screen active all the time.
 
If you want to keep your screen from turning off, you can set the power options to “never” to prevent the display timing out using the Settings app, Control Panel, and Command Prompt.
 
In this guide, you’ll learn the easiest ways to prevent the computer screen from turning off on Windows 10.
 
- Set screen to never turn off using Settings
 - Set screen to never turn off using Control Panel
 - Set screen to never turn off using Command Prompt

 
## Set screen to never turn off using Settings
 
To prevent the screen from turning off automatically, use these steps:
 
- Open Settings on Windows 10.
 - Click on System.
 - Click on Power & Sleep.
 - Under the “Power & sleep” section, use the “On battery, turn off after” drop-down menu and select the Never option. (Option available on laptops only.)
 - Keep screen from turning off
 - Use the “When plugged in, turn off after” drop-down menu and select the Never option.

 
Once you complete the steps, the screen will no longer turn off automatically after some time of inactivity.
 
Open Settings on Windows 10.
 
Click on System.
 
Click on Power & Sleep.
 
Under the “Power & sleep” section, use the “On battery, turn off after” drop-down menu and select the Never option. (Option available on laptops only.)
 
Keep screen from turning off

 
Use the “When plugged in, turn off after” drop-down menu and select the Never option.
 
If you’re using a laptop, you may also want to set the Sleep settings to “Never,” since using the default configuration will turn off the display when the device enters into the sleep power mode.
 
## Set screen to never turn off using Control Panel
 
To keep the display from turning off with Control Panel, use these steps:
 
- Open Control Panel.
 - Click on Hardware and Sound.
 - Click on Power Options.
 - Click the Choose when to turn off the display option from the left navigation pane.
 - Choose when to turn off display option
 - Use the “Turn off the display” drop-down menu and select the Never option for the “On Battery” and “Plugged in” settings. (The “On Battery” option is only available on laptops.)
 - Screen timeout options in Control Panel
 - Click the Save changes button.

 
After you complete the steps, Windows 10 will never turn off the display again automatically to save power.
 
Open Control Panel.
 
Click on Hardware and Sound.
 
Click on Power Options.
 
Click the Choose when to turn off the display option from the left navigation pane.
 
Choose when to turn off display option

 
Use the “Turn off the display” drop-down menu and select the Never option for the “On Battery” and “Plugged in” settings. (The “On Battery” option is only available on laptops.)
 
Screen timeout options in Control Panel

 
Click the Save changes button.
 
## Set screen to never turn off using Command Prompt
 
To set the screen timeout to never with a command, use these steps:
 
- Open Start.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to set timeout setting to never and press Enter:
 - powercfg -change -monitor-timeout-ac 0
 - Command Prompt powercfg never turn off screen
 - (Optional) Type the following command to set screen timeout settings to never when running in battery and press Enter:
 - powercfg -change -monitor-timeout-dc 0

 
Once you complete the steps, the display timeout setting will be set to never turn off, even when you’re not actively using the device.
 
Open Start.
 
Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 
Type the following command to set timeout setting to never and press Enter:
 
powercfg -change -monitor-timeout-ac 0
 
Command Prompt powercfg never turn off screen

 
(Optional) Type the following command to set screen timeout settings to never when running in battery and press Enter:
 
powercfg -change -monitor-timeout-dc 0
 
The above commands run in Command Prompt as well as in PowerShell.
 
If you’re changing the screen timeout setting on a laptop, keep in mind that leaving the display all the time, even when you’re not actively using the device, it’ll drain the battery a lot faster.




