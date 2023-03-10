---
title: "Protect Your Most Private Files With This Genius Windows 10 Trick!"
ShowToc: true 
date: "2023-01-15"
author: "Jean Faulk"
---
*****
Title: Protect Your Most Private Files With This Genius Windows 10 Trick!

Introduction:

Do you have files on your Windows 10 computer that you absolutely don't want anyone else to access? Maybe it's sensitive business documents, confidential emails or even personal photos that you don't want to share with anyone. Well, there's good news. Windows 10 comes with an inbuilt feature that allows you to protect your most private files without the need for any third-party software.

What is this genius Windows 10 trick? Let's find out.

Step 1: Creating A Folder

The first step is to create a new folder on your computer. This is where you'll store all your private files. Right-click on your desktop and click on "New". Then click on "Folder". Give the folder a name that's easy to remember, such as "Private Files".

Step 2: Renaming The Folder

Once you've created the folder, it's time to give it a hidden name. This means that the folder won't show up in your normal directory, and only you will know where to find it. To change the folder name, right-click on the folder and click on "Properties".

In the Properties window, click on the "Customize" tab. Under the "Folder icons" section, click on "Change Icon". You'll see a list of icons. Choose a blank icon, and then click on "OK" twice to close both windows. You'll notice that the folder now has no name.

Step 3: Setting A Password

The final step is to set a password to protect the folder. Right-click on the folder and click on "Properties" again. This time, click on the "Security" tab. Click on "Edit", then click on "Add". Enter your Windows user name, and click on "OK".

In the "Permissions for" section, click on your user name. Under "Permissions" in the lower section, click on "Deny" next to "Full Control" and "Modify". Then click on "OK". This will ensure that no one, including you, can modify, delete or access the folder without first entering a password.

