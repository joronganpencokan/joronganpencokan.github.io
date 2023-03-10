---
title: "Revolutionize Your Design Game: Unlock the Secret to Making Gimp Work Like Photoshop in Linux!"
ShowToc: true 
date: "2022-12-19"
author: "James Bilodeau"
---
*****
Revolutionize Your Design Game: Unlock the Secret to Making Gimp Work Like Photoshop in Linux!

If you're a designer, you understand the importance of having a powerful image editing tool like Adobe Photoshop in your toolkit. But when it comes to working in a Linux system, Adobe Photoshop is not readily available. Fortunately, there is a free, open-source alternative that can revolutionize your design game - Gimp.

Gimp is a great tool for image editing, and it's available on Linux, but many designers find it challenging to switch to Gimp after years of working with Photoshop. The good news is that Gimp can be customized to work like Photoshop with a few tweaks and plugins.

Here are the steps to revolutionize your design game using Gimp in Linux:

1. Install the Gimp Plugin Registry

Gimp Plugin Registry is a collection of plugins that you can add to Gimp to increase its functionality. To install it, open a terminal window and type in the following command:

```
sudo apt-get install gimp-plugin-registry
```

2. Install the G’MIC Plugin

G'MIC stands for GREYC's Magic Image Converter, which is a plugin that adds advanced filters to Gimp. The G'MIC plugin replicates many of Photoshop's filters, and it allows you to create special effects, distortions, and more. To install the G'MIC plugin, type in the following command:

```
sudo apt-get install gmic
```

3. Customize Gimp's Interface

By default, Gimp's interface is different from Photoshop's interface, and this can be frustrating for Photoshop users. But you can customize Gimp's interface to look and work like Photoshop. To do this, go to Edit > Preferences > Interface, and then enable "Single-Window mode" and "Photoshop shortcuts."

4. Use Gimp's Photoshop-Like Features

After customizing Gimp's interface, you can start using its Photoshop-like features. Here are some examples:

- Use the Move Tool (shortcut: M) to move layers around.

- Use the Crop Tool (shortcut: Shift + C) to crop images.

- Use the Healing Tool (shortcut: H) to remove blemishes and other imperfections.

- Use the Clone Tool (shortcut: C) to copy pixels from one area to another.

- Use the Paintbrush Tool (shortcut: B) to add color to your images.

By following these steps, you can make Gimp work like Photoshop in Linux, and you'll be able to transition to a new image editing tool without sacrificing your skillset. Plus, Gimp is free, open-source software, so you won't have to spend any money on licenses or subscriptions.

In conclusion, if you're a designer working in Linux, Gimp is an excellent alternative to Adobe Photoshop. With a few tweaks and plugins, you can make Gimp work like Photoshop and revolutionize your design game. Give it a try, and let us know your experience!

{{< youtube 3qYkFow3BlA >}} 



There’s no denying that Photoshop is the gold standard in digital photo editing, with countless industry professionals relying on it daily to make their living. However, GIMP, its closest open source competitor, has been making huge strides in recent years to make itself a viable alternative.
 
Part of the barrier keeping Photoshop fans from embracing the open source GIMP is the different look, feel, and controls. It’s hard to break old habits, especially when those habits keep paying the bills. There are some simple ways to overcome that barrier, at least in part, by customizing GIMP to look and act more like Photoshop.
 
## Install the Photoshop Icon Theme
 
Obviously, Adobe isn’t going to be releasing the official Photoshop icon theme for GIMP any time soon, but a designer at Deviant Art, Doctormo, meticulously recreated the Photoshop icons and packaged them for GIMP. Head to the page and download the icons.
 

 
Unpack the zip once you’re done downloading. The resulting folder is hidden, so show hidden files on your system. (It’s Ctrl + H on GNOME.) That folder will be called “.gimp-2.8,” and you’ll use it to replace the existing version of the same folder in your /home directory. Rename the current one in case you need it again.
 
Next, move the unpacked folder to replace it.
 
If you’re working with GIMP 2.10, the directory structure is somewhat different.  Your profile directory is actually located at:
 
~/.config/GIMP/2.10
 
The same will apply, though. Rename that directory and replace it with the new one.
 
When you boot up GIMP again, you’ll notice the icons and styling more closely match Photoshop.
 
## Set the Photoshop Keybinds
 
The next step in making GIMP feel more like Photoshop is the keybinds. Any Photoshop user knows that keybinds, often called hotkeys, are an essential part of getting things done efficiently. If you’re used to the Photoshop ones, learning a whole new set on GIMP isn’t just daunting, it’s a total pain.
 
Luckily, someone already did the hardest part for you. You only need to import the keybinds. Download the keybind configuration and rename it to “menurc.” Then, copy it into “~/.gimp-2.8.”  Again, on GIMP 2.10 this would be “~/.config/GIMP/2.10.”
 
## More Photoshop Features
 
There are a couple of additional features and tweaks that will make GIMP feel more like home. These are simple things, but they can certainly go a long way in easing your transition to GIMP.
 
### A More Photoshop-Like Move Tool
 
The move tool in GIMP is similar to the one in Photoshop, but it isn’t exactly the same. That said, there is an option that you can use to make it behave more like Photoshop.
 
Select the Move Tool from the Toolbox window. In the right set of menus you’ll find the available options for the Move Tool. Check the box for “Move Active Layer.”
 
Now, save the change. Click on “Edit,” then “Preferences.” Select “Tool Options” and finally, “Save Tool Options Now.” You can either restart or keep using it.
 
### Snap to Canvas Edge
 
By default, GIMP doesn’t snap layers to the canvas edge or grid lines by default. Moving a layer, then, is much less exact. You can make GIMP snap layers to the canvas with a couple lines of configuration. Use your favorite text editor to open “~/.gimp-2.8/gimprc” or “~/.config/GIMP/2.10.” Add either or both of the following two lines, as you prefer.
 
If you’d prefer a more temporary option, GIMP already includes a “Snap to Canvas” option. You just need to enable it. Click on “View,” then select “Snap to Canvas” in the resulting menu.
 
These tips should bridge the gap between GIMP and Photoshop. Nothing is ever going to be exactly the same, but the feel should mostly be there, and much of your learning curve should be eliminated. GIMP is open source, too, so you can always do your own work and make even deeper modifications if you’re able.
 
Nick is a freelance tech. journalist, Linux enthusiast, and a long time PC gamer.
 
Our latest tutorials delivered straight to your inbox




