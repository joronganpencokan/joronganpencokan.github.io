---
title: "Revolutionize Your Workflow: The Ultimate Guide to Mastering Xfce's Task Manager for Streamlined Running Processes!"
ShowToc: true 
date: "2022-12-12"
author: "John Willard"
---
*****
# Revolutionize Your Workflow: The Ultimate Guide to Mastering Xfce's Task Manager for Streamlined Running Processes!

Are you looking for a way to optimize your workflow and streamline running processes on your Linux computer? Look no further than Xfce's Task Manager!

Xfce's Task Manager is a powerful tool that allows users to keep track of running processes, monitor system performance, and terminate processes that are causing issues. This guide will provide you with step-by-step instructions on how to use Xfce's Task Manager to master your workflow and create a streamlined system.

First, let's dive into some of the features of Xfce's Task Manager:

## Key Features of Xfce's Task Manager

- Process monitoring: Xfce's Task Manager allows you to keep track of all running processes on your system, including CPU and memory usage statistics.

- Resource management: the Task Manager provides a graphical view of your system resources, so you can easily identify any bottlenecks or issues with running applications.

- Process termination: with just a few clicks, you can kill a troublesome process that is consuming too much CPU or memory.

Now that you know some of the key features of Xfce's Task Manager, let's get into the nitty-gritty of how to use it.

## Step-by-Step Guide to Xfce's Task Manager

### Step 1: Launch the Task Manager

The first step is to launch the Task Manager. You can do this in a few different ways:

- Use the keyboard shortcut Ctrl+Alt+Del, which will open the Task Manager by default.

- Open the Whisker Menu and search for "Task Manager."

Once you have the Task Manager open, you'll see a list of all the current processes running on your computer.

### Step 2: Monitor Running Processes

The Task Manager shows you a list of all the processes currently running on your system. You can sort the list by different criteria, such as CPU or memory usage, to help you identify any resource-intensive processes.

### Step 3: Terminate Processes

If you notice a process that is causing issues, such as high CPU or memory usage, you can terminate it with just a few clicks. Simply select the process in the Task Manager and click the "End Process" button.

### Step 4: Monitor System Resources

In addition to tracking running processes, the Task Manager also provides real-time information on your computer's system resources, such as CPU and memory usage. You can view this information in graphical form to help you quickly identify any issues.

### Step 5: Set Priority for Processes

If you need to prioritize certain processes over others, you can do so in the Task Manager. Simply right-click on a process and select "Set Priority," then choose the level of priority you want to assign.

## Conclusion

By mastering Xfce's Task Manager, you can revolutionize your workflow and streamline running processes on your Linux computer. With its powerful features for process monitoring, resource management, and process termination, the Task Manager is an essential tool for anyone looking to optimize their workflow. So why wait? Start using Xfce's Task Manager today and experience the benefits of a streamlined system!

{{< youtube 1Zyw5NCQlbU >}} 



The Task Manager is one of the essential tools that come by default with most operating systems today. Although to the untrained eye, it appears as a live-updating list of all running processes.
 
It is, in fact, precisely that: a list of everything “active” on the computer at any moment. But what most people ignore is that it doesn’t only display those processes – it also allows you to act on them.
 
By learning how to “read” the presented information and tweak your processes, you take active control of how your computer operates.
 
There are many different task managers and, in the land of the penguins, a distribution can come with one or more of them by default. It’s a given that most, if not all, window managers also count a task manager among their basic set of applications.
 
For this article we’re using the Task Manager that comes with XFCE. The configuration in alternative options will be somewhat different, but you use them in almost the same way and achieve the same results.
 
## Run your task manager
 
We find there’s no need to offer any instructions on how to install a task manager. In virtually all cases, you’ll already have access to one. Find it through your distribution’s main app menu or by searching for “task” in any available installed-software search field and run it.
 
Even if yours isn’t the one we’re using here, it won’t look much different. A list of running processes will take up most of the window’s area, usually, by default, sorted by their name.
 

 
## Expand the window
 
Our title doesn’t refer to some hidden, esoteric function. We are merely suggesting to move around and resize the task manager’s window or to maximize it so that it covers your whole screen. The extra space will allow you to see more processes – and more details – at the same time.
 
Use the extra space to move around the columns so that you can easily view all available information. Just click and hold the left mouse button exactly where two columns intersect, and you’ll be able to drag their divider left or right.
 
## Sort by resources
 
Click on any column’s title, and the task list will be sorted accordingly. Click again, and the order will reverse. This is the best way to check which tasks are eating up your computer’s resources at any given moment, as we will see in action later.
 
## See everything
 
The task manager considers some information as “overload” and hides it by default. Theoretically, this makes everything more user-friendly. Practically, we believe it’s easier seeing you have 1GB of RAM available with a single glance, compared to having to math your way out of a “13 percent available” display.
 
Click the icon with the two cogs (or check your task manager’s “appearance” options, or try right-clicking on one of the columns and see if a Configure/Properties option shows up). This will allow you to tweak how the program displays everything.
 
As far as XFCE’s Task Manager goes, we suggest you enable everything but the “Hide into the notification area” option.
 
## Why Tree View helps
 
One of the options you enabled in the previous step, “Show processes as a tree,” changes the list to a hierarchical structure. This way, all running tasks won’t appear as individuals but, instead, as task groups.
 
Unlike individual tasks, task groups start from a single task that then spawns more tasks. And those can spawn more processes and so on. When in a tree view, those relations are displayed in a hierarchical way exactly like the typical file system display in most file managers – with files > inside folders > inside more folders > inside storage media > inside the computer.
 
That’s the reason a tree view can help when dealing with memory hogs: it enables you to realize the big picture. But that is, also, something we’ll see in the very specific example that follows.
 
## Tree View and the big picture
 
If you check your task manager with its default view on, you may see Firefox eating up from 50 to 200MBs of RAM. Then swap to Tree View and, lo and behold, there’s a “mother” Firefox process that’s spawned three more “children”
 
Tree View along with the  Firefox process allows you to see the actual total resources it’s eaten up. “Under” and “inside” it, you will see each spawned process that belongs to the mother process.
 
## Tame all resource hogs
 
If you re-run your task manager with root credentials, you’ll gain access to its two most important options: the Priority setting and the “Kill” function. Just sudo-run it from a terminal like the following command:
 
Running in root mode will enable you to change any task’s priority by right-clicking on it and selecting the appropriate option. Avoid setting any task to a “Very Low” or “Very High” setting; use only the Low, Normal, and High settings. Also, avoid playing around with anything you don’t recognize, as you can hard-lock everything by killing the wrong process or make your whole system crawl.
 
What you can, and should do, is set lower priorities for anything you recognize, deem insignificant, and rarely use – like the ModemManager (except if you are still using a modem). Add higher priorities to anything you want “acting more snappy.”
 
If, in the rare case, a program acts like it’s running, but is frozen and doesn’t allow you to interact with it. You can right-click and “kill” it.
 
Note that everything “in it” will go down in flames as well. If the frozen program was something like a word processor or graphics tool, where you had almost completed your latest masterpiece, it may be better to wait a bit more instead.
 
OK's real life started at around 10, when he got his first computer - a Commodore 128. Since then, he's been melting keycaps by typing 24/7, trying to spread The Word Of Tech to anyone interested enough to listen. Or, rather, read.
 
Our latest tutorials delivered straight to your inbox