To set the password, right-click on the folder and select "7-Zip" from the context menu (if you don't have 7-Zip installed, you can download it for free). Click on "Add to Archive". In the window that pops up, enter a name for the archive and choose "zip" as the archive format. Under "Encryption", enter a password and click on "OK".

Conclusion:

And there you have it - a genius Windows 10 trick that allows you to protect your most private files with a password, without the need for any third-party software. Just remember where you've hidden the folder, and keep the password safe. Your files will be safe from prying eyes.

{{< youtube Fuu5-c-Nqpk >}} 




This article explains how to lock a folder in Windows 10 using the built-in encryption tool or a password protection program.

 
### 
What to Know
 
- To encrypt a folder, right-click it and select Properties > Advanced > Encrypt contents to secure data.To back up encryption keys, enter certmgr.msc into the Run dialog box, and go to Personal > Certificates.To password-protect folders, install a program like Wise Folder Hider.

 
##   How Do I Lock a Specific Folder?  
 

Windows has an encryption tool to prevent other users from opening your files, but install a more robust third-party tool for greater privacy.

 

While there's more than one method, the easiest doesn't involve any third-party programs. Windows 10 has this feature built-in.

 
- Right-click the folder you want to lock, and select Properties.
 - Select Advanced at the bottom of the General tab.
 - Check the box next to Encrypt contents to secure data.
 - Select OK, and then OK again on the Properties window to save.
 - Windows will prompt you to back up your file encryption key to avoid permanently losing access to your encrypted files. You can follow those steps (keep reading) or ignore them.
 - If you don't see the prompt, but you still want to back up the encryption key, skip ahead to the next section.
 - Select Back up now (recommended) if you followed the notification to back it up.
 - Start the Certificate Export Wizard by selecting Next on the first screen.
 - Keep the defaults selected, and then press Next again.
 - Select the box next to Password to enable the password, and fill out the text fields below. Select Next.
 - Choose where to save the PFX file, and give it a name.
 - Select Next to review the information you provided and select Finish to complete the export.
 - Select OK on the successful export prompt. If you ever need to use this certificate, just open it from wherever you saved it in step 9, and follow the on-screen prompts.

 
##   How to Back Up Locked Folder Encryption Keys in Windows 10  
 

Follow these steps to manually back up keys for encrypted folders:

 
This article covers three methods. See the section directly below these steps to learn how this process works; you might prefer to use one of the other techniques instead of this one.
 

Right-click the folder you want to lock, and select Properties.

 

Select Advanced at the bottom of the General tab.

 

Check the box next to Encrypt contents to secure data.

 

Select OK, and then OK again on the Properties window to save.

 

Windows will prompt you to back up your file encryption key to avoid permanently losing access to your encrypted files. You can follow those steps (keep reading) or ignore them.

 
If you don't see the prompt, but you still want to back up the encryption key, skip ahead to the next section.
 

Select Back up now (recommended) if you followed the notification to back it up.

 

Start the Certificate Export Wizard by selecting Next on the first screen.

 

Keep the defaults selected, and then press Next again.

 

Select the box next to Password to enable the password, and fill out the text fields below. Select Next.

 

Choose where to save the PFX file, and give it a name.

 

Select Next to review the information you provided and select Finish to complete the export.

 

Select OK on the successful export prompt. If you ever need to use this certificate, just open it from wherever you saved it in step 9, and follow the on-screen prompts.

 
- Press WIN+R to open the Run command (or just select the search bar on the taskbar), type certmgr.msc, then press Enter.
 - In the left pane, go to Personal > Certificates.
 - Select all certificates for Encrypting File System.
 - Right-click on the selected files, then go to All Tasks > Export.
 - Refer to steps 6-11 in the previous section to complete the backup.

 
##   How Encrypted Files Work on Windows 10  
 

You should know how encrypted files behave in Windows to ensure this is the method you want to use.

 

Press WIN+R to open the Run command (or just select the search bar on the taskbar), type certmgr.msc, then press Enter.

 

In the left pane, go to Personal > Certificates.

 

Select all certificates for Encrypting File System.

 

Right-click on the selected files, then go to All Tasks > Export.

 

Refer to steps 6-11 in the previous section to complete the backup.

 

Take this as an example: An encrypted folder exists on the root of the C drive of a computer with two users. John encrypts the folder and all the files inside it. He has complete control over the data.

 

Another user, Mark, logs in to his account, where he can do nearly everything John can:

 
- See file namesRename filesMove and delete the folder and its filesAdd more files to the folder

 

However, because John encrypted the files in the folder, Mark can't open them. Mark can, however, do essentially anything else.

 

Any files Mark adds to the encrypted folder are automatically encrypted, but now the permissions are reversed: Since Mark is the logged-in user, he can open the files he adds, but John can't.

 
##   Can You Put a Password on a Folder?  
 

Windows 10 doesn't have a way to put a password on a folder, apart from what we described above. That method is similar to other password protection techniques in that you need to provide the correct user account password before you can view the encrypted data.

 

There are, however, third-party tools that let you define any password as the folder password, utterly independent of the logged-in user. The methods described below are arguably more private than Windows' encryption procedure because they can obfuscate the file names and hide even the folder itself.

 
###   Password Protect and Hide the Folder  
 

Wise Folder Hider is a good example. This program is ideal if you're protective of the data because it can hide the folder behind two passwords. It can also secure entire flash drives and encrypt individual files.

 
- Open the program and define an initial password. This is what will be entered each time you want to open Wise Folder Hider.
 - From the Hide File tab, select Hide folder, and choose the folder you want to protect behind a password (or drag the folder into the program window). Any folder but system folders are allowed.
 - After choosing it, the folder will immediately disappear from its original location. To view it again, select the menu button to the right and select Open; it will open in File Explorer. Select Close to hide it again, or Unhide to permanently restore it.
 - Optionally, for greater security, you can force another password to be entered before opening that specific folder. To do that, press the down arrow to the right of the folder path, and select Set Password.

 
###   Make a Password Protected Copy  
 

7-Zip is another favorite. Instead of hiding the original folder, it creates a copy and then encrypts the copy.

 

Open the program and define an initial password. This is what will be entered each time you want to open Wise Folder Hider.

 

From the Hide File tab, select Hide folder, and choose the folder you want to protect behind a password (or drag the folder into the program window). Any folder but system folders are allowed.

 

After choosing it, the folder will immediately disappear from its original location. To view it again, select the menu button to the right and select Open; it will open in File Explorer. Select Close to hide it again, or Unhide to permanently restore it.

 

Optionally, for greater security, you can force another password to be entered before opening that specific folder. To do that, press the down arrow to the right of the folder path, and select Set Password.

 
- Right-click the folder and go to 7-Zip > Add to archive.
 - Change Archive format to be 7z.
 - Enter a password in the text fields in the Encryption section.
 - Optionally define other settings, such as these:
 - Archive is the file name and path to where the encrypted file should be saved.Encrypt file names prevents someone from seeing the file names without providing the password.Create SFX archive lets someone provide the password to decrypt the folder even if they don't have 7-Zip installed. Ideal for sharing the folder; it turns the file extension into EXE.Compression level can be set to a different level to make the file smaller, though it might also increase the encryption and decryption time.
 - Select OK.

 

Other apps are available if you prefer to put your secret files on a virtual hard drive with a custom password.

 

Right-click the folder and go to 7-Zip > Add to archive.

 

Change Archive format to be 7z.

 

Enter a password in the text fields in the Encryption section.

 

Optionally define other settings, such as these:

 
- Archive is the file name and path to where the encrypted file should be saved.Encrypt file names prevents someone from seeing the file names without providing the password.Create SFX archive lets someone provide the password to decrypt the folder even if they don't have 7-Zip installed. Ideal for sharing the folder; it turns the file extension into EXE.Compression level can be set to a different level to make the file smaller, though it might also increase the encryption and decryption time.

 

Select OK.

 
The original folder isn't deleted or changed in any way, so if you take this route, be sure to delete or move the original files after making the password-protected version.
 
A "locked folder" can also mean a folder with files currently in use, but that's not the same idea as a folder you'd lock intentionally for privacy reasons. See How to Move, Delete, and Rename Locked Files for more on how those files work.
 
- How do I lock a folder in Windows 10 to prevent deletion?
 - One option is to right-click the folder and choose Properties > Security > Advanced > Disable Inheritance > Convert inherited permissions into explicit permissions on this object. Then select a user from the list > Edit > Show advanced permissions > Type > Deny > and check the box beside Delete.
 - How do I hide a folder on my PC and lock it for myself in Windows 10?
 - To hide files and folders in Windows 10, right-click the folder and select Properties > General > Hidden > Apply > OK. While you can prevent hidden files from displaying by adjusting the File Explorer view, other users can easily show hidden items by changing this setting. A third-party tool to add password protection locks and hides folders more effectively.

 
One option is to right-click the folder and choose Properties > Security > Advanced > Disable Inheritance > Convert inherited permissions into explicit permissions on this object. Then select a user from the list > Edit > Show advanced permissions > Type > Deny > and check the box beside Delete. 
 
To hide files and folders in Windows 10, right-click the folder and select Properties > General > Hidden > Apply > OK. While you can prevent hidden files from displaying by adjusting the File Explorer view, other users can easily show hidden items by changing this setting. A third-party tool to add password protection locks and hides folders more effectively.
 

Get the Latest Tech News Delivered Every Day




