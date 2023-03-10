---
title: "Revolutionize Your Productivity: Discover How Taskbook in the Terminal Can Transform Your Task Management!"
ShowToc: true 
date: "2023-04-21"
author: "Edward Alvarez"
---
*****
# Revolutionize Your Productivity: Discover How Taskbook in the Terminal Can Transform Your Task Management!

Are you tired of traditional task management systems, such as sticky notes, physical journals, or digital apps that require cumbersome navigation? Do you crave a lean, personalized, and distraction-free approach to organizing your tasks, notes, and goals? If so, you might find your solution in the command line. Taskbook, a powerful yet lightweight task management tool specifically built for the terminal, can revolutionize your productivity and streamline your workflow. In this article, we will explore what Taskbook is, how to use it effectively, and why it can enhance your work and life.

## What is Taskbook?

Taskbook is an open-source, cross-platform, and terminal-based task management program that lets you create, edit, organize, and prioritize your tasks, notes, and tags in a flexible and intuitive manner. Developed by Ryan Palo in 2018, Taskbook is written in Node.js and is available under the MIT license. Its interface mimics a simple text editor, with a set of keyboard shortcuts that allow you to perform various actions without leaving the terminal. You can add new tasks, search for existing ones, mark them as done or undone, reorder them, and archive them with ease. You can also create notes, links, and code snippets, and attach them to specific tasks or tags. Taskbook saves your data as plain text files, so you can access and modify them with any text editor or version control system. Taskbook is designed to be fast, minimalist, and customizable, so you can adapt it to your needs and preferences.

## How to Install Taskbook?

To install Taskbook, you need to have Node.js and npm (Node Package Manager) installed on your computer. If you don't have them, you can download and install them from the official Node.js website (https://nodejs.org/). Once you have Node.js and npm, you can open your terminal and type the following command:

```
npm install -g taskbook
```
This command instructs npm to download and install Taskbook globally, meaning that you can use it from any directory in your system. It may take a few seconds to complete, depending on your internet speed and system configuration.

## How to Use Taskbook?

After you have installed Taskbook, you can start using it by typing the command `tb` in your terminal. This will launch Taskbook, displaying an empty screen with a welcome message and some instructions. Taskbook uses a syntax that resembles Markdown, a markup language for text formatting. Here are some basic commands that you can execute in Taskbook:

- To add a new task, type `t [description]`, where `[description]` is the name of your task. For example, `t Buy groceries`.
- To add a new note, type `n [content]`, where `[content]` is the content of your note. For example, `n Remember to add milk to the list`.
- To mark a task as done, type `x [task ID]`, where `[task ID]` is the ID number of your task. For example, `x 1` will mark the task with ID 1 as done.
- To mark a task as undone, type `o [task ID]`, where `[task ID]` is the ID number of your task. For example, `o 1` will mark the task with ID 1 as undone.
- To reorder tasks, use the `j` and `k` keys to move the cursor up and down, and use the `m` key to switch the task with the selected task. For example, if you want to move the task with ID 2 above the task with ID 3, you can type `j` twice to select the second task, and then type `m` and `j` again to move it up.
- To filter tasks, type `s [filter]`, where `[filter]` is the keyword or tag you want to search for. For example, `s groceries` will show all tasks and notes that contain the word "groceries".
- To archive tasks, type `a`, and then use the `j` and `k` keys to select the tasks you want to archive, and type `d` to confirm. Archived tasks will be saved in a separate file named `archive.md`.

