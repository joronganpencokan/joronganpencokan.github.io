---
title: "Discover the Ultimate Guide to Mastering User Management in Ubuntu - You Won't Believe how Easy it Can Be!"
ShowToc: true 
date: "2023-01-10"
author: "George Angelini"
---
*****
# Discover the Ultimate Guide to Mastering User Management in Ubuntu - You Won't Believe how Easy it Can Be!

User management is a crucial aspect of any operating system, and Ubuntu is no exception. Whether you're a casual user, a system administrator, or somewhere in between, understanding how to manage users on your Ubuntu machine is essential to your success.

In this article, we'll walk you through the ultimate guide to mastering user management in Ubuntu. From creating users and groups to assigning permissions and managing passwords, we've got you covered. You won't believe how easy it can be!

## Creating Users and Groups

The first step in user management is, of course, creating new users and groups. In Ubuntu, this can be done through the command line or through the graphical user interface (GUI).

To create a new user via command line, simply open a terminal window and enter the following command:

```
sudo adduser username
```

Replace 'username' with your desired username and follow the prompts to complete the process.

To create a new user via the GUI, navigate to the 'System Settings' menu and select 'User Accounts'. From there, click the '+' button to add a new user and follow the prompts.

Similarly, to create a new group via command line, enter the following command:

```
sudo addgroup groupname
```

Replace 'groupname' with your desired group name and follow the prompts.

To create a new group via the GUI, click the 'Advanced Settings' button in the 'User Accounts' menu and select the 'Groups' tab. From there, click the '+' button to add a new group and follow the prompts.

## Assigning Permissions

Once you've created your users and groups, you'll need to assign permissions to control who can access what files and directories on your Ubuntu machine.

To assign permissions via command line, use the 'chmod' command followed by the file or directory you wish to modify and the desired permission values. For example, to give a user read, write, and execute permissions on a file, you would enter the following command:

```
sudo chmod u+rwx filename
```

To assign permissions via the GUI, simply right-click on the file or directory you wish to modify, select 'Properties', and navigate to the 'Permissions' tab.

## Managing Passwords

Finally, you'll need to manage your users' passwords to ensure the security of your Ubuntu machine.

To change a user's password via command line, enter the following command:

```
sudo passwd username
```

Replace 'username' with the desired user and follow the prompts to change the password.

To change a user's password via the GUI, navigate to the 'User Accounts' menu and select the user you wish to modify. From there, click the 'Password' button and follow the prompts to change the password.

## Conclusion

User management is a critical aspect of Ubuntu administration, but it doesn't have to be complicated. By following the steps outlined in this article, you can easily create new users and groups, assign appropriate permissions, and manage passwords to keep your Ubuntu machine running smoothly and securely.

{{< youtube bR94iccvn9s >}} 



Having your own space on a family computer can be a real sanity-saver. To always know your favorite apps are where you expect them to be, bookmarks don’t go missing, and documents are securely stored away from prying eyes, can be a real lifesaver. In this tutorial, we show you how to add and manage users in Ubuntu, adjust their privileges, and set up a “Family” folder to allow all users to have one space for collaboration or file sharing.
 
Note: this tutorial is based on Ubuntu 20.04 and Gnome 3.36, but the methods should be broadly similar across distros.
 
## Creating users
 
To begin, go into your Settings app and, from the left edge, choose Users. In order to make changes here, you’ll need to authenticate. Click “Unlock … ” from the top right and put in your password. You’ll now have access to the various tools, such as being able to change your username or password, set automatic login or view Account Activity. Later, as an administrator, you’ll be able to access this information for other accounts too.
 
Select “Add User … ” from the top of the window.
 
## Set up your users
 
On this screen you’ll define whether the new user has admin privileges or not – meaning they can make system level changes, install software, etc. – then provide a Full Name and Username. The latter is used to create the “/home” folder for the account and is not editable. Next, you’ll set passwords. In a family situation, you may want to choose the first option so that your users create a password when they log in, but in our case, we’re assigning a password from here.
 
Password security is always important, so Gnome sets a criteria and won’t allow you to proceed unless your choice has letters, numbers and punctuation. It should be easy to remember but hard to guess.
 
Once you select “Add,” you’ll be asked to authenticate once more, and the account will be created.
 
## Change passwords
 
Congratulations, you’re now a sysadmin with power to grant (and deny) access to files. This also means you’ll be the first port of call if your users forget their password because you can go into their accounts and either create a new password or reset the system so they can create a new password on their next login. To do this, simply select their name from the user list at the top, select the Password field, and set the appropriate action.
 
Next time you boot, you’ll be presented with a list of users. Each user can configure their desktop, taskbar and themes to suit. They’ll also have a directory on the system that is their home, which is generally inaccessible to other users.
 
## Sharing folders
 
There are many times when you want to share documents across accounts. We can do this by setting permissions on particular folders. In our case, we’re going to create a shared folder called “Family,” then instead of setting individual access to the folder, we’ll add other users to the group, called “andy,” that owns that folder. Then we can set permissions for the entire group.
 
Begin by opening Gnome’s file manager, going into the main admin’s Home folder, creating a new folder (right click -> New Folder) and giving it a name. The simple way to share this folder is to right-click and select “Local Network Share.” Selecting the subsequent “Share this folder” option will prompt the installation of the Linux Samba system, so Windows users can also access the folder. We’re not particularly interested in this at present, so we’re going to set things up manually.
 
Instead of the Network Share option, pick “Properties” from the right-click menu and select the Permissions tab.
 
Here you’ll see three classes of users. The owner can “Create and delete files,” the group (named after the owner) can “Access files” and others can also “Access files.” (Read this chmod 777 article for more details on file permission.) We want to elevate the permissions of the group so everyone in the “andy” group can fully access the folder. Change the setting to “Create and delete files.” Note that if you’re doing this to an established folder with lots of subfolders, you can select “Change Permissions for Enclosed Files” to have the change cascade through the folder.
 
## Adding users to a group
 
The most recent versions of Gnome have removed the ability to add users to a group using a graphical interface, so we’re going to need to do a few things at the terminal. Fortunately, it’s not too arduous.
 
Open the terminal – Ubuntu salts this away under the Utilities in its application menu – and type:
 
“Group” is the name of the group and “user” the name of the user. You’ll need to authenticate with your admin user password to make the change.
 
Your user, in their own account, can now navigate to “Computer -> Home -> username -> foldername” to access or add files to the shared folder.
 
The Linux share system is flexible enough to allow you to access your files even if you’re dual-booting Windows and Linux. Just be sure that you didn’t disable the lock screen for your family computer.
 
Andy Channelle is a writer and web developer who has written for Linux Format, Mac Format, 3D World and others, and has also published best-selling books on Ubuntu Linux and OpenOffice.org. He's recently worked on web projects and campaigns for the International Red Cross and the UN. He produces - but hardly ever releases - electronica under the name Collision Detector. Andy lives in Wales, UK.
 
Our latest tutorials delivered straight to your inbox




