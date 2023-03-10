---
title: "Unlock The Full Potential Of Your Netbook - Boost Your Screen Resolution With These Genius Hacks!"
ShowToc: true 
date: "2022-11-29"
author: "Britany Nichols"
---
*****
Unlock The Full Potential Of Your Netbook - Boost Your Screen Resolution With These Genius Hacks!

Netbooks are compact, lightweight, and portable devices that have been around for over a decade. They are designed for simple web browsing, email, editing documents, and basic multimedia playback. However, if you crave more from your netbook, then boosting the screen resolution is a great way to unlock its full potential. With a higher resolution, you'll have more screen real estate to multitask, watch videos, and play games. In this article, we'll explore some genius hacks to boost your netbook screen resolution and enhance your productivity and entertainment experience.

What is screen resolution?

Before we delve into the hacks, let's first understand what screen resolution is. In simple terms, screen resolution refers to the number of pixels that make up the display of your device. It is measured as the number of pixels horizontally and vertically, such as 1366x768 or 1920x1080. The higher the number of pixels, the more detailed and sharper the images and text on your screen will be. Additionally, a higher resolution allows you to fit more content on your screen at once and reduces the need for scrolling.

Hack #1: Update your drivers and settings

The first step to boost your netbook's screen resolution is to ensure that you have the latest graphics drivers installed. Graphics drivers are software that enables your computer to communicate with your netbook's graphics card. Outdated or incorrect drivers can cause issues with your display and limit your resolution options. To update your drivers, visit your computer's manufacturer's website or use third-party software like Driver Booster or Snappy Driver Installer.

Once you have updated your drivers, head over to your display settings and check if you can increase the resolution. In Windows 10, go to Settings > System > Display and select the resolution from the drop-down menu. If your desired resolution is not available, move on to Hack #2.

Hack #2: Use the registry editor trick

If your netbook's manufacturer has limited your resolution options in the display settings, you can use a registry editor hack. However, I must warn you that modifying your registry can be risky and may cause instability or crashes if done incorrectly. Hence, I suggest backing up your registry or creating a system restore point before proceeding.

The registry editor trick involves adding a custom resolution to your netbook's registry that is not available in the display settings. To do this, follow these steps:

1. Press Win + R on your keyboard to open the Run dialog box.

2. Type "regedit" and press Enter to open the Registry Editor.

3. Navigate to HKEY_CURRENT_CONFIG\System\CurrentControlSet\Control\VIDEO\\*\0000, where the asterisk represents a string of alphanumeric characters that varies between systems.

4. Right-click on an empty space in the right pane and select New > String Value.

5. Rename the new string value "DALR6 DFP 0" (without the quotes), which represents your netbook's graphics card.

6. Double-click on the new string value and enter the following values:

Value data: 20 00 00 00 (hexadecimal)

Base: Hexadecimal

7. Close the registry editor and restart your netbook.

8. Once restarted, go back to the display settings, and you should see the new custom resolution available. Select it, and voila, you've boosted your netbook's screen resolution!

Note that not all graphics cards support custom resolutions and may cause issues like black screens, so make sure to research your netbook's graphics card before attempting the hack.

Hack #3: Use third-party software

If the previous hacks didn't work for you or seemed too risky, you can always use third-party software to boost your netbook's screen resolution. There are many software options available, such as PowerStrip, CRU (Custom Resolution Utility), and SwitchResX. These applications allow you to create custom resolutions, adjust refresh rates, and tweak other display settings to make the most of your netbook's screen. Additionally, some software like SwitchResX can automate the resolution switching process for different applications, ensuring that you always have the best resolution for your needs.

In conclusion, boosting your netbook's screen resolution can enhance your productivity and entertainment experience. Whether you're using custom resolutions, registry hacks, or third-party software, make sure to research your netbook's graphics card and backup your system before proceeding. With these hacks, you'll unlock the full potential of your netbook and enjoy a more enjoyable and efficient computing experience.

{{< youtube jzY-N7V__fU >}} 




Many netbooks and less-expensive laptops ship with a default 1024-pixel-by-600-pixel (or similar) small-screen resolution, which causes problems in some apps or requires a lot of scrolling. To increase the amount of screen real estate on your Netbook or use apps that require higher-resolution displays, make a registry change to get options for higher resolutions.

 
##   How to Make the Registry Change  
 

You may have heard warnings about the risks of altering the registry, and these are valid—you don't want to play around in the registry without knowing what you're doing. However, this registry change is not complex.

 
If your netbook's natural resolution is 1024x600, increasing it above this by using this registry tweak results in a lower-quality appearance—but apps that require a higher resolution will display.
 

