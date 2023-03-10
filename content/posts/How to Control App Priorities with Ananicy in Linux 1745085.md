---
title: "Why Successful Linux Users Swear By Ananicy for Gamers and Workflow Efficiency - Here's How You Can Master It too!"
ShowToc: true 
date: "2022-12-17"
author: "Sue Rapp"
---
*****
Why Successful Linux Users Swear By Ananicy for Gamers and Workflow Efficiency - Here's How You Can Master It too!

Are you a Linux user who loves gaming or seeks maximum workflow efficiency? If your answer is yes, then you can't miss out on Ananicy, the full-fledged open-source system daemon that helps you achieve a smoother and snappier Linux experience.

Ananicy is built on the theory that System resources should be distributed dynamically and prioritized based on the user's requirements. Thus, Ananicy aims to keep CPU clock speeds up, the memory unburdened, and render gaming GPU's free from any background servitude.

There are a plethora of reasons why Ananicy could elevate your Linux experience to new heights. In this article, we will explore all aspects of Ananicy and gain insight into how some of the most successful Linux users swear by it.

Here's what you need to know about Ananicy :

1.	ANANICY CONTRIBUTES TO AN OPTIMIZED LINUX GAMING EXPERIENCE

Playing games on Linux may have a steep learning curve, but Ananicy makes it seamless. The game may moderately use your system's resources, and compared to the background services, Ananicy refers to as "non-renounceable" tasks will be given priority.

For instance, if your game requires a stable CPU clock speed and doesn't need much memory or IO throughput, then Ananicy will allocate CPU resources to that game, and other system tasks will be deprioritized to ensure the smooth running of the game. This feature ensures a glitch-free gaming experience and could potentially give gamers a competitive edge by reducing input lag.

2.	ANANICY ENSURES MAXIMUM WORKFLOW EFFICIENCY

Productivity is one of the core features that Ananicy promises. Background processes like package managers, daemons, and other non-essential tasks can distract users and eat up precious system resources.

Ananicy users can prioritize apps based on their usage. That means that the active applications will receive priority and can run at optimum speed without any hindrance from background services. This fast performance will significantly reduce any lag time, increase efficiency, and productivity.

3.	ANANICY IS HIGHLY CONFIGURABLE AND FLEXIBLE

Ananicy is highly configurable and allows granular control of system processes. Users can tailor the Ananicy setting to cater to their unique system requirements.

The configuration file is user-friendly and easier to comprehend than other similar applications. Additionally, Ananicy's ease of use is unparalleled by the range of customization options it provides.

4.	ANANICY HAS PROVEN ITS WORTH TO SOME OF THE MOST SUCCESSFUL LINUX USERS

Ananicy has proven to be highly effective to some Linux users who swear it drastically improved their system's performance. Professional gamers who prefer playing on Linux have testified that Ananicy has provided them with a glitch-free gaming experience and a considerable performance boost.

5. INSTALLING AND CONFIGURING ANANICY

Installing and configuring Ananicy is quite easy. If you have Ubuntu or Debian, the chances are that you won't even need to install via PPAs or repositories. A quick search on the respective platform's terminal will reveal whether Ananicy is already installed or not.

Once installed, users can configure Ananicy by setting priorities for individual applications using the Ananicy config file.

Conclusion

Linux users may have had difficulty with suboptimal experiences while gaming, which could seriously dent their productivity. However, Ananicy, with its optimization capabilities, could provide users with a solution. The dynamic configuration that Ananicy provides and prioritizes helps to ensure smooth gaming and maximum workflow efficiency.

Ananicy has significantly increased the efficiencies of some of the most successful Linux users, and you too could be a happy Ananicy user!

Go ahead and install Ananicy today, optimize your system, and experience the best Linux gaming, and maximum workflow efficiency.


Auto Nice Daemon is ancient, and changing your software priorities manually is annoying. Isn’t there a modern way to control how many resources each program should use? Meet Ananicy (ANother Auto NICe daemon), a modern auto-nice solution, with which you can create profiles for your software to prioritize the apps you care about. Let’s see how you can do that.
 
## Installation
 
Ananicy needs systemd to work, so it isn’t compatible with every distribution under the sun. To install it on Ubuntu, Mint, Debian, and compatible distributions, use:
 
