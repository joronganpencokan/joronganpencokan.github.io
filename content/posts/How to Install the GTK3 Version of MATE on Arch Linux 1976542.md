---
title: "Revamp Your Linux Experience: Unlock the Power of MATE with GTK3 on Arch Linux - Here's How!"
ShowToc: true 
date: "2023-01-22"
author: "Sherry Simmons"
---
*****
Revamp Your Linux Experience: Unlock the Power of MATE with GTK3 on Arch Linux - Here's How!

If you are a Linux user, you know how important it is to have a desktop environment that is fast, intuitive, and customizable. And if you are looking for a desktop environment that ticks all these boxes, then MATE is the perfect choice for you. MATE is a lightweight, open-source desktop environment that is based on the traditional GNOME 2 desktop. And if you want to unlock even more power and customization options, you can use the GTK3 version of MATE on Arch Linux. In this article, we will guide you through the process of installing and using MATE with GTK3 on Arch Linux, so get ready to revamp your Linux experience.

Step 1: Install Arch Linux

If you are new to Arch Linux, you can check out our previous article on how to install Arch Linux. Arch Linux is a rolling release GNU/Linux distribution that is known for its minimalist design and flexibility. When you install Arch Linux, you will have complete control over your system, and you can easily install and configure the software that you need.

Step 2: Install MATE with GTK3

MATE with GTK3 is not available on the official Arch Linux repositories, but you can install it from the AUR (Arch User Repository). To do so, you need to install a package manager for the AUR, such as yay or trizen. Once you have installed a package manager, you can use it to install MATE with GTK3.

To install MATE with GTK3 using yay, open the terminal and run the following command:

```
yay -S mate-gtk3
```

To install MATE with GTK3 using trizen, open the terminal and run the following command:

```
trizen -S mate-gtk3
```

The installation process may take some time, so be patient.

Step 3: Configure MATE with GTK3

Once you have installed MATE with GTK3, you can start configuring it. To do so, open the MATE Control Center by clicking on the "System" menu and selecting "Control Center." In the Control Center, you can configure various MATE settings, such as the appearance, the desktop background, the panels, the startup applications, and more.

If you want to change the GTK3 theme, you need to install the GTK3 themes that you like. You can find many GTK3 themes on websites such as GNOME-Look.org or DeviantArt. Once you have downloaded the GTK3 theme that you like, you can install it by extracting the archive to the /usr/share/themes directory.

Step 4: Enjoy MATE with GTK3

Congratulations, you have now successfully installed MATE with GTK3 on Arch Linux and configured it to your liking! Now you can enjoy the lightweight, intuitive, and customizable desktop environment that MATE offers. With MATE and GTK3, you can personalize your Linux experience to suit your workflow and preferences.

In conclusion, MATE with GTK3 is a powerful and flexible desktop environment that is ideal for Linux users who want a fast and customizable experience. And with Arch Linux, you have the freedom to customize your system even further. We hope this article has helped you to install and configure MATE with GTK3 on Arch Linux, and we wish you happy computing!

{{< youtube jncc3QL8RWI >}} 



If I were to describe one of the current Linux trends as of late, it would be lightweight desktops. A lot of interest has been generated around projects that create a desktop Linux experience that has the ability to run lighter on your machine.
 
Perhaps the most notable is the Mate project. If you don’t know about it, here’s a quick overview. Mate is the spiritual successor to the extremely popular Gnome 2.x. They’ve taken the source code from that old project and converted it into something a lot more modern.
 
The Mate desktop is pretty great. It’s light, efficient and people don’t have a hard time figuring it out. There is one problem though. The software it’s built on is getting pretty dated and isn’t as good as it could be. How do we solve this issue? Simple! Upgrade Mate to GTK3.
 
Note: upgrading Mate from GTK2 to GTK3 is unstable. Do this at your own risk.
 
## Upgrading Mate from GTK2 to GTK3
 
To upgrade your Mate install, you’ll need to add a repository to your pacman configuration file. You can easily do this by editing this file (as root) in your text editor of choice. Open up a terminal window and enter the following.
 

 
Once you’ve opened your “pacman.conf” file, paste the code below into it.
 
When the repository has been added to “pacman.conf”, save it (Ctrl + o) and exit nano (Ctrl + x). After that you’ll need to update pacman to reflect the changes you’ve made. Enter the following into the terminal window.
 
Now that pacman is updated and sees the new repository, you can finally update Mate from GTK2 to GTK3.
 
When the command above is entered, pacman will prompt you to replace a whole lot of Mate GTK2 components with GTK3 ones. Say yes to all of them.
 
When all of the components are replaced, you’ll have the GTK3 version of the Mate desktop instead of the GTK2 version.
 
## Revert Mate back to GTK2
 
Reverting from GTK3 back to 2 is fairly easy. Just enter this command into a terminal to remove it completely.
 
Once this command has finished, you’ll have removed the GTK3 version of Mate.
 
If you want, you can also go back into your “pacman.conf” file and remove the repository. Doing this is considered optional as both versions of Mate are marked as different packages.
 
Note: you may need to re-install the GTK2 version of Mate after removing the updated one.
 
## Conclusion
 
Mate is an awesome piece of software if what you are looking for is a lightweight experience. It’s great. It has everything that you could ever ask for when it comes to a functional desktop. The only real issue is that GTK2 is starting to show its age. This is why I’m really glad there’s a version running with something a bit more modern.
 
What version of Mate do you prefer? Tell us what you think in the comment section below!
 
Derrik Diener is a freelance technology blogger.
 
Our latest tutorials delivered straight to your inbox




