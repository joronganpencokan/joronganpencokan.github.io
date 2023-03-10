---
title: "Revolutionize Your Windows 11 Experience: Learn the Secret Trick to Opening Command Prompt as Admin Straight from File Explorer!"
ShowToc: true 
date: "2023-05-20"
author: "Keri Gonzales"
---
*****
Revolutionize Your Windows 11 Experience: Learn the Secret Trick to Opening Command Prompt as Admin Straight from File Explorer!

As Windows 11 becomes increasingly popular among computer users, it's important to learn helpful tips and tricks that can enhance your experience. One feature that can save you time and effort when working in Windows 11 is the ability to open Command Prompt as an administrator directly from File Explorer. This secret trick can make your workflow smoother, quicker, and more efficient.

Before we dive into how to open Command Prompt as an admin straight from File Explorer, let's quickly review what Command Prompt is and why it's important. Command Prompt is a command line interface that allows users to execute various tasks and commands through a text-based input. It is a powerful tool that grants users access to system settings and files that are otherwise inaccessible through the standard Windows interface. By opening Command Prompt as an administrator, you gain access to additional tools and commands that require elevated privileges, allowing you to make system changes that affect all users of the computer.

So, how do you open Command Prompt as an administrator straight from File Explorer? Follow these simple steps:

Step 1: Open File Explorer by clicking on its icon on the taskbar.

Step 2: Navigate to the folder where you want to open Command Prompt as an administrator.

Step 3: Hold down the Shift key on your keyboard and right-click on the folder. A context menu will appear.

Step 4: Select the "Open PowerShell window here (admin)" option from the context menu. This will open a PowerShell window as an administrator.

Step 5: In the PowerShell window, type "cmd" and press Enter. This will open Command Prompt as an administrator in the directory that you selected.

And that's it! You now have access to all the additional tools and commands that come with opening Command Prompt as an administrator. This will give you more control over your system settings and files, making your Windows 11 experience more efficient and effective.

In conclusion, knowing how to open Command Prompt as an administrator straight from File Explorer is a valuable trick that can save you time and effort when working in Windows 11. It's a simple process that can be easily mastered by following the steps outlined in this article. So, next time you need to make system changes or access files that are otherwise inaccessible, remember this secret trick and revolutionize your Windows 11 experience!

{{< youtube Ifbg1wJnz0Q >}} 



On Windows 11, when you right-click inside a folder, you will find the option to open that File Explorer path in Command Prompt, but you won’t find an entry to open the console as an administrator.
 
However, if you must open a particular folder location in File Explorer with Command Prompt as an administrator to run an application, it’s possible to add an entry to the classic context menu through the Registry.
 
In this guide, you will learn the steps to add a new entry in the File Explorer context menu to open a specific path in Command Prompt as an administrator on Windows 11 (or Windows 10).
 
## Open Command Prompt as admin from File Explorer
 
To open Command Prompt as an administrator from the File Explorer context menu on Windows 11, use these steps:
 
- Open Start on Windows 11.
 - Search for regedit and click the top result to open the app.
 - Navigate to the following path:
 - HKEY_CLASSES_ROOT\Directory\Background\shell
 - Right-click the “shell” key (folder), select New, and choose the Key option.
 - Name the key “runas” and press Enter.
 - Select the runas key.
 - Double-click the “Default” string and set its value to Command Prompt (Admin).
 - Click the OK button.
 - Right-click the “runas” key (folder), select New, and choose the String Value option.
 - Name the key NoWorkingDirectory and press Enter.
 - Right-click the “runas” key (folder), select New, and choose the String Value option.
 - Name the key HasLUAShield and press Enter.
 - Right-click the “runas” key (folder), select New, and choose the String Value option.
 - Name the key Top and press Enter.
 - Double-click the newly created key and change its value to Top.
 - Click the OK button.
 - Right-click the “runas” key (folder), select New, and choose the String Value option.
 - Name the key Icon and press Enter.
 - Double-click the newly created key and change its value to C:\\Windows\\System32\\cmd.exe.
 - Click the OK button.
 - Right-click the “runas” key (folder), select New, and choose the Key option.
 - Name the key command and press Enter.
 - Double-click the Default string and set its value to cmd.exe /s /k pushd \"%V\".
 - Click the OK button.
 - Restart the computer.

 
Once you complete the steps, use the Shift + F10 keyboard shortcut or right-click inside of a folder and choose the Show more options item to open the classic context menu to find the option to open the path in Command Prompt, but with the admin console.
 
Open Start on Windows 11.
 
Search for regedit and click the top result to open the app.
 
Navigate to the following path:
 
HKEY_CLASSES_ROOT\Directory\Background\shell
 
Right-click the “shell” key (folder), select New, and choose the Key option.
 

 
Name the key “runas” and press Enter.
 
Select the runas key.
 
Double-click the “Default” string and set its value to Command Prompt (Admin).
 
Click the OK button.
 
Right-click the “runas” key (folder), select New, and choose the String Value option.
 
Name the key NoWorkingDirectory and press Enter.
 
Name the key HasLUAShield and press Enter.
 
Name the key Top and press Enter.
 
Double-click the newly created key and change its value to Top.
 
Name the key Icon and press Enter.
 
Double-click the newly created key and change its value to C:\\Windows\\System32\\cmd.exe.
 
Right-click the “runas” key (folder), select New, and choose the Key option.
 
Name the key command and press Enter.
 
Double-click the Default string and set its value to cmd.exe /s /k pushd \"%V\".
 
Restart the computer.




