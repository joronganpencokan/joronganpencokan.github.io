---
title: "You Won't Believe How Easy it is to Streamline Your Ubuntu Startup Applications!"
ShowToc: true 
date: "2023-06-02"
author: "Tiffany Keating"
---
*****
# You Won't Believe How Easy it is to Streamline Your Ubuntu Startup Applications!

Are you tired of waiting a long time for your computer to start up? Do you wish there was an easier way to manage your Ubuntu startup applications? Well, you're in luck! With a few simple steps, you can streamline your Ubuntu startup applications and get your computer up and running faster.

Before we get into the steps, let's first understand what startup applications are. Startup applications are programs that automatically run when you start your computer. These applications can be anything from system utilities to software that you use frequently. However, having too many startup applications can slow down your computer's boot time and make it difficult to use.

Now, let's dive into the steps to streamline your Ubuntu startup applications.

Step 1: Open "Startup Applications Preferences"

The first step is to open the "Startup Applications Preferences" program. You can find this program by searching for it in the Ubuntu search bar or by opening the "System Settings" program and selecting "Startup Applications" under the "Hardware" tab.

Step 2: Disable Unnecessary Applications

Once you have opened the "Startup Applications Preferences" program, you will see a list of all the applications that are set to run when you start your computer. The next step is to disable any applications that you don't need to run at startup. To do this, simply uncheck the box next to the application's name.

Step 3: Enable Delayed Applications

For some applications that you don't want to disable completely, you can enable a delayed start time. This will allow your computer to start up faster but still allow the application to run once your computer has finished booting. Simply select the application you want to delay and click on the "Edit" button. In the "Command" field, add a "sleep X && " before the command to delay the application by X seconds.

Step 4: Prioritize Applications

If you have applications that you need to run at startup, but you don't want them to slow down your computer's boot time, you can prioritize them. This will ensure that these applications are given priority when your computer starts up. To do this, simply drag and drop the application to the top of the list.

By following these simple steps, you can streamline your Ubuntu startup applications and get your computer up and running faster. By disabling unnecessary applications, enabling delayed applications, and prioritizing important applications, you can have a faster and more efficient startup process. So, what are you waiting for? Start streamlining your Ubuntu startup applications today!

{{< youtube qHGTs1NSB1s >}} 



Your boot process may take too long to complete if a lot of services and applications load automatically whenever you turn on your computer. Thankfully, Ubuntu allows us to easily manage the startup applications and disable anything we deem unnecessary from automatically loading. Let’s see how.
 
## The Two Startups
 
The boot process of most Linux distributions is split into two separate parts.
 
The first part starts when the Linux kernel loads and lasts up until we reach the login screen. A startup service – usually systemd – loads all services necessary for basic functionality. Those might include a Bluetooth stack, the audio subsystem, etc.
 
The second part starts when you log in and consists of desktop applications, usually like Slack or Skype.
 
It’s easy to control both, but, as we’ll see, we’ll have to use different tools for each job.
 
## Systemd Startup
 
Most modern Linux distributions, including Ubuntu, rely on systemd to automatically start any needed services. Systemd comes with useful tools that can help us check this initial startup process. We can use them to see the impact of everything that loads automatically and disable anything we consider useless.
 
To check how much times systemd took to load everything, type systemd-analyze in the terminal and press Enter.
 
Systemd-analyze will check systemd’s logs and show you how much time it took for your computer’s startup sequence to finish. That’s good to know but not helpful. If your startup sequence is slow, there must be something that takes too long to load, something to blame. That’s precisely what systemd-analyze allows you to do: find who’s to blame. Try it out with:
 
This will show a list of everything systemd loaded, starting from the most impactful entry and progressively moving toward the lightest one. 
 
Tips: If you have a long list of entries, you can export the list to a text file with the command:
 
It is easier to analyze the text file than the entries in the terminal.
 
Why have a printer service running if you don’t even have a printer? If you find some services useless, you can easily disable them. Just use:
 
You should be sure they are useless, though, and that you will never need them. That’s why it’s worth checking what relies on them with:
 
## Managing Your Startup Applications
 
The second part of the startup process relies on the desktop environment itself. Depending on your distribution and desktop environment, you can use different tools to control it. On Ubuntu, you can find that tool by visiting your app menu and typing startup. Select the Startup Applications entry that will show up.
 
The Startup Applications Preferences window will appear, showing you all applications that load automatically after you log in.
 
To disable an app’s automatic loading but keep its entry in case you want to re-enable it in the future, untick the checkbox on its left.
 
To fully remove an entry, click on it to select it and then click on Remove on the right.
 
If some entries aren’t crucial for using your desktop, you can delay loading them so that the rest of the applications load faster. To do that, you must edit their entries and add an extra command before the one that launches them, manually introducing a delay. You can do this as follows:
 
The sleep 60; command will add a 60-second delay to the startup application.
 
### Adding an application to the startup list
 
This is also the spot from which you can add your own applications to the startup sequence. You can do this by clicking the Add button on the right.
 
Enter any name you wish for the startup item in the “Name” field and type your command in the aptly named “Command” field. Alternatively, you can click on the “Browse … ” button on the field’s right and select an executable file from the pop-up file dialog.
 
Finally, if you wish, enter a comment and click “Add” to add the command to the startup list.
 
Now that you have cleaned up your startup application list, you may want to have it automatically empty the trash to free up storage space or hide the top bar to free up screen real estate. 
 
OK's real life started at around 10, when he got his first computer - a Commodore 128. Since then, he's been melting keycaps by typing 24/7, trying to spread The Word Of Tech to anyone interested enough to listen. Or, rather, read.
 
Our latest tutorials delivered straight to your inbox




