---
title: "You won't believe how easy it is to manage your user password in Linux using just the terminal!"
ShowToc: true 
date: "2022-11-28"
author: "Brian Litherland"
---
*****
Title: Managing User Passwords in Linux Using Terminal Made Easy

Introduction
When it comes to managing user passwords on a Linux system, it can be a daunting task, especially for those who are new to the operating system environment. However, managing user passwords in Linux doesn't have to be complicated. In fact, it's easy to manage user passwords using just a terminal. In this article, we will take you through the simple steps to manage user passwords using the terminal. 

Step 1: Open the Terminal 
The first step to managing user passwords in Linux is to open the terminal. You can open the terminal using the keyboard shortcut CTRL+ALT+T or by typing "Terminal" in the search menu on Ubuntu's desktop. 

Step 2: Change the Password 
To begin changing the password of the user, you will first have to switch to that particular user account. This can be done by using the following command: 

sudo su - user 

You will need to replace the "user" with the name of the user account you wish to manage. 

After changing to the user account, the next step is to change the password of that particular user by typing the following command: 

passwd 

You will then be prompted to enter the new password twice. Ensure the password is strong enough and easy to remember. After verifying the new password, it will be immediately changed. 

Step 3: Creating a New User 
Creating a new user is another essential aspect of managing users in Linux. To create a new user, enter the following command: 

sudo adduser username 

Replace "username" with the name of your new user account. You will then be prompted to create a strong password and fill in other necessary details such as the full name of the new user account, room number, work phone, home phone, and any other additional information. 

Step 4: Deleting a User 
If you no longer need a user account and wish to remove it from your Linux system, you can delete the user using the following command: 

sudo deluser username 

Replace "username" with the name of the user account that you wish to delete. 

Conclusion 
The terminal is a powerful tool for managing user passwords on Linux, and with the steps outlined above, it's easy to change, create and delete user accounts in Linux using the terminal. With practice and mastery of terminal commands, managing user passwords in Linux won't be a daunting task anymore.

{{< youtube PeCBpI1hT2Q >}} 



Like with so many things in the Linux world, passwords are most easily managed directly from the command line. The passwd utility was designed to allow you quick and easy access to all of the password-related commands on your system. You can use it to change and manage your own password as well as the passwords of other users on your system. You can also use it to disable password authentication for a user, lock a user’s account, and set mandatory expiration dates, all to keep your system secure.
 
Let’s take a look at the passwd utility and how you can use it to manage your password in Linux.
 
## Change Your Password
 

 
First, the easiest thing you can do with the passwd utility is change your own password. Just use the passwd command with nothing else.
 
It’ll ask you to supply your current password followed by your new one.
 
## Change Someone Else’s Password
 
With root privileges or sudo, you can change someone else’s password, too. Just give passwd the account username for the password you want to change.
 
This time it won’t ask for their current password. It will only ask for you to set a new one.
 
## Locking a Password
 
You can just as easily lock a user’s account by locking their password. This will make them unable to sign in using a password. Other methods, like SSH keys, will still work. In order to lock an account, you’ll need sudo and the -l flag.
 
You can unlock an account, too, with the -u flag.
 
### Locking Root
 
If, for security reasons, you want to lock all access to the root account, leaving sudo the only way to manage the system, you can do that, too.
 
It works the same as with any other user.
 
## Using an Empty Password
 
You can also choose to set a user with an empty password. This is a really bad idea for security, but it can save you a lot of hassle on things like multimedia PCs that you don’t necessarily need to secure that way. Once again, passwd has a simple flag to remove a user’s password, making it blank.
 
## Password Expiration
 
It’s fairly common to set passwords to expire every so often. It’s a good security measure that prevents stale user passwords from compromising a system. If you’re running a system in a business situation, it’s hard to control what your customers use as their passwords and whether they get compromised. Forcing them to change their password after a set time frame will force your users to keep fresh passwords and reduce the risk of a breach.
 
Use the -x flag followed by the number of days you want the user’s password to be valid.
 
That will set the user’s password to expire after thirty days.
 
You can also set up a system to warn the user that their password will expire soon. Use the -w flag with the amount of days before expiration to automatically warn the user to change their password.
 
If you know there has already been an issue with a user’s password, you can automatically make their password expire. This will force them to set a new one immediately.
 
That’s all you really need to get started with passwd. If you’d like to see more of what it can do, check out the utility’s man page.
 
It’ll tell you everything that you can do with passwd. Passwd is an invaluable tool for Linux administrators. Even if you’re not running a big business server, you can still take advantage of passwd to keep your desktop more secure.
 
Nick is a freelance tech. journalist, Linux enthusiast, and a long time PC gamer.
 
Our latest tutorials delivered straight to your inbox




