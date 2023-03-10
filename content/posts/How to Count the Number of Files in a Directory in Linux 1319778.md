---
title: "Discover the Surprising Hack to Quickly Count Files in Your Linux Directory!"
ShowToc: true 
date: "2023-06-29"
author: "Ronald Cory"
---
*****
Discover the Surprising Hack to Quickly Count Files in Your Linux Directory!

As a Linux user, you must have faced the challenge of counting files in a directory without knowing the exact command to use. Sometimes, the task can be frustrating and time-consuming, especially when you have to deal with a large number of files.

However, there is a surprising hack that you can use to quickly count files in your Linux directory. It involves using the "find" command with the "wc" command.

Here is how it works:

Step 1: Open your terminal and navigate to the directory you want to count the files.

Step 2: Type the following command:

`find . -type f | wc -l`

This command will find all the files in your directory and its subdirectories, and then pipe the output to the "wc" command, which will count the number of lines. Since each line represents a file, the final output will be the total number of files in the directory.

Step 3: Hit the "Enter" key, and within seconds, you will see the total number of files in your directory.

Isn't that surprising? This simple hack can save you time and frustration, especially when you have to count files in a directory frequently.

However, it is important to note that the command will count all files in a directory, including hidden files. If you want to exclude hidden files, you can modify the command as follows:

`find . -type f -not -path '*/\.*' | wc -l`

In this modified command, the "-not -path '*/\.*'" option tells the "find" command to exclude hidden files. This will ensure that the number of files counted excludes the hidden files.

In conclusion, the "find" command with the "wc" command is a surprising hack that you can use to quickly count files in your Linux directory. Now that you know this trick, you can save time and eliminate frustration when counting files in your directory.

{{< youtube EFLvHMJ5PHk >}} 



When you have a folder full of files (and sub-folders) you might need to find out how many files are there altogether. Counting files and folders one by one is certainly not an option, especially when there are less gruesome ways to do it, such as the following.
 
## 1. Check with File Manager
 
Let’s start with the easiest way. Just open the directory in a file manager and look at the status bar.
 

 
If you don’t see a status bar, check “View -> Status bar” in the menu to see if the status bar is enabled.
 
The disadvantage of this method is that it counts a folder as one item but doesn’t count the number of files in it. Actually, the figure you are getting for how many files are in the directory is the sum of the number of folders and the number of separate files in this directory. If you want to view them separately (e.g. the number of files or the number of directories only), you need to select them, and then the status bar will show the number of the files/directories in the selection only.
 
## 2. Select the Files/Directories You Want to Count
 
In addition to showing the number of all files and folders in a directory, File Manager will allow you to do more. For instance, if you want to count only files or only folders, or only a part of the files/folder in a directory, just select them, and the status bar will show the number of files/folders in the selection. For example, if I wanted to see the number of the JPEG files only, I would select them. The result is shown in the status bar.
 
## 3. Get More Advanced Statistics with the Properties Window
 
The status bar looks great if you don’t have a lot of files and folders, but if you do, there are better ways to count them. For instance, the below image is of a directory listing of one of my working folders.
 
You see, it’s only directories with lots of files in each of them. The File Manager doesn’t show this, but if I select them and right click to open “Properties,” the Properties window tells me how many there are.
 
I guess the output varies from one file manager to another because I do recall seeing a different output (like a separate number for files and for folders), so what you get depends a lot on the file manager you are using.
 
## 4. How to Count the Number of Files via the Terminal
 
If the simple ways of counting files and folders don’t work for you, or if you are a terminal person, the good news is there are numerous ways to get some data about your files and folders via the terminal. For instance, if you simply want a number, use this:
 
This command returns just the number of files/folders. To count files recursively, use this:
 
I noticed that there is a difference in the numbers I get via the Properties window and via the console, and I assume this is because the console doesn’t count the directories or something.
 
There are other commands for directory listings such as list commands you can use to get a file number, among other things, but I am not going to discuss them. These commands come with many parameters, and the exact syntax varies from one Linux shell to the next. If you are interested in them, check the documentation of the shell you are using.
 
I am a fulltime freelancer who loves technology. Linux and Web technologies are my main interests and two of the topics I most frequently write about.
 
Our latest tutorials delivered straight to your inbox




