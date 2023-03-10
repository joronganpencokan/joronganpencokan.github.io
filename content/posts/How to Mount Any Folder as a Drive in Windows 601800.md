---
title: "You Won't Believe How Easy it is to Mount Any Folder as a Drive in Windows - Say Goodbye to Disk Woes!"
ShowToc: true 
date: "2023-04-29"
author: "Larry Sanchez"
---
*****
Title: You Won't Believe How Easy it is to Mount Any Folder as a Drive in Windows - Say Goodbye to Disk Woes!

Are you tired of cluttered and scattered files all over your computer? Are you looking for an easy solution to organize your files and folders? Look no further because mounting folders as drives in Windows is here to the rescue!

Gone are the days of searching through multiple folders for a single file. By mounting your folders as drives, you can have a more organized and streamlined approach to file management.

Here is a step-by-step guide to mount any folder as a drive in Windows:

Step 1: Open Disk Management

To get started, open the Disk Management tool by pressing the Windows key + X and selecting Disk Management from the list.

Step 2: Select the Folder to Mount

Next, right-click on the folder you wish to mount and select the option to "Change Drive Letter and Paths."

Step 3: Mount the Folder as a Drive

From there, click the "Add" button and select the option to "Mount in the Following Empty NTFS Folder." Choose a drive letter and then click "OK."

Step 4: Access Your New Drive

Congratulations! You have successfully mounted your folder as a new drive. You can now access this drive from "This PC" and use it like any other drive to save, retrieve or transfer files.

By mounting folders as drives, you have more flexibility and control over your files, allowing you to access them quickly and more efficiently, which in turn can help to save time and resources.

Moreover, it is worth noting that this feature can be immensely helpful in cases when your hard disk space is running low, and you do not wish to move files to other drives due to storage limitations. Mounting folders as drives allows you to use the space on the drive that the folder is mounted on as if it was a part of your primary drive.

In conclusion, mounting folders as drives is an easy and efficient method to manage files in Windows, one that undoubtedly will help you save time and minimize the stress associated with managing your files. So, if you haven't tried it yet, go ahead, and give it a try! You won't believe how much easier your life can become with this simple feature.

{{< youtube GkdFeil3NLI >}} 



Even if you are a casual user, I am sure you have tons of folders in your computer that can make it difficult to find the files you want sometimes. The Windows Explorer application in Windows doesn’t make it any easier for you to locate your files. Wouldn’t it be great if you could mount your frequently accessed folder as a virtual drive (such as E:\, F:\ etc.) in Windows so they could appear in the “Computer” list and you could easily access your folder with a single click?
 
Visual Subst is a small tool that allows you to link your favorite folders to virtual drives. It is only 78kb in size and doesn’t require any installation.
 
## Mounting a folder as a virtual drive with Visual Subst
 
1. Download the zipped file from the Visual Subst website. It is only 78kb in size.
 
2. Extract the archive and double click the “VSubst” application to run it. 
 

 
3. In the window that opens, first click the dropdown field to select the Drive letter you want to assign for the folder. In this case, I selected “S:”.
 
4. Next, click the “magnifying glass” icon to locate the folder you want to mount as a drive. In this case, I selected my Dropbox folder. 
 
Optionally, you can check the box beside “Apply virtual drives on Windows startup” if you want this folder to be accessible right from the start.
 
Lastly, click the green “+” icon. This will create the virtual drive. Now open your Windows Explorer and you should see the newly created drive in the Computer list. 
 
To delete it, simply select the entry and click the “x” icon. 
 
## Manually creating the virtual drive
 
If you don’t want to rely on third-party software, here is another way you can do it.
 
1. Open Windows Explorer and navigate to the Startup folder by pasting this line to the location bar:
 
Note: replace the “username” with your login username.
 
2. Right click and select “New -> Shortcut.”
 
3. For the location of the item, enter the following command:
 
Replace “X:” with the drive letter you want to use and “path/to/your/folder” to the folder that you want to mount. For example: subst S: "C:\Dropbox"
 
4. Click Next. Give a name to this shortcut.
 
Click Finish. You should now see a new shortcut in the Startup folder. Double click on it and it will be mounted as a virtual drive. Since it is in the Startup folder, it will be mounted automatically on the next (and every) startup.
 
To delete the virtual drive, simply delete the shortcut file. 
 
## Conclusion
 
Mounting a folder as a virtual drive allows you to quickly access your folder with a single click. This is particularly useful for cloud storage services like Dropbox, Google Drive and OneDrive that reside in their own folders. Try it out and let us know if this is useful to you.
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




