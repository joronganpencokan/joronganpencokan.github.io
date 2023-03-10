---
title: "You won't believe how easy it is to launch Terminal in the current folder on your Mac!"
ShowToc: true 
date: "2022-12-02"
author: "Victoria Reed"
---
*****
Title: You won't believe how easy it is to launch Terminal in the current folder on your Mac!

Are you constantly frustrated with having to navigate to the right folder in Terminal every time you need to work on a project? Fear not, for there is a simple solution – launching Terminal in the current folder.

By default, when you open Terminal, it launches in your home directory. However, with a simple command, you can launch it in the same directory as the Finder window you have open.

Here's how:

1. Open Terminal
2. Type "cd " (without the quotes, but note the space after "cd") in Terminal.
3. Drag the folder you want to open into the Terminal window.
4. Press enter.

And voila, Terminal will now be open in the same directory as the folder you dragged in. 

But wait, there's more! 

If you don't want to type out "cd " every time you use this command, you can create an alias in your .bashrc file. Here's how to do that:

1. Open Terminal
2. Type "nano ~/.bashrc" (without the quotes) in Terminal.
3. Add the following line at the bottom of the file: "alias c='cd $(osascript -e "tell app \"Finder\" to POSIX path of (insertion location as alias)")'" (again, without the quotes).
4. Save the file by pressing Control + O, then exit nano by pressing Control + X.
5. Close and reopen Terminal for your changes to take effect.

Now, whenever you want to open Terminal in the current folder, all you have to do is type "c" (without the quotes) in Terminal, and you're good to go.

In conclusion, launching Terminal in the current folder is a simple yet powerful trick that can save you time and frustration. Give it a try, and see how it changes the way you work on your projects. Happy coding!

{{< youtube aKRYQsKR46I >}} 



Often while working with local files you may need to open a Terminal window in your current folder location. While doing that is as easy as pressing a button and clicking an option in Windows, things are different on Mac. 
 
You are required to first enable an option in your Preferences panel, and then you will have the option to launch an instance of Terminal in any folder of your choice – this was as true five years ago as it is on Big Sur today.
 
Here’s how you can launch Terminal in the current folder location on your Mac.
 
## Launch Terminal Window in the Current Folder on Mac
 
You do not need a third-party app to get the job done. All you need to do is visit the Preferences panel, tweak a few settings here and there, and you will be all set.
 
- Click on the Apple logo in the top-left corner on your Mac, and select “System Preferences…” You will be taken to the Preferences panel on your Mac.

 
- Click on “Keyboard” in the Preferences panel.

 
- Once in the Keyboard panel, click on the “Shortcuts” tab.

 
- In the Shortcuts panel, click on “Services” in the left-hand menu. Scroll down in the right-hand menu, and select the options that say “New Terminal at Folder” and “New Terminal Tab at Folder.” These options should be next to each other.

 
Click on “none” next to “New Terminal at Folder,” and press a key combination on your keyboard to assign a new shortcut key to the feature. That way you will be able to launch a Terminal window using a shortcut key instead of pulling up the menu and selecting the option to launch one.
 
- Once you have enabled the options and assigned a keyboard shortcut, you can close the Preferences panel.

 
- Open the parent directory where your folder is located. Then single-click on the folder where you wish to launch a Terminal window, click on “Finder” followed by “Services,” and select “New Terminal at Folder.” Or you can simply press the keyboard shortcut that you assigned before.

 
- A new Terminal window should launch in the current folder location allowing you to play around with the local files in that folder.

 
Launching a local instance of Terminal should now be easy for you. Should you ever wish to disable the feature, you can do so from the Preferences panel by just unchecking the boxes that you selected in the above steps.
 
## Frequently Asked Questions
 
### 1. Can I drag-and-drop folders into the Terminal?
 
Yes, if you keep the Terminal shortcut in your Dock, then you can open a specific folder in the Terminal by drag-and-dropping that folder from the Finder window onto the Terminal icon.
 
Alternatively, you can drag-and-drop the folder from Finder into an open Terminal window.
 
### 2. How do I navigate to a folder within the Terminal?
 
If you want to use the Terminal to navigate to folders, simply type cd followed by the directory you want to navigate to. For example cd Desktop or  cd Desktop/Downloads
 
To see the current directory you’re in in the Terminal, type pwd, which stands for “print working directory”.
 
If your work revolves around working with local files using Terminal, and you do not want to go through the hassle of providing full paths to the files, you can simply use the above workaround to have Terminal launched keeping your current folder as its current working directory. 
 
If you want to do the opposite, then see our guide on opening any folder from the Mac Terminal. We can also show you how to repair your macOS hard drive using fsck.
 
Content Manager at Make Tech Easier. Enjoys Android, Windows, and tinkering with retro console emulation to breaking point.
 
Our latest tutorials delivered straight to your inbox




