---
title: "Unlock the Power of Linux: Learn How to Multitask like a Pro with Screen!"
ShowToc: true 
date: "2023-05-10"
author: "James Neal"
---
*****
---
title: "Unlock the Power of Linux: Learn How to Multitask like a Pro with Screen!"
date: 2021-10-14T16:29:30+08:00
draft: false
---

If you're a Linux user, you probably already know how powerful the command line can be. However, one thing that can be a challenge when working in the terminal is multitasking. Sure, you can always open up multiple terminal windows, but that can quickly become unwieldy. Fortunately, there's an answer: Screen!

Screen is a powerful tool that allows you to create multiple terminal sessions within a single session. This means you can easily switch between different tasks without having to clutter up your screen with lots of windows. Screen even allows you to detach a session and come back to it later, making it perfect for long-running tasks.

Getting started with Screen is easy. Simply open up a terminal window and type the following command:

```
$ screen
```

This will create a new Screen session. You can then start running commands just as you would in a normal terminal window. However, there are a few key differences to keep in mind. 

The first difference is that you can create new windows within your Screen session. To do this, simply type the following command:

```
Ctrl-a c
```

This will create a new window within your session. You can switch between windows by typing the following command:

```
Ctrl-a n
```

This will switch to the next window within your session. You can also switch to a specific window by typing its number:

```
Ctrl-a [number]
```

The second key difference is that you can detach a session and come back to it later. To do this, type the following command:

```
Ctrl-a d
```

This will detach your session, allowing you to continue working in other terminal windows. To reattach your session later, type the following command:

```
$ screen -r
```

This will reattach your session and bring you back to where you left off.

Screen is a powerful tool that can help you become a more efficient Linux user. With its ability to create multiple terminal sessions within a single session, you can easily switch between tasks without cluttering up your screen with lots of windows. And with its ability to detach and reattach sessions, you can even work on long-running tasks without having to keep a terminal window open the whole time.

So if you're a Linux user looking to become a multitasking pro, give Screen a try!

{{< youtube V1y-mbWM3B8 >}} 



I’ll admit up front – it’s embarrassingly late for me to have discovered screen. Friends and coworkers have been suggesting it to me for years, but it wasn’t until recently that I had a concrete need for it. Now I wish I’d had it all along. In short, screen gives you the equivalent of the “workspaces” you find in Gnome, KDE, and other desktop environments, but for the command line. It may not sound like much, but like the graphical equivalent, you begin to see the power after a few uses. Today we’re going to cover some screen basics useful for your home desktop but especially useful if you use remote access tools like SSH.  
 
## Overview
 
Let’s say you’re at the command line, and you’re running a long process like a kernel recompile. On some machines, that can take up to an hour. An average user might sit and wait. A clever user might background the job, or use the function keys to open a new TTY login. A screen user, however, has already thought ahead. Had screen been launched first (or automatically – more on that later) that user would just hit the proper key combo to create a new shell. And another, and another, if desired. Each one operates independently of the others and all output will remain on the appropriate screen session.  
 
Some of you who like to use the Alt + Ctrl + (F1 through F4) method may wonder how screen is any better. Several reasons actually, some of which would be:
 
- Not limited to number of function keys
 - Ability to name each screen
 - Ability to detach/reattach screen sessions
 - “Status Bar” support
 - Multi-user shared screens
 - Split screens

 
A LOTS more.  
 
## Getting Started
 
As screen is included in nearly every major Linux distro, this guide will not cover installation. The simplest way to launch screen is to just open a terminal and type
 
You might get a welcome screen, but otherwise you may not notice anything different. It just looks like a normal terminal right?  
 

 
What you’re actually seeing is the default screen session, and you can think of it as a layer over your shell. Should you exit or detach the session, you’d be returned to your normal screen-less shell.  
 
## Adding and Navigating Screens
 
For starters, you’ll need to know one major key combo. This is the “magic” key combo that lets you access all the individual commands. What is this magical combination?  Ctrl + A.  For example, Ctrl + A followed by c will create a new screen. Ctrl + A and n will move to the next screen in line (if one exists). The following includes many of the most common action keys (all keys are case-sensitive):
 
- c – Create a new screen
 - n – Move to next screen
 - p – Move to previous screen
 - S – Split screen into stacked regions
 - | – Split to side-by-side regions (might not work on all systems)
 - d – Detach screen
 - A – Set screen title

 
## Attaching/Detaching Screens
 
While there are many great uses for screen, this function could be called screen’s bread and butter. The ability to detach a screen, leaving it running, and pick it back up later is invaluable.  
 
Let’s say you’re running the Minecraft server from last week, and it’s running on an old PC under your bed. Normally if you wanted to, say, enter commands at the server console, you’d have to pull out the machine, dig out a keyboard and monitor, run your commands, and push it all back. Had the server software been started in a screen session, you can just SSH into the server, re-attach the screen, and do what you need. When done, detach the screen, and the server will keep running even after you close the SSH session. Days/weeks/months later, you can log back into the server and reattach that screen to enter new commands.  
 
## .screenrc
 
Finally, we could not cover screen without at least a brief mention of the “~/.screenrc” file. There are many many uses for this file, but as this is an introductory guide, we will not cover all possible options. Instead, we’ll just point out the well-loved hardstatus setting.  
 
This option gives you a fantastically useful info bar that will persist across all screen sessions. Typically, it’s placed at the bottom and holds info such as time, hostname, and title/number of the current screen.  
 
You can find example hardstatus codes all over the net with your preferred search engine, but here are a few to get you started. 
 
## #1
 
## #2
 
## #3
 
Josh Price is a senior MakeTechEasier writer and owner of Rain Dog Software
 
Our latest tutorials delivered straight to your inbox




