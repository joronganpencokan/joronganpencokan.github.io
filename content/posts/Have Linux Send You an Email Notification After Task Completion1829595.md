---
title: "Revolutionize Your Productivity: Discover How Linux Sends Email Alerts After Task Completion!"
ShowToc: true 
date: "2023-03-13"
author: "Brian Cargo"
---
*****
# Revolutionize Your Productivity: Discover How Linux Sends Email Alerts After Task Completion!

In today's era, one of the most valuable assets we have is time, and how we utilize it determines our productivity. In a world where technology dominates almost everything, being able to automate certain tasks can save time and increase efficiency. For those who utilize Linux, there is a fantastic feature that can revolutionize productivity - email alerts after task completion.

Linux is an operating system that has been around for many years and has become the backbone of many enterprises in various industries. One of the things that makes Linux stand out is its ability to integrate various packages to perform a specific task. With this integration, Linux can send an email notification to a specified email address informing users of a successful or failed task completion.

This feature can save valuable time as it eliminates the need to regularly check if tasks are completed, such as long-running scripts or backups. Instead, the user can relax and focus on other tasks, knowing that they will be informed immediately of task completion or failure through their email.

There are various ways to set up email alerts after task completion in Linux; one of the most common methods is using the mail command. The mail command is a simple yet effective way to send emails via the command line interface. To use this command, the user needs the necessary details like mail server address, recipient email address, and their email content.

Here is an example of how you can send an email notification after a task is completed using the mail command.

Syntax:

`<command to be executed>; mail -s "<email subject>" "<receipient_email>" <<EOF <email_body> EOF`

Example:

```
$ find /home/user/ -name *.txt -exec grep 'Hello' '{}' \; -print; mail -s "Task completed" "user@example.com" <<"DELIM"
Task completed, please check!
DELIM
```

In the above example, we are using the find command with the grep command to search for all the text files inside the "user" directory that contain the term "Hello." After the command successfully runs, the user will receive an email informing them that the task was completed successfully.

Linux has various tools that can send email notifications after task completion, and users can choose which tool works best for them, depending on their requirements.

In conclusion, Linux is a powerful operating system that can do more than we can imagine. By utilizing its various features such as email alerts after task completion, we can increase productivity and save valuable time by automating tasks. So go ahead, explore Linux and take advantage of its power to revolutionize your productivity!



**References:**

- https://linuxhandbook.com/send-email-from-linux-command-line/
- https://www.redhat.com/sysadmin/linux-automation-job-completion-email
- https://www.tutorialspoint.com/send-email-with-attachments-from-linux-command-line

{{< youtube PPQ8m8xQAs8 >}} 



In this article we’re going to take a look at how you can have Linux trigger an email alert once a certain condition has been met. We’re assuming you’re an intermediate or advanced user – which you should be, if you’re looking to set up email alerts on Linux – and that you have the mail client installed already.
 
Having an alert sent to you through email can be very useful. For example, if you have a large build being done in the background, it makes no sense to wait around for the process to finish. In such cases, you can have Linux send you a message once the build is done. It saves you a lot of time. You can also have an email alert sent to you at a certain time. If you have an engagement in the evening, you can program it into Linux so you don’t forget!
 
First, let’s take a quick look at how you can send an email to yourself. The command for it is “mailx” or “mail“. This command may be different on your system, depending on the version of Linux you’re running (and it will only work if the server has been setup properly). The command syntax is:
 
You can also attach a file to this, if you want
 

 
## Getting Linux to Trigger an Email Alert
 
Now, we can couple the command we used above with a conditional statement. This means that when the condition is satisfied, an email will be sent to you. Enter the following in the command line:
 
This can be done in another way too. Let’s look at another example. What if you were waiting for a server to respond? You can either keep typing commands in the shell or you can have an email alert delivered to you when the server wakes up. You can use this command, for example:
 
If you look closely, the code above is an infinite loop. When your system pings the server (servername), the loop gets broken and a mail will be sent to you. You don’t need to wait until a server has booted up or updated.
 
If you’re worried about system resources being spent, you can put the system to sleep by amending the command a little:
 
In this case, the computer will sleep for 200 seconds before it executes a new cycle. You also get a regular alert (that the loop is working) every few seconds this way.
 
You can put virtually any shell command as the condition (so long as it’s sensible and doesn’t overload your system):
 
What if you wanted to email yourself on a certain date at a certain time? You can change the command above a little like this:
 
If you were looking to receive notifications whenever you receive an email on your Linux system, you can install applications that support email notifications. Two of the more popular applications are PopTray Minus and Mail Notification.
 
You can experiment with the commands given above. The premise is simple – just design a condition statement which, when met, will trigger an email alert. If you need more info or help on how to use mailx, simply type “mailx --help“to display the help list.
 
Image Credit:  tux flag linux penguin red waving , gray mail envelope white postal letter,  memory reminders reminder dimensional control
 
I'm a techie with over a decade of programming experience, spread across a wide range of interesting, path breaking technologies. Now I'm sharing my passion for technology, and making tech easier, with everyone!  Hope you enjoy reading about, and playing with technology, as much as I do!
 
Our latest tutorials delivered straight to your inbox




