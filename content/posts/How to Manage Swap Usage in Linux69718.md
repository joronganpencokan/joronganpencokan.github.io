---
title: "Unlock the Secret to Boosting Linux Performance with This Simple Swap Usage Hack!"
ShowToc: true 
date: "2023-01-06"
author: "Ralph Phelps"
---
*****
Title: Unlock the Secret to Boosting Linux Performance with This Simple Swap Usage Hack!

Introduction:
Linux is a powerful operating system that has gained popularity among developers, system administrators, and IT professionals. It offers a robust and flexible environment for running applications and managing resources. However, if you use Linux, you may have experienced slow performance at some point, especially when running resource-intensive applications or multitasking.

Fortunately, there is a simple hack that can significantly improve performance on Linux. This hack involves optimizing the use of swap space, which is a portion of the hard drive that the system uses as virtual memory when the physical RAM is full.

In this article, we will explore the swap usage hack and show you how to use it to boost performance on Linux.

Body:
The default configuration of many Linux distributions allocates a small amount of swap space, typically equal to the size of the RAM. This setup works well for most applications, but it may not be sufficient for large or memory-intensive programs.

To optimize the use of swap space, you need to do two things: increase the amount of swap space and adjust the swappiness value.

Increasing Swap Space:
To increase the amount of swap space, you need to create a new swap partition or file. A swap partition is a dedicated section of a hard drive that the system uses exclusively for virtual memory. A swap file is a file that the system uses as virtual memory.

To create a swap partition, follow these steps:

1. Open the terminal and enter the command `sudo fdisk -l` to list the available disks and partitions.
2. Identify the partition that you want to use for swap. It should be a primary or logical partition that is not currently in use.
3. Enter the command `sudo mkswap /dev/partition-name` to create a swap area on the partition. Replace partition-name with the name of the partition that you identified in step 2.
4. Enter the command `sudo swapon /dev/partition-name` to activate the swap area.

To create a swap file, follow these steps:

1. Open the terminal and navigate to the directory where you want to create the swap file.
2. Enter the command `sudo fallocate -l size /swapfile` to create a swap file. Replace size with the size of the file in bytes (e.g., 1G for a 1 gigabyte file).
3. Enter the command `sudo chmod 600 /swapfile` to set the file permissions.
4. Enter the command `sudo mkswap /swapfile` to format the file as a swap area.
5. Enter the command `sudo swapon /swapfile` to activate the swap area.

Adjusting Swappiness:
The swappiness value is a kernel parameter that controls the tendency of the system to use swap space. A low swappiness value means that the system will try to avoid swapping as much as possible, whereas a high value means that the system will swap aggressively.

To adjust the swappiness value, follow these steps:

1. Open the terminal and enter the command `sysctl vm.swappiness` to show the current value.
2. Decide on a new value based on your system's memory usage and workload. A value of 10-20 is recommended for desktops and laptops with sufficient RAM, whereas a value of 60-100 may be more appropriate for servers or systems with limited RAM.
3. Enter the command `sudo sysctl vm.swappiness=value` to set the new value, replacing value with the desired swappiness value.

Conclusion:
Optimizing the use of swap space is a simple and effective way to boost performance on Linux. By increasing the amount of swap space and adjusting the swappiness value, you can ensure that your system has enough virtual memory to handle any workload. With this swap usage hack, you can unleash the full potential of Linux and take your computing experience to the next level.

{{< youtube CyVOL1IYKNA >}} 



You may have experienced system lags, heavy swap usage, or low memory issues in your Linux system. A usual advice is to “decrease the swappiness value”, reduce the swap usage. but what is swappiness? And is it really good to tweak it?
 
Note: we won’t go into detail about the swap partition. You can read all about it in our article on what you need to know about Swap partition on Linux.
 
## Swappiness
 
There is a value called swappiness in UNIX-like systems that determines how pages in memory will be handled. Its default value on most systems is “60,” but it can be set to anything between 0 and 100. If memory runs low, the kernel will either evict some file caches to have more free RAM for processes, or it will swap some process pages from RAM to disk.
 
