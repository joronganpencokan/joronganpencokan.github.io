---
title: "You Won't Believe How Easy it is to Move Shared Folders to Another Drive on Windows 10 – Click to Find Out Now!"
ShowToc: true 
date: "2023-01-26"
author: "Jeramy Canfield"
---
*****
Title: You Won't Believe How Easy it is to Move Shared Folders to Another Drive on Windows 10 – Click to Find Out Now!

Introduction:

Sharing files and folders among multiple users in a network is an essential aspect of modern computing. However, when the shared folders start to take up too much space on your primary drive, you may need to move them to another location for better organization, management, and backup. In Windows 10, you can effortlessly move shared folders to another drive without compromising their accessibility or security. In this article, we'll show you how to do it step by step.

Step One: Identify the Shared Folders on Your PC

Before you can move the shared folders to another drive, you need to identify which ones you are currently sharing on your PC. To do this:

 Open File Explorer and click on the "Network" icon on the left-hand menu.

 Select "Network" from the drop-down list.

 You will see a list of all the computers and devices connected to your network.

 Double-click on the PC sharing the folders you want to move.

 You will see a list of all the shared folders on that PC.

 Write down the names of the folders you want to move.

Step Two: Create a New Folder on Another Drive

Next, you need to create a new folder on the drive where you want to move the shared folders. To do this:

 Open File Explorer.

 Navigate to the drive where you want to create the new folder.

 Right-click anywhere on the empty space and select "New Folder."

 Give the folder a name that you can easily recognize.

 Press "Enter" to save the folder.

Step Three: Stop Sharing the Folders You Want to Move

Before you move the shared folders to another drive, you need to stop sharing them on your PC. To do this:

 Open File Explorer.

 Navigate to the shared folder you want to move.

 Right-click on the folder and select "Properties."

 Click on the "Sharing" tab.

 Click on the "Advanced Sharing" button.

 Uncheck the "Share this folder" option.

 Click on "OK" and then "Apply."

 Repeat this step for each shared folder you want to move.

Step Four: Move the Shared Folders to the New Location

Now you are ready to move the shared folders to the new location on another drive. To do this:

 Open File Explorer.

 Navigate to the shared folder you want to move.

 Right-click on the folder and select "Cut."

 Navigate to the new folder you created on another drive.

 Right-click on the folder and select "Paste."

 Repeat this step for each shared folder you want to move.

Step Five: Share the Folders Again

Once you have moved the shared folders to the new location, you need to share them again on your PC. To do this:

 Open File Explorer.

 Navigate to the new location of the shared folder.

 Right-click on the folder and select "Properties."

 Click on the "Sharing" tab.

 Click on the "Advanced Sharing" button.

 Check the "Share this folder" option.

 Click on "OK" and then "Apply."

 Repeat this step for each shared folder you want to move.

Conclusion:

Moving shared folders to another drive on Windows 10 is a simple and quick process that will help you free up space on your primary drive and better manage your files and data. By following the steps outlined above, you can easily move your shared folders to a new location without disrupting their accessibility, security, or functionality. Give it a try today, and you will be amazed at how easy it is!

{{< youtube iGoTHB--bzc >}} 



On Windows 10 (or Windows 11), if the computer is acting as a file sharing server, the time might come when you may need to move a folder share to a new drive. For example, because the old storage is running out of space, you are upgrading the storage, or it makes logical sense to migrate the data to another drive.
 
Whatever the reason it might be, Windows 10 does not include a tool to make the process easy, but it’s not impossible. If you need to move a shared folder to another drive preserving permissions and without reconfiguration in the clients, you can complete this task by copying the contents to the new drive and either modifying the Registry or changing drive letters, depending on the setup.
 
In this guide, you will learn the steps to move a folder share to a new drive in the same computer or server without network users noticing the change or reconfiguring the share on Windows 10. This should also work on Windows 11, Windows Server 2019, 2016, and 2012.
 
- Move shared folder to new drive modifying Registry on Windows 10
 - Move shared folder to new drive changing drive letter on Windows 10

 
## Move shared folder to new drive modifying Registry on Windows 10
 
Before proceeding, make sure that no one is accessing the files in the shared folder. Also, you will be modifying the Registry. As a result, it’s recommended to make a backup of the system before making changes if you need to roll back.
 
To move a shared folder to a new drive in the same computer, use these steps:
 
