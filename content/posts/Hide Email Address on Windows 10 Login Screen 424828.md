---
title: "Is Your Email Address Exposed on Windows 10 Login Screen? Here's How to Hide It Now!"
ShowToc: true 
date: "2023-06-21"
author: "Janice Posey"
---
*****
+++
title = "Is Your Email Address Exposed on Windows 10 Login Screen? Here's How to Hide It Now!"
date = "2021-09-22"
author = "Your Name"
tags = ["Windows 10", "security", "privacy"]
+++

Are you concerned about your email address being displayed on the Windows 10 login screen? Do you worry about an unauthorized person gaining access to your sensitive information? If so, you're not alone. In this article, we'll discuss how to hide your email address on the Windows 10 login screen.

Why is your email address displayed on the Windows 10 login screen?

When you set up your Windows 10 account, you're asked to use an email address as your username. This email address is displayed on the login screen by default. The idea behind this is to make it easier for you to identify which account to log into.

However, displaying your email address on the login screen can be problematic, especially if multiple users have access to your device, or if someone is looking over your shoulder as you type in your login credentials. It's always a good idea to keep sensitive information hidden from prying eyes.

How to hide your email address on the Windows 10 login screen

The good news is that you can easily hide your email address from the Windows 10 login screen by following these steps:

1. Press the Windows key + R on your keyboard to open the Run dialog box.
2. Type in netplwiz and press Enter.
3. This will open the User Accounts window. Uncheck the box that says "Users must enter a user name and password to use this computer."
4. Click Apply.
5. A new window will appear prompting you to enter your login credentials. Type in your username and password, but this time use the local account instead of your email address.
6. Click OK.
7. Restart your computer to see the changes take effect.

Congratulations! You've successfully hidden your email address from the Windows 10 login screen. From now on, only your username will be displayed.

Benefits of hiding your email address on the Windows 10 login screen

By hiding your email address on the Windows 10 login screen, you're taking an important step to secure your personal data. Anyone who tries to log into your device will only see your username, and not your email address. This makes it more difficult for them to gain unauthorized access to your account.

Additionally, by using a local account instead of your email address as your login credentials, you're also adding another layer of protection. With a local account, you'll need both a username and a password to log in. This provides extra security and makes it more difficult for anyone to compromise your account.

Conclusion

It's always important to take steps to protect your personal information online. By hiding your email address from the Windows 10 login screen, you're taking an important step to secure your device and your personal data. Follow the steps outlined in this article to protect your privacy and stay safe online.

{{< youtube 8-BhognwEaE >}} 



Windows 10 by default shows the email address and the name of the user account on the Login or Sign-in screen, but when you share your computer with many other users, this can lead to privacy issues. You might not be comfortable sharing your personal information such as name and email with other users, which is why we have curated this article, which will show you how to hide your personal details easily.
 

 
If you use your PC in public, you might want to hide such personal information on the login screen or even when you leave your PC unattended, and hackers can take note of such personal details that might give them access to your PC. The login screen itself doesn’t reveal the name and email address of the last users who logged in, and you have to click on the particular username to see such details. Anyway, without wasting any time, let’s see how to Hide Email Address on Windows 10 Login Screen with the help of the below-listed guide.
 
Note: Once you follow the below method, you will need to enter the username and password for your user account manually.
 
## Hide Email Address on Windows 10 Login Screen
 
Make sure to create a restore point, just in case something goes wrong.
 
Contents
 
- Hide Email Address on Windows 10 Login Screen
 - Method 1: Hide Email Address using Windows 10 Settings
 - Method 2: Hide Email Address Using Registry Editor
 - Method 3: Hide Email Address Using Group Policy

 
Note: If you’re using Windows 10 Pro or Enterprise Edition then follow Method 3.
 
### Method 1: Hide Email Address using Windows 10 Settings
 
1. Press Windows Key + I to open Settings then click on Accounts.
 
2. From the left-hand menu, click on Sign-in options.
 
3. Scroll down to Privacy section and then disable the toggle for “Show account details (e.g. email address) on the sign-in screen“.
 
4. Reboot your PC to save changes, and you will be able to Hide Email Address on Windows 10 Login Screen.
 
The above method will only remove your email address from the login screen, but your name & picture will still be there, but if you want to remove these details, follow the below registry trick.
 
### Method 2: Hide Email Address Using Registry Editor
 
Note: If you have followed the above method, then don’t use step 1 to 5 as they will also hide email address on the login screen instead if you want to hide your name & picture then start from the step 6.
 
1. Press Windows Key + R then type regedit and hit Enter.
 
2. Navigate to the following registry key:
 
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System
 
3. Right-click on System the select New > DWORD (32-bit) Value.
 
4. Name this newly created DWORD as BlockUserFromShowingAccountDetailsOnSignin.
 
5. Double click on this DWORD and set its value to 1.
 
6. Now under System in the right window pane double click on dontdisplayusername.
 
Note: If the above key is not present, you need to create it manually.
 
7. Set its value to 1 and then click OK.
 
8. Again right-click on System the select New > DWORD (32-bit) Value. Name the new DWORD as DontDisplayLockedUserID.
 
9. Double click on DontDisplayLockedUserID and set its value to 3 and then click OK.
 
10. Reboot your PC to save changes, and you will be able to Hide Email Address on Windows 10 Login Screen.
 
### Method 3: Hide Email Address Using Group Policy
 
1. Press Windows Key + R then type gpedit.msc and hit Enter.
 
2. Now, in the left-hand menu, navigate to the following:
 
Computer Configuration > Windows Settings > Security Settings > Local Policies > Security Options
 
3. Make sure to select Logon then in the right window pane double-click on “Interactive Logon: Display user information when the session is locked“.
 
4. In the Properties window from the dropdown, select “Do not display user information” to hide the email address from the login screen.
 
5. Click Apply, followed by OK.
 
6. Now under the same folder, i.e. Security Options find “Interactive logon: Do not display last user name“.
 
7. In the Properties window select Enabled. Click Apply followed, OK.
 
8. Reboot your PC to save changes.
 
Recommended:
 
- Fix Windows can’t set up a HomeGroup on this computer
 - Fix Computer Screen Turns Off Randomly
 - Fix Windows 10 Taskbar Won’t Auto Hide
 - How to Read Memory Dump Files in Windows 10

 
That’s it you have successfully learned How to Hide Email Address on Windows 10 Login Screen but if you still have any queries regarding this guide then feel free to ask them in the comment’s section.




