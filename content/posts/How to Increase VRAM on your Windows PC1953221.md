---
title: "You Won't Believe the Insane Results When You Increase Your Vram on Windows PC!"
ShowToc: true 
date: "2023-04-21"
author: "Marc Pickett"
---
*****
# You Won't Believe the Insane Results When You Increase Your VRAM on Windows PC!

Are you struggling with slow gaming performance on your Windows PC? Are you tired of low frame rates and choppy graphics? You may be surprised to learn that the solution to your problems can be as simple as increasing your VRAM.

VRAM, or video random access memory, is a type of memory that is dedicated to graphics processing. The more VRAM your computer has, the better it can handle advanced graphics and processes. And when it comes to gaming, having adequate VRAM is essential for smooth and seamless gameplay.

So, what happens when you increase your VRAM? The answer is simple - your computer's graphics capabilities increase. With more VRAM, your computer can handle advanced graphics processing without compromising performance. You'll see a noticeable difference in your gaming experience, with smoother framerates, better textures, and more detailed graphics.

But how can you increase your VRAM on a Windows PC? The process may vary depending on your computer's specifications, but the general steps are as follows:

Step 1: Check Your Current VRAM
The first step is to check how much VRAM your computer currently has. To do this, right-click on your desktop and select "Display settings." From there, click on "Advanced display settings" and then "Display adapter properties." This will open a window that displays your computer's graphics card and VRAM.

Step 2: Change VRAM Settings
Once you know how much VRAM your computer has, you can adjust the settings to increase it. This process will vary depending on your graphics card and computer specifications. You can usually adjust VRAM settings in your computer's BIOS or through a graphics card control panel.

Step 3. Save and Restart
Once you've adjusted your VRAM settings, make sure to save your changes and restart your computer to ensure the new settings take effect.

It's important to note that not all computers can have their VRAM increased. Some laptops and older computers have integrated graphics cards that have set VRAM that cannot be changed.

In conclusion, increasing your VRAM on a Windows PC can have a significant impact on your gaming experience. With smoother framerates, better graphics, and more detailed textures, you'll be able to fully immerse yourself in your favorite games. So why not give it a try and see the insane results for yourself?

{{< youtube e_XcyANK5zk >}} 




This article explains how to increase VRAM using BIOS/UEFI and the Windows registry on Windows 7, 8, and 10, and how to check how much you have.

 
### 
What to Know
 
- When in the BIOS/UEFI look for an option that allows you to change VGA Share Memory Size or VRAM Size.Or press Windows key+R >type regedit > Enter and follow the instructions below.

 
##   Increase VRAM Using the BIOS/UEFI  
 

Some Windows PCs and laptops will let you assign more system memory to the onboard GPU in the BIOS/UEFI. To do so, access the BIOS or UEFI as explained in this guide. Each BIOS and UEFI is a little different, depending on the manufacturer and BIOS/UEFI version, so you may need to refer to the manual to find out any specifics for access keys and layout.

 

When in the BIOS/UEFI, search for menus labeled Advanced Features or Advanced Chipset Features. If you can find them, you want to look within them for Graphics Settings, Video Settings, and similar. Ultimately you're trying to find an option that allows you to change VGA Share Memory Size or VRAM Size.

 

If these options exist within your system's particular BIOS/UEFI, then you'll be able to change between 128MB, 256MB, 512MB, or maybe even 1024MB. If you have 2GB of system memory, select 256GB; if you have 4GB, select 512MB, and if you have 8GB, select 1024MB.

 
##   Increase VRAM Using the Registry  
 

Another method to increase VRAM in your PC is through the system registry. This is a little more complicated and if you don't know what you're doing you can damage your Windows installation, so be careful and read up on how to access and use the Windows registry before trying it.

 

Consider making a Windows system restore point too.

 
- Press the Windows key+R and type regedit. Then press Enter.
 - If you're using Intel onboard graphics, navigate to HKEY_LOCAL_MACHINE\Software\Intel.
 - If you're using an AMD APU, change the last menu option in that chain to AMD.
 - Right-click (or tap and hold) on the Intel or AMD folder and select New > Key. Name it GMM.
 - Select the new GMM folder and right-click (or tap and hold) in the right Windows pane. Select New > DWORD (32-bit) Value.
 - Name it DedicatedSegmentSize and give it a (Decimal) value equalling the amount of VRAM you want your GPU to have access to. If you have 4GB of system memory, 512MB would be a good value to opt for. If you have 8GB, 1024 would be a good choice.
 - Restart your system and then follow the steps below to see how much VRAM you have. If it reports the higher value, you may have improved your system's performance and made it possible to play games with minimum limits on VRAM usage.

 
##   Check How Much VRAM You Have  
 

Dedicated Video RAM, or VRAM, the colloquial term for the amount of memory (RAM) your system's graphics processing unit (GPU) has access to, can be a major factor in your Windows PC's gaming and 3D rendering performance. Without enough of it, assets have to be pulled from the far slower system storage.

 

Press the Windows key+R and type regedit. Then press Enter.

 

If you're using Intel onboard graphics, navigate to HKEY_LOCAL_MACHINE\Software\Intel.

 

If you're using an AMD APU, change the last menu option in that chain to AMD. 

 

Right-click (or tap and hold) on the Intel or AMD folder and select New > Key. Name it GMM.

 

Select the new GMM folder and right-click (or tap and hold) in the right Windows pane. Select New > DWORD (32-bit) Value.

 

Name it DedicatedSegmentSize and give it a (Decimal) value equalling the amount of VRAM you want your GPU to have access to. If you have 4GB of system memory, 512MB would be a good value to opt for. If you have 8GB, 1024 would be a good choice.

 

Restart your system and then follow the steps below to see how much VRAM you have. If it reports the higher value, you may have improved your system's performance and made it possible to play games with minimum limits on VRAM usage.

 

Before you attempt to increase VRAM in your Windows PC, you need to know how much you have already.

 
- Open the Windows Settings menu by pressing Windows key+I.
 - If using Windows 7 or 8, right-click (or tap and hold) on the desktop and select Screen Resolution, then skip to step 3.
 - Select System, followed by Display in the left-hand menu.
 - Scroll down until you see Advanced display settings. Select it.
 - If you have more than one display in use, make sure the main one connected to your GPU is selected in the top drop-down menu. Then select Display adapter properties.
 - The figure next to Dedicated Video Memory is how much VRAM your GPU currently has available.

 

If you're not sure whether you're using a dedicated graphics card or an onboard GPU solution, then this screen will tell you, too. If your Chip Type is listed as an AMD Radeon Graphics Processor or an Nvidia GTX device, you are using a dedicated graphics card. If it says Intel HD Graphics or AMD Accelerated Processing Unit, then you're using onboard graphics and may be able to increase your VRAM.

 
If you're using a dedicated graphics card, the only way to improve the amount of VRAM you have available is to buy a better graphics card with more of it.
 

Open the Windows Settings menu by pressing Windows key+I.

 
If using Windows 7 or 8, right-click (or tap and hold) on the desktop and select Screen Resolution, then skip to step 3.
 

Select System, followed by Display in the left-hand menu.

 

Scroll down until you see Advanced display settings. Select it.

 

If you have more than one display in use, make sure the main one connected to your GPU is selected in the top drop-down menu. Then select Display adapter properties.

 

The figure next to Dedicated Video Memory is how much VRAM your GPU currently has available.

 

Get the Latest Tech News Delivered Every Day




