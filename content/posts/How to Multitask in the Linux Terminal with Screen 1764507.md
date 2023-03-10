---
title: "Boost your productivity and become a Linux master with this simple trick for multitasking in the terminal!"
ShowToc: true 
date: "2022-12-16"
author: "Jenna Latimore"
---
*****
# Boost Your Productivity and Become a Linux Master with This Simple Trick for Multitasking in the Terminal!

If you've been using Linux for a while, you know how powerful the terminal can be. It allows you to quickly execute commands, navigate through directories, and perform more advanced tasks that are difficult to accomplish using a graphical user interface. However, if you want to truly master the command line, you need to be able to multitask efficiently. This is where the "screen" command comes in handy.

## Meet Screen

Screen is a terminal multiplexer, which means that it allows you to run multiple terminal sessions within a single window. You can use it to split your screen into multiple panes, switch between them, and detach them from your current session. This way, you can continue working on a task even if you need to log out, shut down your computer, or switch to another window.

## Getting Started with Screen

First, you need to make sure that screen is installed on your system. You can check this by running the following command:

```
$ screen -v
```

If screen is not installed, you can install it using your package manager. For example, on Ubuntu, you can run the following command:

```
$ sudo apt-get install screen
```

Once you have screen installed, you can start a new screen session by running:

```
$ screen
```

This will create a new window within your terminal window. You can now run commands within this window just like you normally would.

## Using Multiple Panes

One of the most powerful features of screen is the ability to split your screen into multiple panes. You can use this to run multiple commands simultaneously without having to switch between different terminal windows.

To split your screen horizontally, press:

```
Ctrl-a "
```

This will split your screen in half, with the top pane showing your current session and the bottom pane showing a new one. You can run commands in both panes independent of each other.

To split your screen vertically, press:

```
Ctrl-a %

This will split your screen in half, with the left pane showing your current session and the right pane showing a new one. Again, you can run commands in both panes independently.

## Detaching and Re-Attaching

If you want to detach a screen session while it's running, you can press:

```
Ctrl-a d
```

This will detach the current session and return you to your regular terminal prompt. You can now log out, shut down your computer, or switch to another window without losing your place.

To re-attach a detached screen session, run:

```
$ screen -r
```

This will return you to the place where you left off in your screen session.

## Conclusion

With screen, you can become a Linux master by boosting your productivity and multitasking like a pro. By using multiple panes, detaching and re-attaching sessions, and switching between different terminal windows, you can become more efficient and get more done in less time. So why not give screen a try and see how it can improve your workflow today?

{{< youtube ZNNqkeeOdrk >}} 



Many people don’t know about screen, an excellent little tool, or “a terminal multiplexer,” if you want to get technical. I firmly believe everyone who uses the terminal, for whatever reason, should have it in their arsenal. It’s that useful.
 
Screen makes multitasking in the terminal dead easy. With it, you can run many tools in parallel, each in their session. After you run something in its own “screen,” you can then detach and re-attach to it at will. Being able “to leave things running in a detached session” allows you to jump between tools.
 
If you’re juggling lots of tasks in the terminal every day, you’re either already using it, or you’ll love it after you try it!
 
## Install screen
 
Screen is available for almost every distro under the sun – since it’s an old, tried and tested, albeit somewhat unknown, little treasure. To install it on Debian, Ubuntu, Mint or anything that uses apt, use:
 
In mere seconds you’ll be up and running, since it’s also small and without many dependencies.
 

 
## First session
 
We’ll only delve into screen’s basic features that will allow you to use it immediately. If you like what you see by the end of this tutorial, its manual page explains the extra functions, but we thought they’d be too much for the first introduction in its use.
 
To use it, just add it in front of anything you’d enter in the terminal. Let’s create a document in the popular nano editor as an example. If it’s not installed, available on your distribution, or if you prefer something else, swap “nano” with your choice.
 
By adding “screen” in front of the usual command, we ran it in one of screen’s sessions. It might look like it didn’t have any result, but as we’ll see in the next step, it did.
 
## Detach from session
 
Type something in nano and pressing Ctrl + A and then D on your keyboard. Nano º or whatever editor you were using – will disappear. In the terminal, you’ll see a message similar to:
 
Now you’re back to what you could refer to as the starting terminal from where you ran screen before. But your session with nano isn’t gone.
 
## Get back to the running session
 
Since you have a session running in the background, you can get back to it by entering:
 
After hitting Enter, you’ll be right where you left off in nano. You can detach and reattach the screen as many times as you like. But that’s just one app running in the background, far from what you’d call true multitasking.
 
## Create a second session
 
While back to the original terminal and detached from the running nano session, repeat the first step to run something in a second session. For simplicity’s sake, we created a second document with nano using:
 
Screen, though, isn’t restricted to running multiple sessions of the same app: try running anything with it. Screen proves its usefulness when used for something like compressing many files into an archive with 7z, a process that takes some time. Instead of staring at a terminal, waiting for 7z to finish, you can detach its session and let it run in the background.
 
## Session list
 
If you followed our previous steps, you now have two sessions running with screen. screen -r won’t work like before because it wouldn’t know where to attach. When you have multiple sessions, to go back to one of them, you first have to know its ID. To find it, enter:
 
Screen will display a list of all available sessions.
 
In our case, as you can see in our screenshot, to go back to either session, we’d have to enter:
 
or
 
## Useful extras
 
If you run a task that exits after completion with screen, the screen session will end with it. That’s why you could have run some tasks in screen sessions but now have no active sessions show up. The tasks could have completed their goals in the meantime.
 
If you want a session to remain active in such cases, instead of running a command with screen added before it, run “screen” on its own to create a new session, and then type your command there before detaching. If you run a command in a session you manually created, the session won’t exit when the task completes.
 
Screen also allows you to create a new session from within an existing one. Just hit the command combination Ctrl + A, and then press C to create a new screen and jump to it.
 
For other useful commands you’ll probably end up using, press Ctrl + A and then:
 
- A to enter a title for the session for easier recognition and management
 - K to kill the current session
 - N or P to move to the next or previous active session
 - 0 to 9 to move between the first ten active sessions

 
## Not just for juggling tasks
 
We saved the best for last: screen isn’t bound to a specific terminal. After detaching from a session, you can close the terminal window if you were in a graphic environment, or you can even log-out. As long as your computer is running, the session will remain active.
 
And this means that you can reattach to a running session from a different terminal. As you can see in our screenshot, we used Guake to reattach to a session we created in Mint’s default terminal.
 
Since the implications of this might not have adequately sunk in, think of this usage scenario: you can log in remotely to your computer, with SSH, and start a task with screen. Then, detach and log off. The job will keep running until it either completes or you decide to re-log on, reattach to the screen session and manually end it!
 
How’s that for “multitasking?”
 
OK's real life started at around 10, when he got his first computer - a Commodore 128. Since then, he's been melting keycaps by typing 24/7, trying to spread The Word Of Tech to anyone interested enough to listen. Or, rather, read.
 
Our latest tutorials delivered straight to your inbox