First, try changing the screen resolution in Windows through the Control Panel to see if higher resolutions are available. If not, make these registry changes to make a higher resolution option available.

 
This registry tweak may conflict with some graphics cards and may generate a Blue Screen of Death error. Make a backup of the registry in case something goes wrong. If it does, restore the registry file to undo the changes.
 

To change the registry:

 
- Open the registry editor with the regedit command, either from the Run dialog box, Start menu, or Command Prompt.
 - Scroll to the top of the left pane to go to the top of the registry tree.
 - Go to Edit and select Find. In the search field, enter Display1_DownScalingSupported and select Find Next. The search may take a while to complete.
 - If this registry key is missing, see the next section below for instructions on how to add it.
 - In the right pane, select Display1_DownScalingSupported.
 - Go to Edit and select Modify (or double-click the key name) and in the Value data field change the 0 to a 1.
 - Change the value for every instance of the key found in the search; otherwise, the hack may not work.
 - When you're done, restart the computer.

 

When your PC restarts, and you go to change the resolution, you'll see options for 1024x768 and 1152x864 resolutions for your device, in addition to any previous resolutions.

 

Open the registry editor with the regedit command, either from the Run dialog box, Start menu, or Command Prompt.

 

Scroll to the top of the left pane to go to the top of the registry tree.

 

Go to Edit and select Find. In the search field, enter Display1_DownScalingSupported and select Find Next. The search may take a while to complete.

 
If this registry key is missing, see the next section below for instructions on how to add it.
 

In the right pane, select Display1_DownScalingSupported.

 

Go to Edit and select Modify (or double-click the key name) and in the Value data field change the 0 to a 1. 

 
Change the value for every instance of the key found in the search; otherwise, the hack may not work.
 

When you're done, restart the computer.

 
##   If the Registry Key Is Missing  
 

If you didn't find this registry key, add it yourself. To add a registry key, make a new Display1_DownScalingSupported DWORD value in each registry key location.

 
Changing the default screen resolution on your low-end device may make it look stretched out. To fix this distortion, go to the advanced display properties for the Intel Graphics Media Accelerator (if your device uses Intel GMA) and set the aspect ratio to maintain aspect ratio.
 
- For the first key, go to:
 - HKEY_LOCAL_MACHINE > SYSTEM > CurrentControlSet > Control > Class > {4D36E968-E325-11CE-BFC1-08002BE10318} > 0000
 - On a Lenovo S10-3T, the key is found in one of these two places:
 - HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Control\Video\(154229D9-2695-4849-A329-88A1A7C4860A\0000
 - OR
 - HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Video\(154229D9-2695-4849-A329-88A1A7C4860A)\0000
 - Go to Edit and select New > DWORD (32-bit) Value.
 - In the right pane, change the name of New Value #1 to Display1_DownScalingSupported and press Enter.
 - Select Display1_DownScalingSupported, and press Enter. In the window that opens, set Value data to 1.
 - Repeat the previous steps for each of the following locations if they exist (not all of these may be present), and change all values to 1.
 - HKEY_LOCAL_MACHINE\SYSTEM\Current Control Set\Control\Class\{4D36E968-E325-11CE-BFC1-08002BE10318}\0001
 - HKEY_LOCAL_MACHINE\SYSTEM\Current Control Set\Control\Class\{4D36E968-E325-11CE-BFC1-08002BE10318}\0002
 - Restart the computer.
 - Go to Display settings and, under Resolution, change the setting to a higher resolution.

 

For the first key, go to:

 

HKEY_LOCAL_MACHINE > SYSTEM > CurrentControlSet > Control > Class > {4D36E968-E325-11CE-BFC1-08002BE10318} > 0000

 

On a Lenovo S10-3T, the key is found in one of these two places:

 

HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Control\Video\(154229D9-2695-4849-A329-88A1A7C4860A\0000

 

OR

 

HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Video\(154229D9-2695-4849-A329-88A1A7C4860A)\0000

 

Go to Edit and select New > DWORD (32-bit) Value.

 

In the right pane, change the name of New Value #1 to Display1_DownScalingSupported and press Enter.

 

Select Display1_DownScalingSupported, and press Enter. In the window that opens, set Value data to 1.

 

Repeat the previous steps for each of the following locations if they exist (not all of these may be present), and change all values to 1.

 

HKEY_LOCAL_MACHINE\SYSTEM\Current Control Set\Control\Class\{4D36E968-E325-11CE-BFC1-08002BE10318}\0001

 

HKEY_LOCAL_MACHINE\SYSTEM\Current Control Set\Control\Class\{4D36E968-E325-11CE-BFC1-08002BE10318}\0002

 

Restart the computer.

 

Go to Display settings and, under Resolution, change the setting to a higher resolution.

 

Get the Latest Tech News Delivered Every Day




