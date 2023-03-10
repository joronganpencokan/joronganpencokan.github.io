---
title: "Discover the Mind-Blowing Shortcut to Copy Any Folder's File List in Windows!"
ShowToc: true 
date: "2023-01-27"
author: "Paul Eden"
---
*****
Introduction:

Copying and pasting files in Windows is a common task that every user performs frequently. However, there are situations where you need a quick solution to copy a folder's file list without manually selecting files one by one. In this article, we will describe a mind-blowing shortcut to copy any folder's file list in Windows, using a simple trick that could save you valuable time.

Step-by-Step Guide: 

Step 1: Open Command Prompt 

To use the shortcut, you need to open Command Prompt, which is a built-in tool in Windows. You can launch it by pressing the Windows + R key, typing "cmd," and pressing Enter.

Step 2: Navigate to the Folder 

In Command Prompt, you need to navigate to the folder whose file list you want to copy. You can do this by typing the folder's path, followed by the command "cd," for example: 

cd C:\Users\User1\Documents\TestFolder

Step 3: Generate the File List 

Now, you need to run a simple command that will generate a text file containing the list of all files in the folder. The command is as follows: 

dir /b > fileList.txt

This will create a text file named "fileList.txt" containing the list of all files in the folder. You can save this file in any directory you want.

Step 4: Copy the File List 

Finally, you can open the "fileList.txt" file and copy its contents to the clipboard. To do so, right-click the file, select "Edit," and press Ctrl + A to select all text. Then, press Ctrl + C to copy the text to the clipboard.

Conclusion: 

This shortcut is a quick solution to copy any folder's file list in Windows. You can use this trick to create a list of files in any folder, making it easier to organize and manage your files. By using Command Prompt, you can save valuable time and avoid the hassle of manually selecting files one by one. So, try out this mind-blowing shortcut the next time you need to copy a folder's file list in Windows!


It may not be that often, but you may sometimes need to get the list of files in a folder. There may be several reasons such as to create a list of file names, copy all the file names, export a list of file names to excel, etc. No matter what the reason is, Windows has no default option to create a list of all the filenames in a folder. However, listing file names in a folder is not that hard in Windows. Here is how to create or copy a folder’s file list in Windows.
 
## Create a List of File Names in a Folder
 
The first and easiest way to create a list of file names in a folder is to use the command prompt. We can just use the DIR command to export a list of file names to a text document.
 
To start, navigate to the folder with the files you want to create a list. Now, “Shift + right-click” in the folder, and then select the option “Open command prompt here.”
 

 
The above action will open the Command Prompt in the current folder. Now, copy and execute the below command:
 
As soon as you execute the command, a new text file will be created in the current folder with the list of files in the folder. The good thing about the above command is that it will only list files and ignores any directories or folders.
 
If you want the command to list directories or folders, use the below command:
 
As you can see from the above command, we just modified the previous command and removed the -d attribute to include folders in the list. In case you are wondering, the /o:n switch ensures that the list is automatically sorted by names.
 
## Add Copy File List Option to Right-Click Context Menu
 
If you need to create file lists often, then the above method may not be that user-friendly. To make things easier, you can add a context menu option which copies the file list. You can, in turn, paste the list wherever you want.
 
To start, search for “regedit” in the Start menu and open it.
 
The above action will open the Windows Registry Editor. Here, navigate to the following location:
 
Right-click on the “Shell” key, and select the option “New -> Key.”
 
Name the new key “copylist,” and press the Enter button.
 
By default, all the new keys will have a String Value called “(Default)” with no value data. To change the value data, double-click on the value, enter the Value Data as “Copy file list,” and click on the “OK” button. This value is what you will see in the right-click context menu. Feel free to customize the text if needed.
 
Now, right-click on the “copylist” key, select “New” and then “Key.”
 
Enter “command” as the name of the key.
 
Again, the new key will have its own default value. To edit the value data, double-click on the Default value to open the “Edit Value Data” window. Here, enter cmd /c dir "%1" /b /a:-d /o:n | clip, and click on the “OK” button to save the changes.
 
Note: if you also want to list folders along with files in a folder, then replace /a:-d with /a.
 
From this point forward, you can copy the file list by simply right-clicking on the folder that contains all your files and then selecting the option “Copy file list.” Once copied, you can paste the list whereever you want, like in a Notepad or Excel sheet.
 
Do comment below sharing your thoughts and experiences about using the above method to create or copy the list of files in a folder.
 
Vamsi is a tech and WordPress geek who enjoys writing how-to guides and messing with his computer and software in general. When not writing for MTE, he writes for he shares tips, tricks, and lifehacks on his own blog Stugon.
 
Our latest tutorials delivered straight to your inbox




