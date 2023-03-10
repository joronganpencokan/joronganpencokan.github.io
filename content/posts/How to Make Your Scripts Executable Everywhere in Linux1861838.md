---
title: "Unlock the Secret to Linux Scripting: Learn How to Make Your Scripts Executable Anywhere!"
ShowToc: true 
date: "2023-06-07"
author: "Robert Pinder"
---
*****
Title: Unlock the Secret to Linux Scripting: Learn How to Make Your Scripts Executable Anywhere!

Introduction:
If you work with Linux operating system, scripting is one of the essential skills to have to increase productivity and automate tasks. It's a powerful way to perform actions in a sequence without having to do repetitive tasks manually. However, there may be times when you have created a script on one machine and need to execute it on another, but it fails to run. This is because the script is not executable on the new machine. In this article, we'll discuss how to make your scripts executable anywhere on Linux.

Step 1: Choosing a shell
To make your script executable, you have to choose a shell for your script to run. The shell is a command-line interface that interprets your script and executes it. There are various shells available in Linux, such as Bash, Zsh, Ksh, and more. To make your script portable, the recommended choice is Bash, as it's the default shell for most Linux distributions.

Step 2: Adding a shebang
The next step is to add a shebang (#!) at the beginning of your script. A shebang is a special character sequence that tells the system which shell to use to execute the script. It's essential to specify the correct path to the shell interpreter in the shebang. For Bash, the shebang should be #!/bin/bash.

Step 3: Making the script executable
After adding the shebang, you need to make your script executable. To do this, you have to set the execution permission of the file. To set the permission, use the chmod command. For example, if your script filename is script.sh, the command to make it executable is:

chmod +x script.sh

Now your script is executable, and you can run it by typing ./script.sh in the terminal. If you encounter a permission denied error, use sudo to run the command with root privileges.

Step 4: Testing the script on another machine
To test the script on another machine, you only need to copy the script to the new machine and run it the same way you did on the previous machine. As long as the machine has Bash installed, the script will run without any issues.

Conclusion:
Making your scripts executable anywhere on Linux is a crucial skill for any developer or system administrator. By following the steps outlined in this article, you can make your scripts portable and easily executable on any machine. Remember to choose the correct shell, add a shebang, and set the execution permission. With these techniques, you'll never have to worry about a script not running on a new machine again!

{{< youtube i0I1QGbN9C4 >}} 



When you created a Bash script and save it in a folder, you will find that you can only execute it when you are in that folder. Have you ever notice how ls, imagemagick, apache, and squid might be installed in different directories but accessible everywhere? That’s because their individual paths have been added to the “Path” variable. By adding more paths to it, you can make your scripts executable everywhere too.
 
Tip: Check out our regular expressions cheatsheet.
 
## Adding paths to Bash
 
Before we begin, we should explain that thanks to how Linux security works, you can tweak the Path on three different levels. Bash is the first of them. Everything we see here will affect Bash, and everything that runs in it, but have no effect “outside Bash.”
 
Let’s say you have a collection of scripts in a folder you want accessible from everywhere.
 
To pull this off, you can add their path to “~/.bashrc”. You can open up the “.bashrc” file (it is in your Home directory, but is hidden by default) in your favorite text editor, like gedit.
 
Go to the very end of the file and add:
 
For example, if you keep your executable scripts in folder “/home/myname/scripts”, the command would be:
 
To register the changes, save the file, exit the text editor and then type in your terminal:
 
After that, move to different directories and try to run your scripts from there.
 
## Adding paths to your profile
 
If you want the content of your folder accessible from outside the constraints of Bash, add it to the Profile variable instead.
 
Open the “.profile” file with your favorite text editor.
 
At the very end of the file, enter:
 
You have to logout and re-login to enable the changes.
 
In Ubuntu and its derivatives, it’s suggested you edit the “.pam environment” file instead of “.profile”. 
 
Open the “.pam_environment” file in the text editor. If the file doesn’t exist, create it. 
 
In it, enter:
 
Note that instead of a fully hardcoded path, and unlike in the profile file, here we use a variable. This way, each user’s “/home/USER_NAME/scripts” folder would be added to their path.
 
As when editing the “.profile” file, you have to log out and re-login for the changes to take effect.
 
## Adding paths to the environment
 
The proper way to have the contents of a folder accessible from multiple users who share the same computer is by adding it to the environment path variable. Fire up a terminal and enter:
 
The path variable there contains a bunch of folders in quotation marks, split by colons, similar to:
 
To include your own folder in that list, right after the last path, before the closing quotation mark, enter a colon and the path to your folder. If your folder was, again, “/home/your_username/scripts,” it should look like this:
 
Note that it doesn’t have to be in caps – we used them for emphasis, to help identify where and how you should include your folder.
 
As before, log out and re-login to apply the changes.
 
With the above tricks, you will be able to run your scripts from anywhere in Linux.
 
- How to Get Commands Explanation in Terminal with KmdrAn Even Better Way to Search Your Command Line History Basic Bash Commands for Linux Newbies

 
OK's real life started at around 10, when he got his first computer - a Commodore 128. Since then, he's been melting keycaps by typing 24/7, trying to spread The Word Of Tech to anyone interested enough to listen. Or, rather, read.
 
Our latest tutorials delivered straight to your inbox




