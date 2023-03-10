---
title: "You won't believe how easy it is to keep your Linux processes a secret from prying eyes!"
ShowToc: true 
date: "2023-06-24"
author: "Andrea Rush"
---
*****
You won't believe how easy it is to keep your Linux processes a secret from prying eyes!

If you are using Linux, you might think that your processes are secure and invisible to the outside world. However, this is not always the case. There are many ways in which prying eyes can discover and monitor your processes. In this article, we will show you how to keep your Linux processes a secret from prying eyes.

The first thing you need to know is that there are many tools available that can detect and monitor Linux processes. These tools can be used by system administrators to troubleshoot their systems, and they can also be used by hackers to spy on your system. To keep your processes a secret, you need to first understand how these tools work.

One of the most commonly used tools for monitoring Linux processes is the ps command. This command is used to list all running processes on a Linux system. If you run the ps command from the terminal, you will see a list of all processes running on your system, as well as their IDs, memory usage, and CPU time.

To keep your processes a secret from prying eyes, you can use the hidepid feature of the /proc filesystem. This feature allows you to hide the process IDs of your system processes from non-privileged users. To use this feature, you need to modify the /etc/fstab file and add the hidepid option to the mount options for the /proc filesystem.

Once you have added the hidepid option to the /proc mount options, save the file and then remount the /proc filesystem by running the following command:

mount -o remount /proc

After remounting the /proc filesystem, you can test whether the hidepid option is working by running the ps command with the -ef option. This will show all running processes on your system, including their process IDs. If the hidepid option is working correctly, you should not see any process IDs.

Another tool that can be used to monitor Linux processes is the top command. This command is used to display real-time information about running processes on a Linux system. To keep your processes a secret from prying eyes, you can use the nice and ionice commands to change the priority of your processes.

The nice command is used to change the priority of a process. By default, all processes are given a priority of 0, which means that they have the same priority as other system processes. You can use the nice command to increase or decrease the priority of your processes. For example, if you want to run a process with a lower priority, you can use the following command:

nice -n 10 command

This will run the command with a priority of 10, which means that it will have a lower priority than other processes on your system.

The ionice command is used to change the I/O priority of a process. By default, all processes are given a priority of 0, which means that they have the same I/O priority as other system processes. You can use the ionice command to increase or decrease the I/O priority of your processes. For example, if you want to run a process with a lower I/O priority, you can use the following command:

ionice -c3 command

This will run the command with a priority of 3, which means that it will have a lower I/O priority than other processes on your system.

In conclusion, keeping your Linux processes a secret from prying eyes is easy if you know the right tools and techniques. By using the hidepid feature of the /proc filesystem and the nice and ionice commands, you can make your processes invisible and give them lower priorities than other system processes. With these techniques, you can ensure that your Linux system is secure and protected from prying eyes.

{{< youtube _FlV6pgwlrk >}} 



All modern multi-tasking operating systems, including Linux, run a series of processes for each of the tasks being executed. A notepad application is a process, a terminal window is a process, the SSH server is a process, each SSH connection is a process and so on. Linux schedules the various system resources (CPU time, memory, I/O) so that each process get an opportunity to run.
 
To see the list of current processes running, you can use the ps command. Try this in a terminal:
 
The aux parameters tell ps to list all the system processes with extra information about who owns the processes and what calling parameters were used.
 

 
As you can see, the list shows processes owned by different users including “pi” (the default Raspbian user on a Raspberry Pi), “root” and “www-data”. Here is a slightly modified screenshot which shows the processes along with fuller details about the commands and their parameters.
 
If you look down the list, you will see the command nano MYBANKACCOUNTNUMBER.TXT which is owned by the user “john.” Imagine if the file name was a little more revealing than the example; such data is exposed to all users on the system and could be used for malicious purposes.
 
Since Linux kernel 3.2 there is a way to stop users getting access to information about processes which they don’t own. The ps command gets the process information from the /proc filesystem (where “proc” is short for process). There is a new parameter called “hidepid” which is used when the /proc filesystem is mounted. It can hide processes and controls who has access to the information under /proc.
 
- hidepid=0 – The default behavior where any user can read the files under /proc/PID/
 - hidepid=1 – It means users may not access any /proc/PID/ sub-directory except their own. Also files like cmdline, io, sched*, status, wchan are inaccessible to other users.
 - hidepid=2 – Everything from hidepid=1, plus all /proc/PID/ sub-directories will be hidden to other users.

 
The /proc filesystem can be remounted on the fly using the remount option of the mount command. To test hidepid, you can remount the /proc filesystem like this:
 
Now you can try the ps command again:
 
Now the output only shows processes that are owned by the user “pi”.
 
To make this change permanent, you need to edit your Pi’s “/etc/fstab” file. The “fstab” file controls which file systems are mounted at start up.
 
And find the line which reads:
 
And change it to:
 
Exit the editor using “Ctrl + X.” Now reboot your Raspberry Pi. When it reboots, check that the /proc filesystem has been mounted with the right options. First use mount and grep to see the current options:
 
Now test the ps command, exactly as we have done above:
 
Notice now that only the processes owned by “pi” are visible, but unlike before when we remounted the /proc file system, this is now the permanent setting. However one word of warning, even when hidepid is used, “root” can still see all the processes and the calling parameters.
 
The technique used above will work on other Linux machines and distributions, not just the Raspberry Pi with Raspbian. If you have questions about using the “hidepid” option on the /proc file system, please feel free to use the comments section below, and we will see if we can help.
 
Gary has been a technical writer, author and blogger since 2003. He is an expert in open source systems (including Linux), system administration, system security and networking protocols. He also knows several programming languages, as he was previously a software engineer for 10 years. He has a Bachelor of Science in business information systems from a UK University.
 
Our latest tutorials delivered straight to your inbox




