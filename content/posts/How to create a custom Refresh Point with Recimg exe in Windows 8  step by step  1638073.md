---
title: "Revamp Your Windows 8 Experience With This Foolproof Guide to Creating A Custom Refresh Point!"
ShowToc: true 
date: "2023-02-01"
author: "Samantha Dodd"
---
*****
# Revamp Your Windows 8 Experience With This Foolproof Guide to Creating A Custom Refresh Point!

Are you tired of constantly dealing with sluggish performance and system crashes on your Windows 8 computer? If so, you’re not alone. Many users struggle with these same issues, but the good news is that there’s a simple solution that can help improve your computer’s performance and stability.

One of the most effective ways to optimize your Windows 8 experience is by creating a custom refresh point. A refresh point is essentially a snapshot of your computer’s settings and system files at a given moment in time. This allows you to easily restore your computer to a previous state if anything goes wrong, such as a virus or software malfunction. 

In this article, we’ll provide you with a step-by-step guide on how to create a custom refresh point in Windows 8. Follow these instructions and you’ll be well on your way to a faster, more reliable computing experience.

## Step 1: Open the System Properties Window

To get started, right-click on the start menu button and select ‘System’ from the menu. This will bring up the System Properties window.

## Step 2: Access the System Protection Settings

In the System Properties window, select the ‘System Protection’ tab. This will allow you to configure your computer’s restore settings.

## Step 3: Create a Custom Refresh Point

Once you’re in the System Protection tab, click on the ‘Create’ button to create a new restore point. You will be prompted to give it a name so you can easily recognize it later on.

## Step 4: Confirm Your Settings

After creating the refresh point, you’ll receive a confirmation message letting you know that the process was successful. Make sure to take note of the name you gave the point in order to easily access it later on.

## Step 5: Use Your Custom Refresh Point

After creating the refresh point, you can use it to restore your computer to its previous state at any time. Simply go back to the System Properties window, select the ‘System Protection’ tab, and click on ‘System Restore’. From there, you’ll be able to see all the available restore points and select the one you want to restore your computer to.

By creating a custom refresh point, you can safeguard your computer against system crashes, software malfunctions, and other issues that can cause it to slow down or stop working properly. Not only that, but you’ll save yourself valuable time and effort by being able to quickly restore your computer to a previous state if anything goes wrong.

So go ahead and give it a try! With this simple guide, you can revamp your Windows 8 experience and enjoy a faster, more reliable computing experience.

{{< youtube XEEcxYzNOfI >}} 



In Windows 8, Microsoft has introduced two really nifty system recovery tool features: “Refresh your PC without affecting your files” and “Remove everything and reinstall Windows”. This first feature helps you when your PC isn’t working well by reinstalling Windows, but without losing your data or your Windows 8 apps, and the second feature “Remove everything” is a really good options is you want to completely start from scratch (reset to factory) or recycle your PC without giving away your personal information.
 
Both features are great, the problem with these features are that desktop applications like iTunes, Chrome, Photoshop or websites are not kept. This translate and many unnecessary hours reinstalling and reconfiguring those applications you use everyday.
 
To mitigate this issue, Windows 8 includes a new command utility called Recimg.exe, that will help you to create a custom Windows 8 Refresh Point (or recovery image) which may include special Windows settings, desktop applications and more. Even though this is done through a command line utility, it is not something difficult to do, using Recimg you’ll only need to point to a target location to save the Windows Installer Image (WIN) image format and configure custom Refresh your PC image a default & active.
 
## Steps to create a custom Refresh Point in Windows 8
 
1. In the Start Screen type cmd, right-click and select Run as administrator.
 
2. In Windows Command Prompt type the following and press Enter:
 

 
The “C:\Custom_Image_Refresh” in the command is just the path to where I want to store the recovery image — you can add your own location and folder name –, and as you might have guessed the /createimage is a switch from recimg that is use to create a custom Windows 8 Refresh image. It’s also important to note that the /createimage switch will also set this new custom recovery image as the new default & active. You can always keep more than one Refresh Point image, but if you want to use one of them, you’ll need to manually set it as default & active.
 
To configure a custom Refresh Point as default & active you have to open the Command Prompt as administrator and type the following:
 
Remember to replace the “C:\Custom_Image_Refresh” with the path to where you have saved the custom image. If for any reason Windows doesn’t find the custom recovery image in the specified location, Windows will fall back to the default image (or installation media) when you refresh your PC.
 
What you’ve done so far is to create and configure a default custom Refresh your PC image. Now when it comes the time and you need to refresh your PC:
 
1. Move the mouse pointer to the top-right or bottom-right of the screen and from the Charms, click or tap Settings and then click on Change PC settings.
 
2. From PC settings, click on General and on Refresh your PC without affecting your files, click on Get started.
 
3. Finally, click Next, Refresh and wait for Windows 8 to finish.
 
The good thing about this process is that you can always go back and use Microsoft’s Windows 8 default to Refresh your PC image, you can do this by using the Recimg.exe utility with the /deregister switch. And to check which custom image is current you can use the /showcurrent switch.




