---
title: "Are you tired of struggling with font compatibility in Ubuntu? Learn how to convert any font to TTF format with this easy hack!"
ShowToc: true 
date: "2023-04-07"
author: "Lillian Murphy"
---
*****
Are you tired of struggling with font compatibility in Ubuntu? Learn how to convert any font to TTF format with this easy hack!

If you're an Ubuntu user, you've probably encountered some frustration when it comes to font compatibility. Certain font formats, such as OTF or Type1, aren't always recognized by the OS, leaving you with limited font options when designing documents or creating graphics.

Luckily, there's an easy hack you can use to convert any font to TTF format, which is widely recognized by Ubuntu and other systems.

First, you'll need to download FontForge, an open-source font editor that allows you to convert fonts to various formats, including TTF.

Once you've downloaded and installed FontForge, open the program and click on "Open" in the top left corner. Select the font file you want to convert and click "OK."

Next, go to "File" in the top left corner and select "Generate Fonts." In the pop-up window, choose TTF as the output format and click "Generate."

FontForge will then create a TTF version of your font, which you can save to your computer and install on Ubuntu or any other system.

With this simple hack, you'll be able to use any font you like in your Ubuntu projects, without worrying about compatibility issues. Whether you're working on a professional document or just designing a fun graphic, having access to a wide range of fonts can really enhance your work.

So why not give this hack a try and see how it can benefit your Ubuntu experience? Who knows, you may just discover a new favorite font that you never knew existed!


For those who are dealing with writing or design projects, it is common for you to come across a font that your application cannot support. It could be a Macintosh font, a bitmap font or an open type font (otf). For some reason or another, you just can’t get your Ubuntu machine to read them. In such cases, the best way is to convert these fonts to TrueType font (ttf).
 
Fontforge is an outline font editor that allows you to create your own postscript, truetype, opentype, cid-keyed, multi-master, cff, svg and bitmap (bdf, FON, NFNT) fonts. It also allows you to edit existing ones and convert one format to another.
 
## Installing Fontforge
 
The program is available in Ubuntu’s apt repository, so you can easily install the program by running the following command:
 
## Convert Fonts in Ubuntu using FontForge
 
- With FontForge installed, press the Win key, then type “fontforge.”

 
- Click the Fontforge icon to launch it.
 - Once Fontforge is up and running, load the font that you want to convert. This will load a preview of all the available glyphs for your font file.

 
- Press the “File” button on Fontforge’s Menu Bar and select “Generate Fonts.” This will open a small dialog box with a drop-down list where you can select the format that you want to convert to.

 
- Select “TrueType.”

 
- Press the “Generate” button on the dialog box’s lower left corner.

 
- Depending on the source file, it might generate some error messages. Click “Yes” to continue the conversion process.

 
## Using Fontforge’s CLI to Convert Fonts
 
Aside from running the Fontforge GUI, it is also possible to use the program to convert fonts from inside your terminal. This can be especially useful for users that want to create scripts that can automatically convert fonts on the fly.
 
By default, the CLI allows you to run Fontforge-specific functions. For example, running the following command will automatically convert an OTF font to TTF:
 
- The -lang=ff flag tells Fontforge to only use its built-in functions for this command.
 - On the other hand, the -c flag will load and run the built-in Fontforge functions in your terminal. In this case, the Open() function will load your font file to memory and Generate() will convert it to the format that you want.
 - Lastly, you need to provide the path for both your original and converted font. For this, you also need to write the proper file extensions for both fonts. This means that if you are converting from OTF to TTF, you need to write “.otf” at the end of the original font and “.ttf” at the converted one.

 
Next, you can also use a simple Bash for loop to run this command on an entire font directory:
 
## Convert Fonts using woff2
 
While Fontforge is a powerful font editing program, it does not properly convert some of the common font types. For example, WOFF2 is a format that most websites use today. As such, it can be an issue for users that want to use web fonts for their local documents.
 
To convert WOFF2 fonts, you need to first install the appropriate utilities for it. You can do this by running the following command:
 
Once that is done, you can now convert your WOFF2 font to TTF:
 
Similar to the Fontforge CLI, you can create a basic shell script to automate the process of converting WOFF2 fonts. For example, the following line of code will go through all the fonts in the current directory and convert it to TTF:
 
## Installing your New Font
 
With your new fonts available, you can now install them in your system. In order to do this, you need to first go to your home directory:
 
Create a new folder and name it “.font” (include the dot in front of the font) and copy the new ttf font into the folder:
 
Restart your application or reload your font cache. To do the latter, you need to run the following command:
 
You machine should be able to detect the new font now.
 
## Frequently Asked Questions
 
Image credit: Unsplash. All alterations and screenshots by Ramces Red.
 
### Is it possible to convert fonts back to WOFF2 format?
 
You can convert any TTF fonts to WOFF2 with the command: woff2_compress font.ttf.
 
### My fonts are not showing up after I converted them.
 
The most common cause is that your machine is missing the proper locale setting.
 
You can fix this issue by adding the following line: export LC_ALL=en_US.UTF-8 to your “.bash_profile” file.
 
Ramces is a technology writer that lived with computers all his life. A prolific reader and a student of Anthropology, he is an eccentric character that writes articles about Linux and anything *nix.
 
Our latest tutorials delivered straight to your inbox




