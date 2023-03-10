---
title: "Revolutionize Your Linux User Management with These Command Line Tricks!"
ShowToc: true 
date: "2022-11-29"
author: "Scott Fredrickson"
---
*****
Revolutionize Your Linux User Management with These Command Line Tricks!

Are you tired of managing users on your Linux system manually? Do you find the Graphical User Interface (GUI) tools too cumbersome to use? Fear not, for the Linux command line can make user management a breeze. In this article, we will introduce you to some nifty command line tricks that will revolutionize the way you manage users on Linux systems.

Add a new user and assign a password

To add a new user to your Linux system, use the useradd command followed by the desired username, as shown below:

```
sudo useradd john
```

To assign a password to the new user, use the passwd command, followed by the desired username.

```
sudo passwd john
```

Delete an existing user

To delete an existing user from your Linux system, use the userdel command, followed by the username you wish to delete.

```
sudo userdel john
```

Note that the userdel command deletes the user's home directory as well unless you use the --preserve-home option.

Change the user's password

To change a user's password, use the passwd command, followed by the desired username.

```
sudo passwd john
```

You will be asked to enter the new password twice for confirmation. Once the password has been changed, the user will no longer be able to log in with the old password.

Modify a user's account

To modify an existing user's account, use the usermod command, followed by the username and the option you wish to modify. For example, to change the user's home directory:

```
sudo usermod -d /home/john_new john
```

Lock a user account

To lock an existing user's account, use the passwd command with the -l option, followed by the username.

```
sudo passwd -l john
```

This will prevent the user from logging in until the account is unlocked.

Unlock a user account

To unlock a locked user account, use the passwd command with the -u option, followed by the username.

```
sudo passwd -u john
```

This will allow the user to log in again.

Conclusion

These command line tricks are just the tip of the iceberg when it comes to Linux user management. The command line can be a powerful tool to manage users efficiently and quickly, without having to rely on the GUI. Whether you are a seasoned Linux administrator or a newbie, these tips will help you to take control of your Linux user management with ease.

{{< youtube AVXYq8aL47Q >}} 



One of the central responsibilities of Linux administration is the management of users. Through the use of the command line, user creation can be completed remotely or programmatically. Once you’ve created a user, you can then add them to groups or give them escalated privileges. In addition, you are able to keep an audit trail on what has been done on your server and any potential issues.
 
If you’ve developed software or programmed for the Web, you might be familiar with the policy of never trusting users. This same premise applies in other areas of computer usage in regards to user involvement. Only give access to those who need it and when they need it. Generous delegation of privileges could allow unspecified and unauthorized access to others’ information and core data.
 
## Viewing existing users
 
One of the quickest ways to view users is to use the cat (concatenate) or more (pager) commands to view the list of users on the system. The file you will need to view is the “/etc/passwd” file. This file stores all user accounts and user login information.
 
## Utilizing the useradd command
 
useradd is a low-level binary available on most distros. This command is typically less used due to it being less user-friendly and intuitive compared to the adduser command. However, there are very few differences and either can be used.
 
To find out more about useradd, run the man command or add --help to get a quick overview.
 

 
To add a user using useradd, type useradd and the name of the login you want to create.
 
In the case above, the user “testuser” will be created. By default, this command will only create the user and nothing else. If you need a home directory for this user, append the --create-home flag to create the home directory for the user.
 
## Utilizing the adduser command
 
The adduser command is a perl script that will create the user similar to the useradd command. What makes it different is that it is an interactive command and will prompt you to set the password, the home directory path, etc. Take note that on some distros, such as Red Hat and CentOS, adduser is a symbolic link to useradd, and on other distro like Arch Linux, adduser comes as a package that is not installed by default.
 
Using this command will create a group for the user using the user’s login by default. Other defaults can typically be found in the useradd file at “/etc/default”.
 
In this file you can change default settings for users created with useradd such as the shell and the home directory.
 
Run the adduser command similar to the following:
 
This will then prompt you regarding the defaults you want set and ask you for the password.
 
## Passwords and security
 
Adding a password for a user will require running the passwd command.
 
Without superuser privileges, running passwd will only change the password of the logged-in user. This command will test the password for complexity. On Ubuntu password requirements are set in the common-password file located in “/ec/pam.d.” More information regarding updating the complexity can be found in the man page for pam-auth-update.
 
## Updating user information
 
Once a user is on the system, you can review the “/etc/passwd” file to see the user’s information and encrypted password. If you need to make changes to a user, you will need to utilize the usermod command.
 
As an example, to change the user id for the testuser4 account created above, you would run the command:
 
You can then review the changes in the “/etc/passwd” file.
 
Be careful of changing critical information such as the login name, or as in this case, the user id. Review the man page for usermod to see what you will need to do if those items are changed.
 
## Adding users to group
 
There are times when you need to add users to a group so they have the necessary permission to run certain tasks.
 
To add a user to a group:
 
Note that the -a flag is necessary to “append” the group for the user. If not, you will risk removing the user from the “sudo” group if the user is supposed to have superuser permission.
 
Alternatively, you can use the gpasswd command to add/remove user to/from group.
 
To remove user from a group:
 
## Removing users
 
Similar to the other user commands, deleting a user is prefixed with “user” and the action. In this case you will need to use the userdel command.
 
Take note that userdel will not remove a user if there are processes using that user’s account.
 
## Viewing user logs
 
Depending on your distro, you will either check the auth log or the secure log located in “/var/log” to review user logins. This log file will give you logins on your system as soon as they happen. This is a critical element to monitoring events in the case of a breach and just to ensure things are working as desired.
 
User management is a crucial part of managing Linux servers if there is more than one person who will use your system. Using the command line will allow you to quickly administer users, as well as have a history of account creation and changes. Perhaps one of the best uses would be to automate creation with a shell script if multiple accounts are needed at once.
 
Either way, be sure to go through your accounts on a regular basis and remove accounts that are no longer needed. Ensure access is granted only to those who currently need access and monitor your logs frequently.
 
Our latest tutorials delivered straight to your inbox