If you are on Arch, Manjaro, or another similar distribution, you can install it with:
 
Ananicy also relies on schedtool, so if it’s not already installed, make sure to add this, too. You can do that on Debian-compatible and Arch-compatible distributions, respectively, with:
 
With everything set up, enable its daemon to have it always active and monitoring your applications:
 
To start the actual application, use:
 
If you are on a low-powered system, where every piece of software is fighting for resources, it may start feeling somewhat more responsive right away.
 
## Check the Presets
 
Ananicy comes pre-bundled with a bunch of rules for many popular applications. To check them out, fire up your favorite terminal and pay a visit to Ananicy’s rules directory:
 
The rules for each application are stored in separate files. For example, to check out the preset rules for the popular qBittorrent filesharing client, you could use:
 
You can use those as a base for your own rules.
 
## Add your own rules
 
To create rules for an application, you should know its process name. Thankfully, on Linux, that’s usually the same as the application’s name. You can use the top command to verify the process name.
 
Locate a process that is hogging your computer and note down its name. Let’s use the timeshift app as our example.
 
Create a new text file in Ananicy’s rules directory. It’s better if you use the application’s name for easier future reference. Make sure to have your file end with “.rules” for Ananicy to recognize it as a rules file.
 
The easiest way to create a rule for a piece of software is by only stating its name and classifying its type. Ananicy comes with predefined types for games, multimedia apps, document editors, etc. To check them out, use the command:
 
Each of those comes with different nice, ionice, cgroup, and other values, but it’s suggested you don’t go further than tweaking an application’s nice value. However, for applications that read and write a lot to your storage, it’s also worth defining their input-output priority using the ioclass parameter.
 
With all that in mind, we are ready to craft our own custom rule:
 
The above rule:
 
- States the application’s nameDefines its typeAssigns it a different nice priority compared to the presetsSets its input/output priority as idle

 
Theoretically, you only have to state an application’s name, and everything else is optional. Practically, if you do only that, Ananicy will only acknowledge the app’s existence but not try to control it. For that, you will have to define its type at least.
 
Its type comes with different predefined nice and input/output values, and you’ll probably find one that matches how you want to restrict a piece of software. Sometimes, though, like in our case with timeshift, you may want to tweak them further. That’s when you will have to explicitly state the nice or ioclass value you want if it’s different than the one included in Ananicy’s type preset.
 
The BG_CPUIO preset we selected matches our application’s type since, as a backup solution, it usually runs in the background but can eat up a lot of processing cycles while performing continuous reads and writes. However, the BG_CPUIO preset would assign it the lowest possible nice and ionice values, which could make a backup process take ages. Because of this, we increased the nice value to 17 and the ioclass to best-effort, to somewhat speed up the process.
 
Let’s take a look at another example. Batman: Arkham City’s “Joker’s Carnival” DLC is one of my favorite pieces of gaming. Its action relies on fluid motion, though, and I could feel it stuttering in Linux Mint whenever another piece of software is running in the background. Thus, for this one, I wanted to do the opposite – increase its priority over everything else.
 
By checking Linux Mint’s System Monitor after running the game through Steam with Proton, we can see its process name as “BatmanAC.exe.” To give it a nice boost with Ananicy, I created a new rule called “BatmanAC_ody.rules” like before. However, in this case, its contents were:
 
That was enough since the “Game” type comes with a “-5” nice value, prioritizing an app over everything else. Thus, you don’t have to explicitly state the nice value yourself or craft more complicated rules.
 
One restart later, for good measure, and Ananicy will be active, ready to spring into action to tweak your software’s priorities. The value you see for the BatmanAC.exe process in the screenshot below was assigned automatically, without needing any user intervention.
 
Note that you don’t have to do this for all your software, but pulling the reins on the most demanding background processes and boosting the more interactive ones can make a world of difference to how using your computer feels. It can minimize stuttering and provide a smoother experience all around.
 
Are you already using Ananicy or another similar solution that allows you to control how your computer’s resources are assigned to your apps? Are you manually renicing your software? Tell us in the comments section below.
 
OK's real life started at around 10, when he got his first computer - a Commodore 128. Since then, he's been melting keycaps by typing 24/7, trying to spread The Word Of Tech to anyone interested enough to listen. Or, rather, read.
 
Our latest tutorials delivered straight to your inbox