A default of 60 means swapping will be used less, and I/O caches will more likely be freed for reallocating RAM. Evicting caches is considered “cheaper” (less resource intensive), while swapping out pages includes disk reads and writes, making them more “expensive.” At a value of ’60,’ swap usage will be slightly lower than cache reuse. If the value of swappiness is increased to 100, swapping and file cache eviction will be used with equal weight. This means more swapping and faster I/O than default. Lower values like “10” mean that swapping will be used much less, and I/O caches can be much sooner evicted in favor of processes. This might increase interactivity but could also hurt I/O speed.
 
## Decreasing swappiness
 
You will often see the advice on websites and forums to reduce swappiness to around “10.” This is supposed to speed things up by using less swap and keeping more processes in physical RAM. This logic might be somewhat too straightforward and might not be a “one size fits all solution.”
 
Decreasing the value of swappiness might be good in the following scenarios:
 
- For databases systems, or if you use a lot of database intensive applications: Databases generally handle file caching way better than the OS would. If you reduce swappiness, you will limit the OS’s file caching, thus giving a chance to the database to handle its own caches.
 - For interactivity: If you multitask a lot but handle few files or don’t open large documents, this could improve how smooth your system will feel. Less processes will be written out to disk, and as RAM access is much faster, your computer can feel faster. You must also bear in mind that this can reduce I/O performance. If you have slow disks or do anything I/O intensive, it might even hurt performance.
 - For placebo: Many believe that a lower swappiness will speed up the system,. Seriously, f you think that your system is faster, it might have the effect of perceiving it to be faster, too.

 
Keep in mind that decreasing swappiness might result in crashes and processes being randomly killed by the system in order to free up memory. Decreasing swappiness will be best if you have enough RAM available to run your system smoothly. But you should keep the value above “10”, as some swap use is good to have.
 
## Increasing swappiness
 
Increasing swappiness can have the general advantage of speeding up I/O. Although not often advised, increasing swappiness might come in handy if:
 
- You perform some I/O intensive operations, and you have slow, old HDDs. For example: performing backups or batch editing images can be I/O intensive (A notable exception is databases which are naturally I/O intensive but could benefit from a lower swappiness value as seen above.).
 - You have low memory but have relatively fast disks. In this unlikely scenario, a higher value of swappiness might help to handle memory more efficiently (although setting it too high might again hurt performance.).

 
## How to manage swappiness
 
First, you should consider if you need to touch this value at all. Are you experiencing performance issues? And more importantly, have you tried other system tweaks yet? If not, it is probably best to look elsewhere first. But if you have a specific scenario in mind, you might want to continue.
 
Next, how heavy is your swap usage? You can find it out with any performance monitoring tool of your choice or with the free command. free -m will give you a snapshot of the memory usage in megabytes. For continuous monitoring, you might want to use watch.
 
This will run the free -m command every second and print its output until you press “Ctrl + C.”
 

 
As you see above, very little swap is being used by the system this article is written on.
 
Now if you do experience swapping, you might be interested how much of it is active. The command vmstat will tell you all you need to know about your system’s virtual memory usage (swap and physical ram together).
 
You need to check the swap column where si means “swap in”, and so means “swap out.” If the numbers are high, it means a lot of swapping activity which is an indicator of low memory issues. If you see swap usage by free but little active swapping, tweaking swappiness might be due.
 
It is also a good idea to establish other performance benchmarks like disk I/O, load averages, etc., so when you test your new swappiness values, you have something to compare against.
 
To test a different swappiness value, you can set it temporarily with the sysctl command. This needs no rebooting, and the effect is immediate. In fact, rebooting will restore the default value, so you are quite safe to experiment:
 
Of course, you can put any value instead of “10” (between “0” and “100”).
 
Once you’ve found your preferred value, you can permanently change the system configuration by editing “/etc/sysctl.conf”
 
and adding the lines
 
to the end of this file, with the value set to your preference once again, of course.
 
## Conclusion
 
Lowering swappiness to “10” is often advised as a one-size-fits-all solution, but the actual use of the technique might be a tiny bit more complicated than that. By establishing benchmarks, knowing your system, how you use it, and what you need from it, you can fine tune your swap usage and achieve some performance (either interactivity or I/O) increase.
 
Attila is a writer, blogger and author with a background in IT management. Using GNU/Linux systems both personally and professionally, his advice stems from 10+ years of hands on experience. In his free time he also runs the popular Meditation for Beginners blog.
 
Our latest tutorials delivered straight to your inbox




