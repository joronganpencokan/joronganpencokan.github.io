---
title: "Unlock the Secret to Transform Your Ubuntu Interface with MDM Display Manager - Steps Inside!"
ShowToc: true 
date: "2022-11-10"
author: "Emma Wendler"
---
*****
# Unlock the Secret to Transform Your Ubuntu Interface with MDM Display Manager - Steps Inside!

As an Ubuntu user, you may have noticed that the default display manager can be somewhat bland and unexciting. However, fear not! The MDM display manager is a powerful tool that can completely transform your Ubuntu interface and give it a fresh, new look.

In this article, we will guide you through the simple steps required to install and configure MDM on Ubuntu.

## Step 1: Install MDM

The first step to unlocking the power of MDM is to install it on your Ubuntu operating system. To do this, open the terminal and enter the following command:

```
sudo apt-get install mdm
```

This will begin the download and installation process for MDM.

## Step 2: Configure MDM

Once MDM is installed, you can begin configuring it to your liking. To access the MDM configuration screen, enter the following command in the terminal:

```
sudo mdmsetup
```

This will open the MDM configuration window.

## Step 3: Choose Your Theme

One of the great things about MDM is the ability to customize the look of your login screen. This is done by choosing a theme from the available options in the MDM configuration window.

To access the available themes, click on the 'Themes' tab in the configuration window. From here, you can browse through the available options and choose the one that best fits your style.

## Step 4: Add Your Own Background

Another way to customize your MDM login screen is by adding your own background image. To do this, click on the 'Local' tab in the MDM configuration window. From here, you can browse to the location of your desired image and select it.

Once you have added your background image, you can see a preview of how it will look on the login screen by clicking on the 'Preview' button.

## Step 5: Save Your Changes

After you have made all of your desired changes, be sure to click on the 'Save' button in the MDM configuration window. This will save your configuration settings and apply them to your login screen.

## Conclusion

By following these simple steps, you can unlock the power of MDM and completely transform the look of your Ubuntu interface. With a wide range of themes and customization options available, the possibilities are endless. So what are you waiting for? Start customizing your display manager today!

{{< youtube JwudRbgLTNQ >}} 



If you have heard of Linux Mint, you will be pleased to know that the latest release (Linux Mint 14) comes with a new login manager – MDM Display Manager, that is both beautiful and customizable. Here is how you can get it on your Ubuntu.
 
The MDM Display Manager is based on the GDM 2.20. While it comes with its own set of themes, you can also install custom GDM theme from gnome-look.org and customize it to your liking. 
 
1. Open a terminal and type:
 
This will add the Linux Mint 14 repository to your repo list. 
 
Next, we are going to do a repo update:
 
You will see an error message like this:
 

 
Ignore it. Proceed to install the Linux mint keyring. This will get rid of the error above.
 
If you have previously installed GDM, you have to remove it as it conflicts with MDM:
 
Next, install MDM:
 
As it installs, it will show the following message:
 
Click “OK” to proceed.
 
Tap arrow-down to select MDM and click OK.
 
That’s it. Restart your computer and you should MDM as the default login manager in the next bootup.
 
## Customizing MDM
 
In the terminal, type:
 
This will open the Login Windows Preferences. Here is where you can configure many aspect of the login screen, including auto-login, remote access etc.
 
To change the theme, first go to “Gnome-look.org -> GDM themes” and download your favorite theme. It should be in .tar.gz format. 
 
Next, in the Login Windows Preferences, go to the “Local” tab.
 
Click the “Add” button and select the downloaded theme. The new theme should appear in the list. Select it and click “Close”. Log out of your current session and you should see the new theme in action.
 
If you find that the GDM theme that you have downloaded cannot be added, it is probably because it is not coded for the MDM. To fix this, you just have to go into the .tar.gz file and rename every instance of “GdmGreeterTheme” to “MdmGreeterTheme”.  Once that is done, you will be able to add it to the MDM theme directory.
 
To switch back to lightdm
 
and you should be able to choose lightdm as the default display manager. Restart the computer for it to take effect. 
 
That’s all. 
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




