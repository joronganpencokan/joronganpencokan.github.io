---
title: "Unlock the Secrets of Windows 11: Become a Master Administrator with this Simple Trick!"
ShowToc: true 
date: "2023-03-03"
author: "Neva Strohschein"
---
*****
title: Unlock the Secrets of Windows 11: Become a Master Administrator with this Simple Trick!

Windows 11, the latest operating system from Microsoft, has a lot of new features and improvements over its predecessors. However, to fully take advantage of these features and customize your system, you need to have admin privileges. In this article, we will show you a simple trick to become a master administrator in Windows 11.

Before we start, let's have a brief look at what an administrator is and why you need to have admin privileges. An administrator is a user account with the highest level of access in Windows. Admin privileges allow you to install applications, make system-wide changes, and access sensitive files and settings that are usually hidden from normal users. In short, an administrator can control everything on a computer. 

Now, let's jump into the trick that will help you become a master administrator in Windows 11. Follow the steps mentioned below to get started:

Step 1: Open the Start menu and search for "CMD." Right-click on the Command Prompt option and select "Run as administrator." 

Step 2: In the Command Prompt window, type the following command:

net user administrator /active:yes

This command will activate the built-in administrator account in Windows 11. 

Step 3: Now, you can switch to the administrator account by logging out of your current user account and signing in with the administrator account. 

Step 4: Once you have logged in with the administrator account, you can make system-wide changes, install applications, and access sensitive files and settings. 

Step 5: To deactivate the administrator account, perform the same steps as above and type the following command in the Command Prompt window:

net user administrator /active:no

This will deactivate the administrator account, and you will return to your normal user account. 

In conclusion, becoming a master administrator in Windows 11 is a simple task that requires only a few steps. However, with great power comes great responsibility. Always use admin privileges with caution and only make necessary changes that you are sure of. Now that you have admin privileges, you can take full control of your Windows 11 system and unlock its secrets.

{{< youtube e3qRQOCWp-Q >}} 



If you have to change an account from “Standard User” to “Administrator,” you can complete this task from the Settings app, Command Prompt, or PowerShell, and in this guide, you will learn how on Windows 11.
 
On Windows 11, you typically use one of the two account types, the “Administrator” or “Standard User.” The Administrator type belongs to the “Administrators” and “Users” groups, and it offers unrestricted access, meaning that users can change global settings, install apps, and run elevated commands.
 
The Standard User type belongs only to the “Users” group, which means limited access to the device. The user can still run applications and change settings, but they can’t change global settings, install apps, or run elevated commands.
 
Although it’s recommended to use a Standard User account to work with Windows 11, sometimes, you may have reasons to switch to an Administrator account, and if you must change the account type, you can do this in at least three ways.
 
This guide will teach you the steps to change the account type from Standard User to Administrator on Windows 11.
 
## Change account type to administrator on Windows 11
 
On Windows 11, you can change the account type to make a user an administrator from the Settings app or using commands with PowerShell or Command Prompt.
 
### Settings method
 
To make a Standard User an Administrator on Windows 11, use these steps:
 
- Sign in (as admin) on Windows 11.
 - Open Settings.
 - Click on Accounts.
 - Click the Family & other users tab.
 - Under the “Other users” section, select the standard account and click the Change account type button.
 - Select the Administrator option.
 - Click the OK button.

 
Once you complete the steps, the account will have unrestricted access to change settings, install apps, and run elevated commands.
 
Sign in (as admin) on Windows 11.
 
Open Settings.
 
Click on Accounts.
 
Click the Family & other users tab.
 
Under the “Other users” section, select the standard account and click the Change account type button.
 

 
Select the Administrator option.
 
Click the OK button.
 
### Command Prompt method
 
To make a user account administrator from Command Prompt, use these steps:
 
- Open Start.
 - Search for Command Prompt, right-click the top result, and select the Run administrator option.
 - Sign in with an account that has administrator privileges.
 - Type the following command to list the available users and press Enter:
 - net user
 - Type the following command to add the account to the Administrators group and press Enter:
 - net localgroup Administrators "ACCOUNT-NAME" /add

 
After you complete the steps, sign out and sign back into the account to apply the changes and start using the account as an administrator.
 
Open Start.
 
Search for Command Prompt, right-click the top result, and select the Run administrator option.
 
Sign in with an account that has administrator privileges.
 
Type the following command to list the available users and press Enter:
 
net user
 
Type the following command to add the account to the Administrators group and press Enter:
 
net localgroup Administrators "ACCOUNT-NAME" /add
 
### PowerShell method
 
Alternatively, you can also use PowerShell to make a Standard User account an Administrator. You can do this while you are signed in as a Standard User.
 
To make a user account an administrator with PowerShell, use these steps:
 
- Open Start.
 - Search for PowerShell, right-click the top result, and select the Run as administrator option.
 - Type the following command to list the available users and press Enter:
 - Get-LocalUser
 - Type the following command to change the account type to “Administrator” and press Enter:
 - Add-LocalGroupMember -Group "Administrators" -Member "ACCOUNT-NAME"
 - In the command, change the ACCOUNT-NAME for the name of the account to change. The quotation marks are only necessary if there is a space in the name.

 
Once you complete the steps, the Standard User account will become an Administrator account.
 
Search for PowerShell, right-click the top result, and select the Run as administrator option.
 
Get-LocalUser
 
Type the following command to change the account type to “Administrator” and press Enter:
 
Add-LocalGroupMember -Group "Administrators" -Member "ACCOUNT-NAME"
 
In the command, change the ACCOUNT-NAME for the name of the account to change. The quotation marks are only necessary if there is a space in the name.




