---
title: "Transform Your Gnome Shell Interface into a Stunning Unity Look with These Easy Tips!"
ShowToc: true 
date: "2023-05-24"
author: "Ana Dickson"
---
*****
Transform Your Gnome Shell Interface into a Stunning Unity Look with These Easy Tips!

If you are a Linux user, you would know that Gnome Shell is one of the most popular desktop environments. It is customizable and can be tailored to fit your personal preferences. However, if you have used Unity before, you might miss its user-friendly interface, which is why you might want to transform your Gnome Shell interface into a stunning Unity look.

In this article, we will share some easy tips that will help you achieve the desired look in no time.

Install the Unity Shell Theme

The first step towards achieving a Unity look is to install the Unity Shell theme. You can download it from the Gnome-look website or by using the following command in your terminal:

$ sudo apt-get install unity-tweak-tool

Once installed, open the Unity Tweak Tool, go to Appearance and select the Unity theme. This will change the overall look of your desktop to resemble that of the Unity interface.

Install the Unity Dash

Another important aspect of the Unity interface is its Dash, which is a search bar that enables you to quickly search for apps and files. To install the Unity Dash in your Gnome Shell interface, you need to download and install the Gnome-Shell-Extensions-Dash-to-Dock extension.

You can install it by using the following command:

$ sudo apt-get install gnome-shell-extension-dash-to-dock

Once installed, open the Gnome Tweak Tool, go to Extensions and enable the Dash to Dock extension. This will add a Dash to your desktop that resembles the Unity interface.

Install the Unity App Menu

Lastly, to complete the Unity look, you need to add the Unity App Menu. This menu is similar to the one found in Ubuntu's Unity interface and provides a centralized location to access your apps.

To install the Unity App Menu, you need to install the Gnome-Shell-Extensions-Applications-Menu extension. You can install it by using the following command:

$ sudo apt-get install gnome-shell-extension-applications-menu

Once installed, open the Gnome Tweak Tool, go to Extensions and enable the Applications Menu extension. This will add the Unity App Menu to your desktop.

Conclusion

In conclusion, transforming your Gnome Shell interface into a stunning Unity look is easy and can be done in a few simple steps. By installing the Unity Shell theme, the Dash to Dock extension, and the Applications Menu extension, you can achieve a unified interface that resembles the Unity desktop environment. So, go ahead and try these tips to experience the best of both worlds!

{{< youtube lrTaAokzH20 >}} 



Canonical, Ubuntu’s parent company, is dumping the Unity interface for upcoming releases in favor of the GNOME desktop environment. This has the Ubuntu community divided, to say the least. Some people really like Unity and don’t want to see it go. Others would prefer GNOME and have probably been waiting for it to come back as the default. If you fall into the first group, don’t worry. There ware ways to make GNOME, and other desktop environments, look and feel like Unity.
 
Before you go any further, you might want to consider KDE. Yes, this article is about Unity and GNOME, but KDE can be customized very easily, and you can make it look like Unity without a whole lot of effort of extras. That said, if you plan on downloading the default Ubuntu releases, you’re stuck with GNOME, so keep on reading.
 
## Download the Packages
 
There are some packages that you’re going to need to pick up from the Ubuntu repositories before you start customizing GNOME. Install them all with apt now so you can focus on putting everything together later on.
 
Once they’re done, you’re ready to start rearranging GNOME to look like Unity.
 
## Bring Unity’s HUD to Gnome with Plotinus
 
Plotinus provides what it calls a “searchable command palate” for GTK3 applications. The functionality actually behaves a lot like Unity’s HUD. Since GNOME is based on GTK3, Plotinus will bring Unity-like behavior to most of your applications.
 
Unfortunately, Plotinus isn’t available in Ubuntu’s repositories, but it’s really easy to build from its source.
 
Open a terminal. You’ll clone Plotinus from its Git repository and build it.
 
Now, change into that directory and create a build directory. Change into that directory, too, and build Plotinus.
 
It won’t take long at all to compile. When it’s done, use sudo to install it.
 
