---
title: "Is Your Windows 11 System Safe? Learn How To Set Automatic Restore Points Now!"
ShowToc: true 
date: "2022-11-18"
author: "Mary Gonzalis"
---
*****
Is Your Windows 11 System Safe? Learn How To Set Automatic Restore Points Now!

With the launch of Windows 11, many users are excited to experience its new features and improved performance. However, in order to ensure a smooth and secure experience, it is important to take necessary precautions and set up automatic restore points on your system.

What are restore points?

A restore point is a snapshot of your system files, settings, and programs taken at a specific point in time. In the event of a system failure or critical error, you can use a restore point to revert your system to a previous state before the issue occurred.

Why do you need restore points?

Setting up automatic restore points is crucial for maintaining the health and security of your Windows 11 system. If a virus or malware infects your system, corrupts crucial files, or causes other critical issues, you can use restore points to undo the damage and restore your system to a functioning state.

Moreover, Windows 11 updates can also cause issues and conflicts with your software or hardware. If an update leads to issues or causes your system to crash, you can use restore points to go back to a previous version of Windows 11.

How to set up automatic restore points on Windows 11?

Setting up automatic restore points is a quick and easy process on Windows 11. Here's how you can do it:

1. Open the Start menu and search for "Create a restore point."

2. Click on the "Create a restore point" option from the search results.

3. In the System Properties window, click on the "System Protection" tab.

4. Select your hard drive from the list and click on the "Configure" button.

5. In the System Protection Settings window, select the "Turn on system protection" option.

6. Adjust the maximum disk space usage for system protection as per your preference.

7. Click on the "Create" button to create a new restore point.

8. Enter a name for the restore point and click on the "Create" button.

9. Once the restore point is created, you can see it in the System Protection tab.

10. Click on the "Apply" and "OK" buttons to save the changes.

Conclusion

Automatic restore points are an important part of maintaining a secure and healthy Windows 11 system. By following the steps mentioned above, you can set up automatic restore points on your system and safeguard your data and applications. Remember to create restore points regularly to ensure maximum protection against system failures, viruses, and malware.

{{< youtube udHfkn0s4qs >}} 



The feature is available even on the latest Windows 11, but you must enable it manually. We have already shared a detailed guide on creating a restore point in Windows 11; check that guide to know how to enable the backup & restore feature.
Windows 11 automatically creates a restore point when it detects special events. However, you can force the operating system to create restore points automatically on a schedule.
Also read: How to Schedule Shutdown in Windows 11

 
## Steps to Schedule Automatic System Restore Points in Windows 11


Hence, if you are interested in scheduling automatic restore points on Windows 11, you are reading the right guide. Below, we have shared a step-by-step guide on scheduling automatic restore points on Windows 11. Let’s check out.

 
### 1) Enable the System Restore on Windows 11


Before scheduling automatic restore points in Windows 11, you first need to enable the feature. We have already shared a step-by-step guide on enabling system restore on Windows 11.
Make sure to go through that guide and set up the system restore point creation on Windows 11. Once enabled, follow the next steps.

 
### 2) Schedule Automatic Restore Points in Windows 11


To create periodic restore points on Windows 11, you must create a scheduled task via Task Scheduler. Here’s how to schedule automatic restore points in Windows 11.
1. First, click on the Windows 11 search and type Task Scheduler. Next, open the Task Scheduler app from the list of options.

2. On the right pane, right-click on the My Tasks and select Create Task option.

3. On the Create Task window, switch to the General tab. In the name field, type a name for the task, and under the Security options, select ‘Run whether user is logged on or not’ and check the ‘Run with highest privileges’ option.

4. Once done, switch to the Trigger tab and select ‘On a schedule’ on the Begin the task drop-down. On the Settings section on the left, select ‘Daily‘ and configure the scheduling settings (date, time, and frequency) on the right side. After making the changes, click on the Ok button.

5. Next, switch to the Actions tab and click on the ‘New‘ button.

6. On the Actions drop-down, select the ‘Start a program’ option. On the Program/script: field, type powershell.exe. Once done, type the following command in the ‘Add arguments (optional)’ field and click on the Ok button.
-ExecutionPolicy Bypass -Command "Checkpoint-Computer -Description \"My Daily Periodic Restore Point\" -RestorePointType \"MODIFY_SETTINGS\""

7. Now switch to the Condition tab and uncheck all options. Once done, click on the Ok button.

That’s it! This will schedule automatic restore points on your Windows 11.

 
### How to Delete the Task from the Task Scheduler?


If you don’t want Windows 11 to create restore points on a schedule, you need to delete the task you have created via Task Scheduler. For that, open Task Scheduler and select the ‘Task Scheduler Library’. Next, find the task you have created, right-click on it and select ‘Delete‘.

 
Also Read: How to Check CPU Temperature in Windows 11
So, that’s all about how to schedule automatic restore points on Windows 11. The method is quite lengthy, so follow each step carefully. If you are stuck anywhere in the steps, let us know in the comments below.