Taskbook also supports some advanced commands, such as tagging tasks with `@` and `#`, linking tasks and notes with `[` and `]`, adding code snippets with ````, and customizing the appearance and behavior of Taskbook with a configuration file (`.taskbookrc`). You can find more information and examples on the official Taskbook website (https://github.com/klauscfhq/taskbook).

## Why Use Taskbook?

Taskbook stands out from other task management tools for several reasons:

- It is fast, lightweight, and terminal-based, meaning that it runs on any platform, requires only a small disk space and memory, and lets you focus on your tasks without distractions or clutter.
- It is flexible and customizable, so you can adapt it to your workflow, style, and preferences, and use it for a variety of purposes, such as project management, note-taking, journaling, and coding.
- It is transparent and portable, meaning that you own and control your data, and can access and modify it with any text editor or version control system. You can also share your data across devices and platforms without compatibility issues.
- It is free and open-source, meaning that you can use, study, modify, and distribute it for any purpose, and contribute to its development and community. You can also benefit from the support and feedback of other users and developers.

Taskbook can help you increase your productivity and achieve your goals by providing a simple and effective way to manage your tasks and notes. By using Taskbook, you can reduce the friction and overhead of traditional task management systems, simplify your workflow, and get more done with less effort. Taskbook is not a silver bullet or a one-size-fits-all solution, but rather a tool that empowers you to design your own productivity system that suits your needs and styles. You can combine Taskbook with other tools and techniques, such as Pomodoro, GTD, Eisenhower Matrix, and habit tracking, to maximize your productivity and creativity. Give Taskbook a try today and see how it can transform your task management!

{{< youtube T4wOlEr4hI4 >}} 



If you’d prefer to manage all your tasks directly from the terminal, Taskbook allows you to do that using simple commands. There’s no annoying GUI, nor waiting for pages to load. Everything is instant and only a keypress away. Let’s see how you can use it to organize all your tasks in the Terminal.
 
## Install Taskbook
 
The suggested ways to install Taskbook are through Yarn, NPM, or Snapcraft. The commands for this, as provided by the app’s documentation, are:
 
Since we are using it on Ubuntu 20.04, we’ll go the snap route. For easier use, it’s also suggested you use an alias for taskbook so you won’t have to type its full name to manage your tasks. You can add the alias “tb” to taskbook with:
 
## Adding Tasks And Notes
 
With Taskbook installed, to create a task, type:
 
Press Enter and your task will be added to Taskbook’s list. To add some more tasks, repeat this command like in the below example.
 
Check out your tasks: type tb and press Enter.
 
To add a note about something that won’t be an actionable task, use the -n switch instead of -t:
 
If you check out your task list after adding some tasks and notes, you’ll see notes start with a circle icon, whereas tasks have a classic checkbox on their left.
 
## Use the Boards, Luke!
 
For better task organization, you can use different boards. Each board can contain a different set of tasks and notes, but if you wish, a task or note can exist in more than one board at the same time. To add a task to a board, use:
 
In the following example, we’re adding two tasks, one to the “mte” board and one to the “pc” and “tablet” boards.
 
Notice that we didn’t have to create the board manually. Taskbook will have created the boards automatically and assigned the tasks to them, with one task existing on two boards.
 
## Acting on Tasks
 
To mark the tasks you’ve started working on as “active,” use the -b switch. When looking at how to select tasks, notice the number preceding each task. Select the task by specifying the number beside it.
 
You’ll see your active tasks marked with three dots (“…”).
 
To mark a task as “completed,” use the switch -c and the task’s number:
 
You can now see that the completed task is greyed out and has a checkmark beside it.
 
If a task you’ve marked as active takes too long to complete, you can pause or undo it using the same command you used to start it.
 
To mark your most important ones with a star, using the -s switch:
 
For even more control, you can use actual priorities. The syntax is somewhat more complex, though.
 
For example, to set our 2nd task’s priority to “normal,” our 1st task’s priority to “high,” and the 3rd task’s priority to “medium,” we used:
 
You can see in the following screenshot how the commands above marked our “Make Tech Easier” task as the most important, “Fix CSS” as medium priority, and left “Download Updates” unchanged at normal priority.
 
If you also noticed in our screenshot, we added a new task to our “tablet” board. But we also used p:2 before entering its actual text. The command in non-screenshot form was:
 
With the above, we’ve added the task “Flash new ROM” to the “tablet” board with medium priority. You can prioritize each task as you create it so you won’t have to edit it afterward.
 
But what if you added a task to the wrong board? Move it to the correct one with:
 
As you can see in our screenshot, you can move a task to more than one board at once.
 
After a while, though, your boards will be filled with tasks, and the completed ones will keep appearing in grey. To clean up your lists, use:
 
The above command “deletes” all completed tasks. To manually delete a task or note, use the switch -d and its number:
 
We used quotation marks with “delete” because the tasks and notes aren’t actually deleted. Instead, they’re archived. To access your archive of past tasks, use:
 
To restore any tasks from the archive to your boards, use -r followed by their number:
 
Note that you can restore more than one entry by using multiple numbers.
 
To see tasks from a specific board, use -l and the board’s name. In the following example, we’re only checking the tasks in our mte board:
 
Finally, when you have dozens of tasks in your boards, you can filter your lists with -f and a text string:
 
After you get familiar with Taskbook’s commands, you’ll be able to juggle all your tasks by only using your keyboard while working in the terminal.
 
Now that you know how to manage tasks in the terminal, do you still prefer a more visual way to manage your tasks? A web-based solution or an app you also use on your smartphone? Tell us in the comments section below.
 
OK's real life started at around 10, when he got his first computer - a Commodore 128. Since then, he's been melting keycaps by typing 24/7, trying to spread The Word Of Tech to anyone interested enough to listen. Or, rather, read.
 
Our latest tutorials delivered straight to your inbox




