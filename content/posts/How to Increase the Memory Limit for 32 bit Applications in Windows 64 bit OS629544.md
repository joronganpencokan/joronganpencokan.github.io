---
title: "You Won't Believe the Simple Trick to Boosting Your 32-Bit App Performance on Windows 64-Bit!"
ShowToc: true 
date: "2023-05-01"
author: "Julie Bolden"
---
*****
You Won't Believe the Simple Trick to Boosting Your 32-Bit App Performance on Windows 64-Bit!

If you are using a 32-bit application on a 64-bit Windows system, you may be experiencing some performance issues. This is because the 32-bit application is not optimized to run on a 64-bit system. It is important to note that this problem is not limited to Windows systems alone; it can also be experienced on Mac and Linux systems. However, in this article, we'll focus on how to improve the performance of your 32-bit application on a 64-bit Windows system.

The good news is that there is a simple trick to improve the performance of your 32-bit app on a 64-bit Windows system. This trick involves using a program called "CorFlags.exe," which comes with the .NET Framework. CorFlags.exe is a command-line tool that allows you to set the 32-bit flag of an executable file. When you set this flag, it tells Windows to run the application as a 32-bit application, even though it is being executed on a 64-bit system.

Here is how to use CorFlags.exe:

Step 1: Open a command prompt by pressing the Windows key + R on your keyboard and typing in "cmd" in the Run dialog box.

Step 2: Navigate to the directory that contains the executable file of your 32-bit application using the "cd" command.

Step 3: Type in the following command: "CorFlags.exe /32BIT+ your_app.exe" (replace "your_app.exe" with the name of your application).

Step 4: Press Enter. You should see a message that says "CorFlags conversion success."

Step 5: Launch your 32-bit application and see if the performance has improved.

If this trick does not work for you or if you prefer a graphical user interface, you can use a tool called "CorFlags GUI," which is available for download online. CorFlags GUI is a user-friendly tool that allows you to easily set the 32-bit flag of an executable file.

In conclusion, if you are experiencing performance issues with your 32-bit application on a 64-bit Windows system, using the CorFlags.exe tool could help improve its performance. Give it a try and see if it makes a difference.

{{< youtube PjbV-PQycT8 >}} 



Most of us are now probably using a 64-bit Microsoft Operating System like Windows 7 x64 or Windows Vista x64, which allows the computer to address more than 3GB of RAM. Did you know, however, that any 32-bit applications you run are still limited to making use of only 2GB of RAM? This includes many games and probably the version of Microsoft Office you have installed, unless you specifically opted to install the 64-bit version.
 
You might wonder why this is a problem. Well, obviously if your system has more than 2GB of RAM, it’d be great to allow your applications or games to make use of it. Furthermore, some applications actually crash when they hit this limit, or start popping up boxes with out of memory errors. If you work on large excel files (500,000 rows+) then you’ll know what I’m talking about.
 
## The Solution
 
Thankfully, there’s a solution! A great coder by the name of Daniel Pistelli has written a little patching application that will modify your 32-bit programs, and allow them to address up to 4GB of RAM. It’s important to remember that this utility is only useful if you are running a 64-bit OS. If you don’t know what I’m talking about, then here’s an easy way to check:
 
1. Go to Control Panel, and click view by “small icons” in the top right hand corner
2. Click System
3. As per the image below, next to System Type, it should say 64-bit operating system. If it doesn’t then this utility is of no use to you.
 

 
The second thing to remember is that this utility can only be used on 32-bit applications. If you are unsure if an application you are running is 32-bit, run task manager by pressing CTRL-SHIFT-ESCAPE. Click the tab for processes. A list of currently running programs will load. Find your application in the list, and look to see if it has *32 next to it. The example image below illustrates what I mean.
 
## Using the patch
 
Assuming that you’ve followed the previous two points and now wish to patch your 32-bit application, first backup the executable file of the program you wish to patch. If the patching process fails, or if you need to download an update for the program you are patching, you may need to revert to the original file. Remember, you only need to backup the executable file for the program (i.e. the file with a .exe extension), not the entire program folder itself. Once you’ve done this, download the patching utility from here. Run it, and it will ask you to select your program. Simply select the executable file you wish to patch and the utility will work its magic. Upon completion, it will ask you if you wish to patch another file. If you do, go ahead, if not, quit!
 
## Conclusion
 
If all goes well, your application should now be able to make use of up to 4GB of RAM. Obviously this will be most useful for resource-intensive applications, and you’ll probably see the greatest benefits with games. Some productivity software will also benefit, assuming you aren’t utilising the 64-bit versions of these (e.g. Excel, Photoshop, 3D Studio Max, and so on.)
 
JJ runs a company that specialises in IT Support and cloud IT Solutions in Australia. He also moonlights as a tech blogger.
 
Our latest tutorials delivered straight to your inbox




