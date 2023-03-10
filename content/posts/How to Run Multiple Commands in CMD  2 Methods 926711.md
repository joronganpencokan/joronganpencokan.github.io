---
title: "Unleash Your Command Prompt Powers: Learn How To Run Multiple Commands Simultaneously with These 2 Genius Methods!"
ShowToc: true 
date: "2023-03-24"
author: "Meaghan Albers"
---
*****
# Unleash Your Command Prompt Powers: Learn How To Run Multiple Commands Simultaneously with These 2 Genius Methods!

Are you a power user who spends hours on the command prompt every day? Do you find yourself running the same set of commands over and over again? If so, you'll love these two genius ways to run multiple commands simultaneously on the command prompt.

## Method 1: Using the Ampersand (&) Operator

The first method is simple and straightforward. It involves using the ampersand (&) operator to run multiple commands in a single line. Here's how it works:

1. Open the command prompt.

2. Type the first command you want to run and press Enter.

3. Type the second command, followed by an ampersand (&), and press Enter again.

4. Repeat the process for as many commands as you want to run simultaneously.

For example, if you wanted to run three commands simultaneously, your command prompt syntax would look like this:

```
C:\> command1 & command2 & command3
```

When you press Enter, all three commands will run simultaneously, saving you valuable time and effort.

## Method 2: Using a Batch File

The second method involves using a batch file to run multiple commands simultaneously. A batch file is a script that contains a set of commands that are executed in sequence when the file is run. Here's how to use this method:

1. Open Notepad or any other text editor.

2. Type the commands you want to run, one per line.

3. Save the file with a .bat extension in a location of your choice.

4. Open the command prompt and navigate to the location where you saved the batch file.

5. Type the name of the batch file, followed by .bat, and press Enter.

For example, let's say you have a set of 10 commands you need to run every time you start your computer. You can create a batch file called startup.bat and save it in the Windows startup folder. Whenever you log in, the batch file will run automatically, executing all 10 commands simultaneously.

By using these two genius methods, you can save valuable time and effort when working on the command prompt. Whether you are a power user or a beginner, these tips will help you unleash your command prompt powers and take your productivity to the next level. Give them a try today and see the difference for yourself!

{{< youtube Jfvg3CS1X3A >}} 



There are plenty of things that you can do with the command prompt. For example, you can utilize the best CMD commands to perform basic stuff. Similarly, there are times when we want to run multiple commands on Command Prompt.
You can execute multiple commands on the Command prompt, but you must do it manually. What if I tell you that you can run multiple commands simultaneously in Command Prompt?

 
## Best Methods to run Multiple Commands in CMD


You can run two commands in one line in Windows Command Prompt. For that, you need to create a batch script file using Notepad. Below, we have shared the two best methods to run multiple commands in CMD on Windows 10 computers. Let’s check out.

 
### 1) Using Notepad


This method includes creating a batch script to run multiple commands. Using this, you can execute all your commands one by one automatically. For that, we are going to use the commands to reset the DNS cache of Windows 10 –

 

ipconfig /displaydns
ipconfig /flushdns
ipconfig /release
ipconfig /renew



1. First of all, open the Notepad on your computer.

2. Now, enter the commands you want to execute with a single click. In this example, we use the four commands mentioned above.

3. Next, click on the file and select Save as an option.

4. Now save this file with the .bat extension. For example, DNSreset.bat

5. If you wish to reset the DNS cache, double-click on the batch script file.

That’s it! You are done. This is how you can run multiple commands in Command prompt.

 
### 2) Using Special Characters


In this method, we will use some special characters between the commands to execute them simultaneously. Follow the steps given below.
1.  If you want to run two or more commands simultaneously, just insert the “&” between the commands. For example – ipconfig /flushdns & ipconfig /renew

2. If you want to execute the second command after the success of the first command, then use the “&&” between the commands. For example – ipconfig /flushdns && ipconfig /renew

3. If you want to run the second command only if the first one fails to execute, enter “||” between the commands. For example – ipconfig /flushdns || ipconfig /renew

That’s it! You are done. You can use these signs in between commands as per your wish.
So, this article is all about how to run multiple commands in CMD on Windows 10. I hope this article helped you! Please share it with your friends also. If you have any doubts about this, let us know in the comment box below.





