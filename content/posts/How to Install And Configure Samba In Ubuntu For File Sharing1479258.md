---
title: "You won't believe how easy it is to share files on Ubuntu with this one simple trick: Install and Configure Samba!"
ShowToc: true 
date: "2023-03-15"
author: "William Barron"
---
*****
Title: You Won't Believe How Easy it is to Share Files on Ubuntu with This One Simple Trick: Install and Configure Samba!

Introduction:
As a Ubuntu user, you might find it difficult to share files between different computers running on different operating systems. However, it's not so difficult - in fact, it's incredibly easy! How? By installing and configuring Samba. 

Body:
So, what exactly is Samba? It is a free and open-source software suite that allows you to share files, printers, and other resources between computers. Basically, it enables communication between Ubuntu and Windows systems, making sharing files a breeze. 

Now, let's get started with the installation process:

Step 1: Open Terminal on Ubuntu and type the following command to update the system's package list:
sudo apt-get update 

Step 2: Type the following command to install Samba:
sudo apt-get install samba 

Step 3: Once the installation is complete, it's time to configure Samba. First, we will need to create a directory that we want to share. Let's create a folder on the Desktop and name it "Shared": 
mkdir ~/Desktop/Shared 

Step 4: Next, we need to modify the Samba configuration file. Type the following command to open the file:
sudo nano /etc/samba/smb.conf 

Step 5: Scroll down to the last line of the file and add the following lines:
[Shared]
comment = Shared Folder
path = ~/Desktop/Shared
read only = no
guest ok = yes

Step 6: Press Ctrl+X to save and exit the file. 

Step 7: Restart Samba by typing the following command:
sudo service smbd restart 

Congratulations! You have successfully installed and configured Samba on Ubuntu. 

Now, let's see how to access the shared folder from a Windows computer:

Step 1: Open File Explorer on your Windows computer and navigate to "Network". 

Step 2: You should be able to see your Ubuntu computer's name. Double-click on it. 

Step 3: You will see the "Shared" folder that you created earlier. Double-click on it to access the contents. 

Voila! You can now easily share files between Ubuntu and Windows systems using Samba. 

Conclusion:
Samba is a powerful tool that makes sharing files between Ubuntu and Windows systems incredibly easy. By following the simple steps outlined above, you can easily install and configure Samba on your Ubuntu system and start sharing files in no time. So what are you waiting for? Go ahead and give it a try!

{{< youtube 7Q0mnAT1MRg >}} 



Samba is a useful service found in most Unix and Linux system that allows you to share file and print services with another computer, particularly a Microsoft Windows client. In Ubuntu, while the Nautiilus File Manager comes with a series of connection protocols to access files from a remote server, it doesn’t turn the machine into a file server and accept connection from other PC. Samba is the one that does the job. In this tutorial, we will show you how to install and configure Samba so you can turn your Ubuntu PC into a file server.

 
## Installing Samba
 
Samba is not installed by default. Open a terminal and type the following command:
 
Alternatively, you can install Samba via the Ubuntu Software Center.
 
## Configuring Samba
 
To get Samba to work the way we want it to work, we have to make some changes to its configuration file. 
 
In the terminal, 
 
This will open the config file in Gedit.
 
Scroll down the page until you see the line:
 
This is the identifier of your PC. You can keep it as the default, but it is best to change it to something more meaningful, like “HOME-DESKTOP”. 
 

 
Next, scroll down further till you reach the “Authentication” section. You should see the line:
 
Remove the “#” at the front of the line.
 
Continue to scroll down further until you reach the “Share Definitions” section. This is where you configure the files/folders that you want to share with others.
 
If you want the Home folder to be accessible, you should uncomment (remove the “;” at the front of the line) the following lines:
 
Don’t forget to change the browseable value to “yes”. You can also uncomment the read only = no line if you allow others to write to your Home folder.  
 
The last line  valid users = %S means that only you, or anyone with your login account, can connect to your own Home folder via Samba. 
 
To add additional file sharing path, add the following lines to the end of the file:
 
Change the name of this share configuration and change the path to the folder you want to share.
 
You can change the “guest ok=yes” line to “guest ok=no” if you want the share path only available for logged in users.
 
Lastly, save and exit the file. 
 
## Setting Samba user password
 
To add yourself to the Samba user list, you just have to type the following command:
 
Replace <username> with your username. It will then prompt you to set a password for this Samba account.
 
Alternatively, you can also create a new user account and add this user to the Samba user list
 
To create a user account, use the following command:
 
Restart Samba services
 
That’s it. You should be able to connect to this PC from another PC. 
 
## More Samba Tips
 
If you are looking for an easier way to configure the Samba settings, you can install “Samba Server Configuration” GUI.
 
On your Nautilus File Manager, you can also right-click on any folder and select the Sharing Options to enable sharing. 
 
Enjoy!
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