- Open Start on Windows 10.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to copy the shared folder content to the new drive on the same computer and press Enter:
 - robocopy C:\SOURCE-SHARE D:\DESTINATION-SAHRE /R:5 /W:2 /Copyall /E /MIR
 - In the command, make sure to update the source and destination paths with the locations that apply to your setup.
 - For example, this command copies the data from “MyShare” folder in the “C” drive to the “MyShare” folder in the “D” drive on the same server.
 - robocopy C:\MyShare D:\MyShare /R:5 /W:2 /Copyall /E /MIR
 - Open Start.
 - Search for Registry and click the top result to open the app.
 - Browse the following path:
 - HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\LanmanServer\Shares
 - Right-click the “String” with the shared folder name to move to a new drive and select the Modify option. For example, MyShare.
 - In the “Path” field, change the drive letter with the letter to the new destination. For example, change C for D if the data has been moved to the “D” drive.
 - Click the OK button.
 - Restart the computer.

 
Once you complete the steps, network users should be able to access the files in the shared folder from the new location.
 
Open Start on Windows 10.
 
Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 
Type the following command to copy the shared folder content to the new drive on the same computer and press Enter:
 
robocopy C:\SOURCE-SHARE D:\DESTINATION-SAHRE /R:5 /W:2 /Copyall /E /MIR
 
In the command, make sure to update the source and destination paths with the locations that apply to your setup.
 
For example, this command copies the data from “MyShare” folder in the “C” drive to the “MyShare” folder in the “D” drive on the same server.
 
robocopy C:\MyShare D:\MyShare /R:5 /W:2 /Copyall /E /MIR
 

 
Open Start.
 
Search for Registry and click the top result to open the app.
 
Browse the following path:
 
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\LanmanServer\Shares
 
Right-click the “String” with the shared folder name to move to a new drive and select the Modify option. For example, MyShare.
 
In the “Path” field, change the drive letter with the letter to the new destination. For example, change C for D if the data has been moved to the “D” drive.
 
Click the OK button.
 
Restart the computer.
 
Here’s a breakdown of the Robocopy options:
 
- /R:5 — Retries 5 times (you can specify a different number, the default is 1 million).
 - /W:2 — Waits 2 seconds before retrying (you can specify a different number, the default is 30 seconds).
 - /Copyall — Copies all file information (equivalent to /copy:DATSOU).
 - /E — Copies Subdirectories, including empty ones.
 - /MIR — Mirrors a directory tree (equivalent to /e plus /purge). Using this option with the /e option and a destination directory overwrites the destination directory security settings.

 
This is an example of the command you can use to move the data with their permissions to the drive. However, depending on your environment, you may need to use different options. For example, you can use the “/MT:n” switch to perform multi-threaded copies with n threads (default is 8).
 
## Move shared folder to new drive changing drive letter on Windows 10
 
If the data resides on a drive other than the “C” drive, you do not need to modify the Registry. You can use Robocopy to copy the files to the new drive and then change the letter of the new driver to the previous letter, assuming that you don’t have an application or another share that will be affected by this change.
 
To move a folder share to a new drive by changing the drive letter instead of modifying the Registry, use these steps:
 
- Open Start.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to copy the shared folder content to the new drive on the same computer and press Enter:
 - robocopy C:\SOURCE-SHARE D:\DESTINATION-SAHRE /R:5 /W:2 /Copyall /E /MIR
 - In the command, make sure to update the source and destination paths with the locations that apply to your setup.
 - For example, this command copies the data from “MyShare” folder in the F drive to the “MyShare” folder in the D drive on the same server.
 - robocopy F:\MyShare D:\MyShare /R:5 /W:2 /Copyall /E /MIR
 - Open Start.
 - Search for Disk Management and click the Create and format hard disk partitions to open the app.
 - Right-click the source drive and select the Change Drive Letter and Paths option.
 - Click the Change button.
 - Check the Assign the following drive letter option.
 - Select another drive letter to free up the current letter.
 - Click the OK button.
 - Click the Yes button to confirm.
 - Right-click the destination drive and select the Change Drive Letter and Paths option.
 - Click the Change button.
 - Check the Assign the following drive letter option.
 - Select the drive letter that was using the source drive.
 - Click the OK button.
 - Click the Yes button to confirm.

 
After you complete the steps, the shared folder will become available from the new location, but users won’t notice the difference since you also change the drive letter.
 
For example, this command copies the data from “MyShare” folder in the F drive to the “MyShare” folder in the D drive on the same server.
 
robocopy F:\MyShare D:\MyShare /R:5 /W:2 /Copyall /E /MIR
 
Search for Disk Management and click the Create and format hard disk partitions to open the app.
 
Right-click the source drive and select the Change Drive Letter and Paths option.
 
Click the Change button.
 
Check the Assign the following drive letter option.
 
Select another drive letter to free up the current letter.
 
Click the Yes button to confirm.
 
Right-click the destination drive and select the Change Drive Letter and Paths option.
 
Select the drive letter that was using the source drive.
 
Only after you have confirmed that everything is working correctly, you can proceed to delete the old shared folder to free up space (as needed).




