---
title: "Unlock the Secret to Efficiently Managing Compressed Files with Midnight Commander - You Won't Believe How Easy It Is!"
ShowToc: true 
date: "2023-04-27"
author: "Anika Viverette"
---
*****
Unlock the Secret to Efficiently Managing Compressed Files with Midnight Commander - You Won't Believe How Easy It Is!

Have you ever struggled with managing compressed files on your computer? The process of extracting and compressing files can be time-consuming and frustrating. However, there is a way to make this process much smoother and more efficient - with the use of Midnight Commander.

Midnight Commander is a popular file manager for Linux and other Unix-like operating systems. It is a powerful and flexible tool that makes it easy to navigate your computer's file system and perform a variety of tasks. One of the most useful features of Midnight Commander is its ability to manage compressed files.

Here's how it works. When you open Midnight Commander, you'll see a split-screen interface with two panels. The left panel displays the contents of the current directory, while the right panel is where you can view and manipulate the files in the selected directory.

To manage a compressed file, simply navigate to the folder where the file is located in the left panel. Then, select the file in the right panel - this will display the contents of the compressed file. From here, you can extract individual files or entire directories by pressing the F5 key. Alternatively, you can compress files or directories by pressing the F2 key.

One of the great things about Midnight Commander is that it supports a wide range of compression formats, including ZIP, GZIP, TAR, and RAR. This means that you can easily work with compressed files, no matter what format they are in.

Another useful feature of Midnight Commander is its ability to perform batch operations. For example, if you have a large number of files that you need to extract from a compressed folder, you can select all of them and extract them all at once. This can save you a lot of time and effort, especially if you're working with large files or complex directory structures.

Overall, using Midnight Commander to manage compressed files is a great way to streamline your workflow and make your life easier. With its intuitive interface and powerful features, it's a tool that every Linux user should have in their arsenal. Give it a try today and see how it can help you unlock the secret to efficient file management!

{{< youtube fJOkuaihAek >}} 



Do you often deal with compressed archives? It is easy to do so in your desktop, but in the server environment, it can be difficult to manage compressed files. With Midnight Commander, you can quickly select a bunch of files and folders and compress them to a GZ archive. You can also extract the contents of a BZ archive or enter those archives and either add or extract specific files to and from them. Let’s see how.
 
## Installation
 
Although Midnight Commander (MC for short) is not preinstalled in most Linux distributions, you can find it in their repositories. To install it on Ubuntu, Debian, and compatible distributions, enter your favorite terminal and use:
 
If you are on Red Hat, you can install it with:
 
Arch fans can bring it onboard using:
 
For Suse, try:
 
Windows fans aren’t left out since there is a native port of Midnight Commander for for the Microsoft OS, compatible with 32-bit Windows XP or newer. You can download the installer from its SourceForge page and install it as you would any other application on your computer.
 
## First Run
 
After installing Midnight Commander, you can run it from your terminal by typing mc.
 
Midnight Commander presents you with two panes. The active one you are currently on (by default, the left one) is used as the source for every file action. The other one works as the destination. If you select a bunch of files on the left pane and press F5, which maps to “copy,” the selected files will be copied to the directory presented in the right pane.
 
You can move between the two panes by pressing Tab on your keyboard. The 10 Function Keys work as shortcuts for the functions presented on the bottom of Midnight Commander’s screen.
 
By default, MC uses filenames for sorting. Since you want all your image files bundled together, sort contents based on file extensions.
 
Press F9 to access MC’s pulldown menus. 
 
Choose “Sort order … ” and change it to “Extension” from the options that appear.
 
After that, all files in the left pane will be sorted based on their extensions instead of the filenames.
 
## Compress Individual Files and Folders
 
Scroll up/down the list and press Insert to select (or deselect) entries. MC displays selected entries with a different color.
 
To compress all selected entries into an archive, press F2 to access the file menu. Move with the cursor keys to “Gzip or gunzip tagged files” or “Bzip2 or bunzip2 tagged files,” and press Enter to choose the format you prefer for your archives. It’s even quicker if you use the shortcut: Y for Gzip and B for Bzip2.
 
After a temporary jump to a terminal, you will find a compressed version of your files in the same folder.
 
## Compressing all selected files to a single archive
 
What if you wanted to compress all the selected files into a single archive? Midnight Commander doesn’t include such a function by default, but you can do it semi-manually.
 
Select a bunch of files as before.
 
Press F2 to access the file menu once again. This time press @ or select “Do something on the tagged files.” This option allows you to manually input a command that will act on the file selection.
 
Use your preferred archiver’s command for adding multiple files into a single archive but replace the files themselves with %s. This parameter corresponds to “everything selected in the active pane.”
 
For example, to compress files in 7z format, we used:
 
Soon after, an archive with the selected files appeared in the same folder.
 
## File Extraction
 
Extracting compressed archives is even easier with MC. Thanks to using a virtual filesystem to mount them as volumes, it allows you to act on the contents without extracting and recompressing them.
 
To extract a whole archive, select it and then press F2. Press Z or select “Extract compressed tar files to subdirectories” to do that. With MC, though, you don’t have to extract everything if you only need specific files or folders.
 
With your archive highlighted, press Enter to enter it. Yes, we know this sounded redundant, but it’s precisely what happens since MC allows you to get inside your archives and manage the content.
 
Just like with any normal folder, while inside an archive, you can select individual files and folders and press F5 to copy (extract) them to the destination pane. You can also press F6 to move them there, which means that after being extracted to your destination pane, they will be removed from your archive. You can also press F8 to remove something from your archive.
 
It’s also worth noting that if you want to jump back to a typical terminal for a while, you don’t have to exit Midnight Commander. Press Ctrl + O simultaneously, and MC will hide in the background, leaving you in the terminal where you launched it.
 
You can move back to MC using the same shortcut. To really exit MC, press F10 on your keyboard.
 
Another way to better manage compressed files is to create a self-extracting archive so you don’t have to worry about installing additional applications.
 
OK's real life started at around 10, when he got his first computer - a Commodore 128. Since then, he's been melting keycaps by typing 24/7, trying to spread The Word Of Tech to anyone interested enough to listen. Or, rather, read.
 
Our latest tutorials delivered straight to your inbox