There’s one last step. You need to tell GNOME where to find the Plotinus library that you built. There is a file called “/etc/environment,” and you need to add the following line in there. You’ll need sudo to write the file.
 
Make sure to replace “username” with your actual username.
 

 
In order for the changes to take effect, you need to restart your computer or GDM. You can do either now or after everything is finished.
 
## Install the GNOME Extensions
 
Most of the visual changes that you can make to GNOME come from extensions. All of these extensions are super easy to install and use. Actually, you can install them all from your web browser.
 
Head to the GNOME extension website. At the top of the page you’ll see a big blue box. There will be a link in that box asking you to install the browser extension. Click it and follow the instructions to install it. That extension allows you to use your browser and the extensions site to manage your GNOME extensions.
 
To install every one of these extensions, flip the switch on the right side of the extension’s web page.
 
### Dash to Dock
 
The first extension that you’re going to need is Dash to Dock. It takes the “favorites” tab from the GNOME dash and turns it into a permanent dock on your desktop.
 
Once you have the extension installed, you’ll immediately notice the dock on your desktop. It’s a good start, but it isn’t perfect. Right-click on the application launcher button to open the Dash to Dock Settings.
 
The first tab handles positioning and size. You’ll want to set the dock on the main monitor to the left side of the screen. Turn off “intelligent autohide.”
 
At the bottom check both boxes to extend the dock to the full height of the screen and stop the icons from shrinking. Use the slider to set the icon size between 32 and 48. Adjust it to what looks best for you on your screen.
 
Move on to the “Launchers” tab. Flip all three switches to “On.” The other most important item to check is the box that moves the applications button to the top. Check that.
 
Finally, head to the “Appearance” tab. You need to flip the switches that shrink the dash and enable window counter indicators. Those two emulate Unity’s behavior. The rest are a matter of preference.
 
### Hide Activities
 
This next extension is very simple. It removes the “Activities” button in the top-left of the screen. It isn’t there in Unity, so you don’t want it here either.
 
### Better Volume
 
The Better Volume extension doesn’t change the way GNOME looks, but it does make the volume controls function more like Unity by enabling mouse scroll controls.
 
### Hot Corners
 
Hot Corners is that annoying “feature” that causes the GNOME dashboard to open when your mouse moves too far into the top corners. This extension removes that for the top left.
 
### Move the Clock
 
Unity’s clock is in the top-right corner of the screen. Flippery Move Clock moves GNOME’s clock to the same position.
 
### Impatience
 
Impatience usually isn’t a good thing, but here it speeds up GNOME’s default animations which can be pretty annoying and take too long. Shorter animations also match Unity’s behavior much more closely.
 
## Gnome Tweak Tool
 
The last bit of customization comes from the GNOME Tweak Tool. It comes installed with Ubuntu GNOME by default, so you’ll only need to open it.
 
In the “Appearance” tab you have three options that will help make GNOME look much more like Unity. First, set the “GTK” theme to “Adwaita-dark.” Set the “Icons” to “Humanity.” Lastly, set your “Cursor” to “DMZ-white.”
 
You might be able to find another theme that better emulates the default Unity look. There was one called Ambiance GNOME, but as of now, it doesn’t appear to support the latest GNOME releases.
 
## Wallpaper
 
If you want the default Ubuntu wallpaper, you can set that now, too. Right-click on your desktop. Select “Change Background…” then click on “Background” and find the default Ubuntu background.
 
## The Future
 
By now, your GNOME desktop looks and works a lot like Unity. It’s not exact, but it should be a much easier adjustment for Unity fans. You should remember, though, that unless someone else takes up the Unity mantle, it will disappear. Those add-ons are all developed by volunteers, so they, too, may eventually fall behind. You may want to begin getting accustomed to the default GNOME desktop or explore any of the other excellent options out there for Linux.
 
Nick is a freelance tech. journalist, Linux enthusiast, and a long time PC gamer.
 
Our latest tutorials delivered straight to your inbox




