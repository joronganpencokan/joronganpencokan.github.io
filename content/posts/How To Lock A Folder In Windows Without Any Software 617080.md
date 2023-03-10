---
title: "You Won't Believe How Easy It Is To Lock A Folder In Windows Without Spending A Dime!"
ShowToc: true 
date: "2023-01-24"
author: "Cynthia Anderson"
---
*****
Title: You Won't Believe How Easy It Is To Lock A Folder In Windows Without Spending A Dime!

Have you ever wanted to keep your confidential or sensitive files away from prying eyes? Maybe it’s your personal diary, your financial documents, or your browsing history that you’d like to keep private. Fortunately, Windows offers a simple way to lock your folders without the need for any third-party software or expensive apps. In this article, we’ll show you how you can use Windows to lock your folders easily, and best of all, it’s free!

Before we dive into the steps of locking a folder in Windows, let’s clarify what it means. Locking a folder means that no one, including the users with administrator rights, can access its contents without first unlocking it through a password. This process adds an extra layer of security to your confidential files and folders, making it difficult for anyone to tamper with them.

So, how do you lock a folder in Windows easily and for free? Here’s a step-by-step guide:

1. First, create a new folder on your desktop or anywhere else on your computer where you want to store your confidential files.

2. Right-click on the folder and select “Properties” from the dropdown menu.

3. In the Properties dialog box, click on the “Advanced” button.

4. In the Advanced Attributes dialog box, check the box next to “Encrypt contents to secure data.”

5. Click “OK” and then click “Apply.”

6. You’ll be prompted to back up the encryption key. Choose “EFSWizard.exe” to save the key.

7. Set up a strong password to use as your encryption key.

After following these simple steps, your folder is now encrypted and locked, and only you will be able to access it using your password. It’s that easy!

Now, let’s address some common concerns you might have about locking your files this way. First, it’s important to note that this method only works on local drives, not on external devices, so be aware of that when storing sensitive data. Second, if you forget your password, it’s impossible to unlock your folder, so create a strong password and make sure you remember it.

In conclusion, locking a folder in Windows doesn’t require any fancy software or expensive apps. With these simple steps, you can keep your confidential files and folders secure from prying eyes. It’s an easy way to add that extra layer of security to your digital life. So, go ahead and try it out - you won’t believe how easy it is!

{{< youtube 5bEimiIZ9dA >}} 



We do all sorts of things with our system. Whether it is watching movies or preparing an excel sheet for office. We totally rely on our system for, well, almost everything. And when we use our system that extravagantly, then there will be always some data to protect from others.
 
Now, this “precious” data of yours can be anything, like your personal photos, or some confidential file. And we all run into situations when we have to give up our system to someone else. Those kinds of situations are really scary, even if the other person is using our system for a short time. So, the best thing you could do is lock the folder which contains the files you want to protect. Because by doing that, you’ll only get scared while watching Conjuring, and not because you want to hide something on your Windows system. And in this article, we’re going to show you how you can do that and that too without any software.
 
Recommended Read: NTUSER.DAT File Meaning And Its Use
 
## Lock A Folder In Windows Without Any Software
 
In order to lock or protect a folder with a password on Windows, you have to create a Batch(BAT) file. Don’t worry, we’re going to guide you through it all. However, it might be good if you save a backup of your file before testing the method for the first time.
 
1. First, open the folder which you want to lock.
 
2. Next, right-click within that folder and navigate to New > Text Document.
 

 
3. When you do that, a blank notepad page will open up. Paste the code given below on that page.
 
cls
 
@ECHO OFF
 
title Folder Locker
 
if EXIST “Control Panel.{21EC2020-3AEA-1069-A2DD-08002B30309D}” goto UNLOCK
 
if NOT EXIST Locker goto MDLOCKER
 
:CONFIRM
 
echo Are you sure u want to Lock the folder(Y/N)
 
set/p “cho=>”
 
if %cho%==Y goto LOCK
 
if %cho%==y goto LOCK
 
if %cho%==n goto END
 
if %cho%==N goto END
 
echo Invalid choice.
 
goto CONFIRM
 
:LOCK
 
ren Locker “Control Panel.{21EC2020-3AEA-1069-A2DD-08002B30309D}”
 
attrib +h +s “Control Panel.{21EC2020-3AEA-1069-A2DD-08002B30309D}”
 
echo Folder locked
 
goto End
 
:UNLOCK
 
echo Enter password to Unlock folder
 
set/p “pass=>”
 
if NOT %pass%==Your-Password-Here goto FAIL
 
attrib -h -s “Control Panel.{21EC2020-3AEA-1069-A2DD-08002B30309D}”
 
ren “Control Panel.{21EC2020-3AEA-1069-A2DD-08002B30309D}” Locker
 
echo Folder Unlocked successfully
 
:FAIL
 
echo Invalid password
 
goto end
 
:MDLOCKER
 
md Locker
 
echo Locker created successfully
 
:End
 
4. Within that code, find the line if NOT %pass%==Your-Password-Here goto FAIL. You can use the Ctlr+F shortcut to search for it.
 
5. Now, change the Your-Password-Here bit in that line with the password you want to set for the folder. Like, if I want to use the password ‘Jumanji,’ then the line will be changed to if NOT %pass%==Jumanji goto FAIL.
 
6. As soon as you’re done with that, Click on File at the top left corner and select Save As… option.
 
7. In the Save as type: change the file type to ‘All Files’ by using the drop-down arrow.
 
8. Then, change the file name to anything you want. However, you have to end the name with .bat. Like if I used the file name ‘lock,’ then I would use ‘lock.bat’ as the full name.
 
9. After giving it a name, click on the Save option.
 
10. After the ninth step, you’ll see that a batch file has been created in the same folder. Click on it and a new blank folder will be created.
 
11. Move all the content you want to protect in the created folder.
 
12. Then again click on the batch file and answer the Are you sure u want to Lock the folder(Y/N) question with Y and hit ENTER.
 
13. Now, the folder in which you’ve moved your data will disappear.
 
14. In order to reveal that folder, you have to click on the Batch file again and provide the password you’ve used while creating the Batch file.
 
15. After putting in the password, you’ll be able to access the folder with ease.
 
Do note that once you unlock the folder, you have to repeat the twelfth step in order to lock it again.
 
Recommended Read: SuperFetch Meaning And How To Turn It On/Off
 
### Wrapping Up
 
So, locking a folder on Windows doesn’t seem so difficult now, right? You can now lock as many folders as you want. Although, do remember to note down your password to be secure. Because you never know when your memory is going to betray you.




