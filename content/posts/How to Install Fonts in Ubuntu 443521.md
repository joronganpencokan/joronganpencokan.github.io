---
title: "Unlock the Secret to Perfect Typography: Learn How to Install Fonts in Ubuntu Today!"
ShowToc: true 
date: "2023-01-17"
author: "Jan Watkins"
---
*****
Intro:

Typography is an essential element of design. It’s one of those elements that make everything pop in design. Without good typography, your design would look amateurish and flat. Unfortunately, not everyone knows how to install and use fonts in their designs, especially those using Ubuntu. In this article, you will learn how to install fonts in Ubuntu and unlock the secret to perfect typography.

Body:

Step 1: Find the font you want to install

The first step to installing your preferred font is to go online and find it. There are a wide variety of fonts to choose from, so you can sift through until you find something that suits your style. You can find free fonts on Google Fonts, Font Squirrel, and other sites.

Step 2: Download the font

Once you have found the font you want to install, download it to your computer. Fonts are generally in the “.ttf” or “.otf” format. Most websites provide a download button that will save the file to your computer.

Step 3: Copy the font file to the fonts directory

After the font has downloaded, you need to move the file to the fonts directory. To do this, open your home folder, press “Control+H” on your keyboard to show hidden files, and navigate to “.fonts.” If this folder doesn't exist, make it by right-clicking in the current directory and selecting "New Folder." Then, copy the downloaded font file into the “.fonts” folder.

Step 4: Refresh the font cache

After copying the font file to the “.fonts” directory, you need to refresh the font cache for the newly-installed font to be visible. Open a terminal and type the command: “fc-cache -fv” and press enter. This will refresh the font cache and make the new font available to Ubuntu.

Step 5: Use the newly-installed font

To use the newly-installed font, open your design software (e.g., GIMP, Inkscape, Scribus) and navigate to the font selection menu. You should see the newly-installed font in the list.

Conclusion:

In conclusion, typography is an essential design element, and with Ubuntu, it's easy to install and use new fonts. With a little bit of effort, you can have access to thousands of fonts that can help bring your designs to the next level. By following the steps outlined in this article, you're one step closer to unlocking the secret to perfect typography in Ubuntu.

{{< youtube fR4ThXzhQYI >}} 



Most people will probably consider the collection of fonts that comes with the latest version of Ubuntu as “more than enough.” Others, though, may need (much) more in their line of work. And some would like to have more choices. If you, too, would like to install more fonts in Ubuntu, read on, for this is precisely what this tutorial tackles.
 
## The Mainstay: Microsoft Core Fonts
 
As long as their installer is available, Microsoft’s Core Fonts will feature in every tutorial about adding fonts to a Linux installation. Some of them remain hugely popular, and you may need them, especially if you’re collaborating with Windows users. To install them, fire up your favorite terminal and enter:
 
## Individual Free Fonts
 
Ubuntu doesn’t come with every font under the sun by default. There are many more you can get individually, however, to extend your font collection. You can install them, as with any other package, using:
 
Replace “PACKAGE_NAME” with any of the following:
 
- fonts-cantarell
 - lmodern
 - ttf-aenigma
 - ttf-georgewilliams
 - ttf-bitstream-vera
 - ttf-sjfonts
 - ttf-unifont
 - fonts-entypo
 - fonts-isabella
 - fonts-mplus
 - fonts-prociono
 - ttf-anonymous-pro
 - ttf-engadget
 - ttf-staypuft
 - ttf-summersby

 
## All at Once
 
If you don’t only need one or two more fonts but have decided to drastically expand your collection with everything we mentioned up until now, don’t install each package individually. You can bring them all on board at once by combining their installation in a single apt command, like:
 
Copy the line above, paste it in your terminal, press Enter, and soon you’ll be playing with a ton of new fonts.
 
## Manual TTF Installation
 
If you already have a specific TrueType Font (or more) that you want to install, you only have to copy it to a specific folder.
 
First, make sure that what you have is in TTF format. If you downloaded some fonts from a site, they might be compressed in an archive that you will have to extract. We won’t get into details about how to do that since it depends on the archive format, and there are dozens available.
 
When you have one or more TTF files in a folder, to install them, move them to the hidden “fonts” folder in your Home directory with:
 
If you have more than one TTF file in a folder, you can move them all at once using:
 
This can be done as long as they all have a TTF file extension.
 
If you need the fonts to be available system-wide so other users can make use of them too, use this command instead:
 
## Update the Font Cache
 
If your fonts don’t show up in any application, you can try manually updating the fonts cache with:
 
For system-wide fonts:
 
If they still don’t appear, double-check that they were in TTF format and that you have copied them to the correct folder, “~/.fonts.” Check that they have been copied with:
 
## Converting your Fonts
 
If you own a font that is not in the otf or ttf format, and you want to use it in Ubuntu, one way you can do is to convert the fonts to ttf format. To do that, we can make use of the FontForge software.
 
- Install it in Ubuntu:

 
- Open FontForge and load up the font you want to convert
 - Without making any changes, go to “File -> Generate Fonts”. Save the file with .ttf extension.

 
With the newly generated .ttf file, you can now install it in Ubuntu with the above method.
 
## Fonts in Action
 
Your new fonts should be available in any application that supports the manual selection of TrueType Fonts. For example, run LibreOffice Writer, type something, select it with your mouse, and change the font from the pull-down menu. Your new fonts should appear among the previously available ones.
 
As you can see, it is very easy to install fonts in Ubuntu 20.04. If you have read our Ubuntu 20.04 review, you will know that it is fast and stable. Are you currently using Ubuntu 20.04? Tell us in the comments section below.
 
OK's real life started at around 10, when he got his first computer - a Commodore 128. Since then, he's been melting keycaps by typing 24/7, trying to spread The Word Of Tech to anyone interested enough to listen. Or, rather, read.
 
Our latest tutorials delivered straight to your inbox




