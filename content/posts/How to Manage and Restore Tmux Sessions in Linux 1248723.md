---
title: "Revive Your Linux Productivity: Master the Art of Managing and Restoring Tmux Sessions!"
ShowToc: true 
date: "2023-06-29"
author: "Christopher Simmons"
---
*****
Revive Your Linux Productivity: Master the Art of Managing and Restoring Tmux Sessions!

Are you tired of losing your work in Linux when your terminal closes or your SSH connection drops? Have you ever wished for a way to keep your Linux sessions active and organized? Look no further than Tmux, the terminal multiplexer that lets you manage multiple sessions and windows within a single terminal window.

Tmux is a powerful tool for managing Linux sessions, and it's especially useful for remote work, where you may need to keep your work going even after you disconnect from a server. With Tmux, you can create and organize sessions, and then detach and reattach them as needed. This means you can switch between tasks, detach from a session when you're finished, and then reattach to it later with all your work intact.

Here's how to get started with Tmux and make the most of this powerful tool:

Installation

Tmux is available for most Linux distributions and can be installed using the system's package manager. For example, to install Tmux on Ubuntu, you can use the following command:

$ sudo apt-get install tmux

Creating a Session

To create a new session, simply run the following command:

$ tmux new-session

You will be presented with a new terminal window inside the current terminal window. This new window is your Tmux session.

Now you can start working in this window just like you would in any other terminal window. Tmux allows you to split the window into multiple panes, resize them, and move between them. Here are some basic commands to get started:

- Split the window horizontally: Ctrl+b and %
- Split the window vertically: Ctrl+b and "
- Switch between panes: Ctrl+b and arrow key
- Resize panes: Ctrl+b and +/- key

Detaching and Reattaching a Session

When you're ready to detach from your session, simply type:

$ tmux detach

Your session will continue running in the background. You can then close the terminal window or disconnect from your remote server without losing any work.

To reattach to a session, use the following command:

$ tmux attach

By default, this will reattach you to the most recently used Tmux session. If you have multiple sessions running, you can specify which one you want to attach to with the -t option:

$ tmux attach -t session-name

Managing and Restoring Sessions

With Tmux, you can easily manage multiple sessions and restore them as needed.

To list all active sessions, run:

$ tmux list-sessions

This will show you a list of all the Tmux sessions that are currently running. You can then attach to any of these sessions using the attach command with the appropriate session name or ID.

If you want to restore a session that was running but has since been detached or closed, you can use the following command:

$ tmux attach-session -t session-name

This will restore the specified session and all of its windows and panes.

Conclusion

Tmux is a powerful tool for managing Linux sessions and keeping your work organized and intact. With Tmux, you can easily create, detach, and reattach sessions, switch between windows and panes, and even restore sessions that were previously closed or detached.

By mastering the art of managing and restoring Tmux sessions, you can become more productive and efficient in your Linux workflow. Give it a try and see how Tmux can revolutionize the way you work in Linux!

{{< youtube BHhA_ZKjyxo >}} 



Tmux is a terminal multiplexer that comes stocked with a wide range of useful features and is backed by a surprising number of community-made plugins. Terminal multiplexers like tmux and Screen give your terminal window super productivity powers, allowing you to open multiple sessions in tabs and split screens. Combined with multiple terminal tools and session saving, you can also restore Tmux sessions after a hard reboot.
 
## Installing tmux
 
Getting tmux ready and running on your system is relatively simple if you are using a Linux distribution.
 
For Ubuntu, this means summoning apt from your terminal and installing the package from the distribution’s official repository. For other distros, use your included package manager to handle the installation. (tmux is available on most distributions.)
 

 
Got it? Great! Now, let’s split our screen.
 
## Creating Windows and Panes
 
In tmux, two terms are used to describe the main types of layout configurations we can create. “Windows” are the tmux term for tabs. Creating a new window will make a tab that you can switch over to with a simple command.
 
“Panes,” on the other hand, are splits in the current “Window” or tab that can also be switched to using a command.
 
Before we begin creating these, it is important to note that tmux is modal in function. What this means is that interactions with your terminal session and with tmux happen in separate “modes.” This is useful as you can use each individual terminal session you open normally without accidentally activating a tmux command.
 
To gain access to tmux and begin issuing commands, we’ll first start our new tmux session and name it:
 
Feel free to change the name (“babytmux”), of course!
 
Tmux should open immediately, and a new shell session should start up for you. But we want more than one, remember?
 
To enter tmux’s command mode, we’ll need to use the prefix. This is usually Ctrl and b pressed simultaneously. Alone, you won’t notice anything changing by pressing the prefix, but we can type out commands by entering : immediately after. To leave command mode, either complete the command by pressing Enter or press the ESC key to exit without making changes.
 
Tip: Get our Tmux keyboard shortcuts cheatsheet for a complete overview of basic keybindings.
 
We’ll use a shortcut to create a horizontal split: Press Ctrl and b, then "
 
Cool! Now, we can navigate between the two with the following: Ctrl and b, then o.
 
Each session is independent of the other, so we can open separate programs in each. Let’s quarter our screen with vertical splits and try it out: Ctrl and b, then %
 
Open whatever you want in each pane, and it will keep running while you access the others.
 
To make a window, use the following: Ctrl and b, then c
 
You can switch back to a previous window or move forward one window with:
 
Ctrl and b, then p
 
or
 
Ctrl and b, then n
 
The status bar at the bottom of the screen shows you a process that is running in each window and which window you are on (with “*”) for reference.
 
To leave this tmux session, use this: Ctrl and b, then type :detach-client
 
Your session will not stop running unless your machine is rebooted or you manually cancel it. To access it again, use this:
 
To create truly immortal tmux sessions that can come back after a reboot, we need to install a plugin or two.
 
## Installing Plugins
 
Using plugins in tmux is relatively straightforward. However, there is a plugin manager we can install to make subsequent plugin installations easier.
 
### Plugin Manager
 
To install Tmux Plugin Manager, we will clone its files from Github with the following code:
 
Next, add the following code to “.tmux.conf” in your home folder:
 
As you can see above, we will need to add the github username and plugin name (found in a plugin’s github URL) for each plugin we want to install from now on. The plugin manager will handle the rest. Use this code to get the plugin manager working:
 
Now, for the plugin we need to restore sessions after rebooting, keep reading.
 
### Resurrect
 
Tmux Resurrect does just what its name suggests and brings your saved session back to life using a simple command.
 
This plugin can be installed by adding the following to your .tmux.conf file:
 
Now, let Tmux Plugin Manager install it by using the following command in tmux: Ctrl and b, then I (This is “i” in UPPERCASE.)
 
Once installed, we can start a session and save it with the following: Ctrl and b, then Ctrl + s
 
To restore our session, we can use Ctrl and b, then Ctrl + r
 
Using the above, you can maintain an immortal tmux session with all of your preferred tools and processes in place even after rebooting. Give it a try and explore more of tmux’s features to get the most from your terminal.
 
Jeff is a long time laptop lover and coding hobbyist. His interests span the gamut from DAWs to Dapps and beyond. He runs a music/arts site at Odd Nugget.
 
Our latest tutorials delivered straight to your inbox




