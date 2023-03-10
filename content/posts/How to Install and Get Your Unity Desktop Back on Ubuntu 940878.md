---
title: "Say Goodbye to Boring Ubuntu: Learn How to Bring Back Your Fave Unity Desktop in Minutes!"
ShowToc: true 
date: "2023-01-17"
author: "Faustino Swanger"
---
*****
Say Goodbye to Boring Ubuntu: Learn How to Bring Back Your Fave Unity Desktop in Minutes!

Ubuntu has been the go-to operating system for developers and enthusiasts alike for years. It's the perfect blend of reliability and flexibility that makes it an excellent choice for work as well as personal use. However, the recent change in Ubuntu's interface design may have left some users disappointed.

The company has shifted its focus from Unity, the desktop environment that was once the default interface of Ubuntu, to a new design called GNOME. While GNOME is an impressive interface in its own right, there are still some users who prefer the familiar look and feel of Unity.

If you're one of those users, don't despair. You can still bring back the Unity desktop with just a few simple steps. In this article, we'll go over how to install Unity and switch back to it in Ubuntu in minutes!

Before we begin, there are a few requirements that you'll need to meet. You'll need to be running Ubuntu 18.04 or later versions on your computer. It's also essential to have an internet connection so that you can download the necessary files.

Step 1: Install Unity

The first step is to install the Unity desktop environment. To do this, open up the terminal by pressing Ctrl+Alt+T or by searching for “Terminal” in the Dash.

Now, run the following commands:

```
$ sudo apt-get update
$ sudo apt-get install unity-session
```

This command will download and install the necessary files for the Unity desktop environment.

Step 2: Logout

Once the installation is complete, log out of your current session. You can do this by clicking on the “Log Out” button in the top-right corner of the screen or by pressing Ctrl+Alt+Del.

Step 3: Choose Unity

After logging out, you'll find yourself on the login screen. In the top-right corner of the screen, you'll see a small gear icon. Click on it to open a drop-down menu and choose the “Unity” option.

Step 4: Login

Now, enter your password and log in as usual. You should now see the Unity desktop environment.

Conclusion

In conclusion, bringing back the Unity desktop environment to your Ubuntu installation is straightforward and can be done in just a few minutes. Once you have installed Unity and switched back to it, you'll be able to enjoy the familiar interface that you've grown to love.

Whether you're a developer or a casual user, the Unity desktop environment offers a perfect blend of functionality and ease-of-use that's hard to beat. So why wait? Go ahead and say goodbye to the boring GNOME interface and bring back your favorite Unity desktop today!

{{< youtube zLX3vJgLdrw >}} 



If you ever installed Ubuntu between versions 10 and 16, you surely had contact with the Unity desktop. As it was very different from other graphical shells, some have hated it. Others loved it, including some macOS fans possibly too, as the interface was somewhat similar to Apple’s operating system in some areas.
 
But, alas, Ubuntu 18.04 removed Unity and replaced it with the Gnome shell. Since it introduces even more alien concepts to the desktop experience, people started to migrate to LXDE, XFCE, KDE, MATE and other environments/shells.
 
But maybe you’re nostalgic and want Unity back. Or, maybe you’re actually one of the people that loved it for its way of doing things and feel more productive in it. These things are of course subjective. However, an objective fact is that Unity is much more fluid, faster, and responsive when compared to Gnome. Whatever your motivation may be, it’s easy to install Unity and make it the default graphical shell again.
 

 
## From “main” to “universe”
 
All of Unity’s components were moved from “main” to the “universe” software repositories. Canonical actively maintains whatever resides in “main.” In contrast, the community maintains stuff in “universe,” meaning that volunteers update and/or improve software there – that is, if someone gets around to it and has the time and motivation to do so. This means there’s no guarantee the software will work in future generations of Ubuntu. Usually though, software packages that are popular, like this one, do get to live on either in the same form, or as some fork, under a different name, adapted to function on new versions of the operating system.
 
So, consider this tutorial as “tested to work on Ubuntu 18.04,” and if you encounter problems on future editions, try to research if anything has changed. The first thing you should look for is whether the package name “ubuntu-unity-destkop” is the same on Ubuntu 20.04, 20.10, 22.04 and beyond.
 
Make sure you have the “universe” repository enabled. It’s active, by default, on most installations. In that case the command will just report this and do nothing else. If it isn’t, it will enable it.
 
## Install Unity Graphical Shell and Dependencies
 
Install packages and dependencies:
 
You will get some prompts to choose the default login manager. First, you will get some generic text that explains what the choice is about, and you will only get an “OK” button to select. At the next screen, press the down arrow, select “lightdm” and press Enter.
 
## Change Default Graphical Shell in Login Manager
 
Reboot your computer to reload the entire graphical stack.
 
When you get to the login screen, click on the button highlighted in red in the next image.
 
You should then see what desktop environment/graphical shell will launch when the user logs in. Unity should already be the default at this point. If it isn’t it, pick it from that list. If it is, just click the back button (highlighted in red) and then log in normally.
 
## Conclusion
 
That was easy, wasn’t it? And just in case you don’t like how Gnome “simplified” some programs by removing features you possibly liked, remember that you can install other programs and make your desktop even more pleasant. For example, maybe you don’t like the default file manager, Nautilus, because it looks so bare. With a simple sudo apt install caja, you can install the Caja file manager, or whatever else you prefer. Have fun making your desktop your own!
 
Fell in love with computers when he was four years old. 27 years later, the passion is still burning, fueling constant learning. Spends most of his time in terminal windows and SSH sessions, managing Linux desktops and servers.
 
Our latest tutorials delivered straight to your inbox




