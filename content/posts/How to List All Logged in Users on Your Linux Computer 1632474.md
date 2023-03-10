---
title: "Unlock the Secret to Revealing All Your Linux Computer's Active Users with this One Simple Trick!"
ShowToc: true 
date: "2023-07-06"
author: "Kim Towle"
---
*****
Unlock the Secret to Revealing All Your Linux Computer's Active Users with this One Simple Trick!


Are you currently running a Linux-based computer that you share with other users? Do you ever wonder who’s been on the computer besides yourself? If so, you’re in luck! There is a simple trick to unlocking the secret of revealing all your Linux computer’s active users.

Firstly, open the terminal application. Once the terminal is open, all you need to do is type in the following command:

```
w
```

By entering this command, you will be able to see all the active users on the system and their activities. The output will provide you with information such as the username, the terminal used, the time the user logged in, and their activity (whether they are idle or actively using the system).

The “w” command stands for “who” and is used to display information about the users who are currently logged in to the system. It is a simple yet powerful command that is often overlooked by Linux users. This command is also useful for system administrators who need to monitor user activity on the system.

In addition to the “w” command, there are other commands that can be used to view active users on the system. For example, you can use the following command to display all logged-in users’ usernames:

```
who
```

This command provides similar output to the “w” command but does not display users’ activity.

Another command that can be used to view active users is the “users” command. This command displays a list of users who are currently logged in to the system:

```
users
```

Whichever command you use, if you’re a Linux user who shares a computer with others or an administrator responsible for monitoring user activity, understanding who is currently using the system is essential for security and accountability purposes.

In conclusion, whether you’re a Linux novice or a seasoned user, the “w,” “who,” and “users” commands are valuable tools for unveiling all your Linux computer’s active users. This simple trick can help you keep track of system usage and ensure your computer’s security. So, the next time someone asks, “Who’s been on the computer?” you’ll be able to reveal the answer with ease.

{{< youtube AOHI9U8phDw >}} 



For your Linux system, it’s possible to have multiple users connected to a computer at the same time. The good thing is, you can easily find out who is on board and connected to the system. Learn how to list logged-in users on your Linux computer.
 
## 1. Using the “who” command
 
We use the who command to get information on the different users connected with the information displayed in four columns.
 
- The first column shows the usernames.The second column indicates the TTY used.The third column is the time the user logged in.The fourth is the hostname or IP address of the connected users.

 
You can also display the number of users logged on to the system with the -q parameter.
 
It is possible to have more information by displaying all details of the current logged-in user with the -a option.
 
You can get more details on how to use the command by using the --help command if you need additional information.
 
## 2. Using the “w” command
 
Contrary to the who command, the w command shows the users who are logged in and what they are doing.
 
The output shows some useful information such as:
 
- current timehow long the system has been runningnumber of users currently logged inname of the logged-in userremote hosttime the user logged in

 
You can also display just the information about the logged-in users when you use the -h option.
 
You can filter the output of the command by using some other options. It’s possible to have a full list of the different options and their roles with the w --help command.
 
## 3. Using the “users” command
 
There is also the simple command users that shows only the users currently logged in without a parameter.
 
That command doesn’t give additional information like the other commands, but you still have an idea about the users currently logged in to the system. When you use the man users command, you see that there is no other information.
 
## 4. Using the “last” command
 
There is another command that we can use. The last command with the -a parameter gives you some information, such as the username (even the special users like “reboot”), TTY, IP address from where the users are connected, and some others.
 
When you use the -p parameter, it is possible to display the users connected to the present day.
 
The command also offers more options that can help you to have useful information. You can check with the man last command.
 
With all the commands above, you can easily list the logged-in users on Linux. This will allow you to monitor your system and see if there is any unauthorized access. You can take some actions with the identified users, if needed, with these users management commands.
 
Image credit: Panda for helping little skaters to teach skate on ice by Yayimages 
 
A Linux system administrator passionate about Open-Source environments and working on installations, deployments for different IT solutions and cloud environments. I like to share my knowledge regarding the technologies that I can discover and use
 
Our latest tutorials delivered straight to your inbox




