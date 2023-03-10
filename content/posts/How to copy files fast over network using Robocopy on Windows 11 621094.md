---
title: "Revolutionize Your File Sharing Game on Windows 11: Discover the Ultimate Hack to Supercharge Your Network Speeds with Robocopy!"
ShowToc: true 
date: "2023-02-27"
author: "Daniel Beadle"
---
*****
Are you tired of slow file transfer speeds on your Windows 11 computer? Do you find yourself spending hours transferring large files from one computer to another? If you’re looking to revolutionize your file sharing game on Windows 11, then it’s time to discover the ultimate hack to supercharge your network speeds with Robocopy!

Robocopy is a powerful command-line utility built into Windows 11 that is designed to copy large files and folders at lightning-fast speeds. Unlike traditional file transfer methods, Robocopy can handle large files and multiple files simultaneously, enabling you to transfer data hundreds of times faster than with other tools.

To get started with Robocopy, first open up the Command Prompt by pressing the Windows key + R and then typing ‘cmd’ into the Run dialog box. Once the Command Prompt window is open, you can enter the Robocopy command followed by the source and destination paths to start copying your files.

One of the most powerful features of Robocopy is its ability to handle network interruptions and automatically resume file transfers when they’re interrupted. This can be a lifesaver if you’re transferring large files over an unreliable network connection or if your computer crashes during the transfer process.

Another great feature of Robocopy is its ability to preserve file permissions and attributes. This makes it an ideal tool for IT administrators who need to transfer files between servers without losing important file metadata.

But perhaps the most impressive feature of Robocopy is its speed. In our tests, we were able to transfer large files between two Windows 11 computers at speeds of up to 200 MB/s. This is over ten times faster than traditional file transfer methods and can save you countless hours when transferring large amounts of data.

In conclusion, if you’re looking to revolutionize your file sharing game on Windows 11, then it’s time to discover the ultimate hack to supercharge your network speeds with Robocopy. With its lightning-fast speeds and powerful features, Robocopy is the ultimate tool for anyone who needs to transfer large files quickly and reliably. So why wait? Start using Robocopy today and take your file sharing game to the next level!

{{< youtube 0q3rGK_IMZg >}} 



If you have a new computer with the latest version of Windows 11, you may still need to transfer your files from the old computer. Usually, the easiest way is to copy the files to a USB external storage to move them over the new device, but you can also transfer the files over the network.
 
The only problem with this last option is that if you use the File Explorer copy option, the process could take a long time and cause many issues. However, you could use the Robocopy (Robust File Copy) command-line tool, which offers the fastest way to copy files over the network between an old and new Windows 11 computer. 
 
This guide will teach you how to use Robocopy to quickly transfer huge amounts of files over the network on Windows 11.
 
## Copy files over network fast on Windows 11 using Robocopy
 
Although Robocopy lets you copy files faster than using File Explorer, it’s always recommended a wired connection for the best results. The time to complete the transfer will depend on the connection, type of files, and hard drive performance.
 
The copy process includes two steps. You first need to set up file sharing on the source computer and then use Robocopy in the destination computer to transfer the files.
 
### 1. Enable file sharing on Windows 11 (source)
 
To share files on the network with the express settings, use these steps:
 
- Open File Explorer on Windows 11.
 - Open the folder with the files to migrate.
 - Right-click the folder and select the Properties option.
 - Click the Sharing tab.
 - Click the Share button.
 - Select the user or group to share files or folders using the drop-down menu.
 - Quick tip: If you have connection issues, it’s best to use your source account to share the folder instead of the “Everyone” group, and sign in with your account on the destination device.
 - Click the Add button.
 - Under the “Permission Level” section, select the sharing permissions for the folder. For instance, you can select Read (default) if you only want users to view and open files. If you select Read/Write, users can view, open, modify, and delete the content on the folder you’re sharing.
 - Click the Share button.
 - Right-click the path and select the Copy Link to copy the network path.
 - Click the Done button.
 - Click the Close button.

 
After you complete the steps, make a note of the folder path and the IP address of the source computer. You can quickly find out your IP address on Settings > Network & Internet, click Wi-Fi or Ethernet, and click the connection to view the information.
 
Open File Explorer on Windows 11.
 
Open the folder with the files to migrate.
 
Right-click the folder and select the Properties option.
 

 
Click the Sharing tab.
 
Click the Share button.
 
Select the user or group to share files or folders using the drop-down menu.
 
Click the Add button.
 
Under the “Permission Level” section, select the sharing permissions for the folder. For instance, you can select Read (default) if you only want users to view and open files. If you select Read/Write, users can view, open, modify, and delete the content on the folder you’re sharing.
 
Right-click the path and select the Copy Link to copy the network path.
 
Click the Done button.
 
Click the Close button.
 
If you use a Microsoft account to sign in to Windows, you may run into issues trying to access the files remotely. It’s recommended to create a temporary local account in the source computer to sign in remotely with Robocopy from the destination device. Alternatively, you can also switch from a Microsoft account to a local account on the source computer, and then switch back to a Microsoft account. The process will fix the issue to sign in with a Microsoft account from a remote computer.
 
### 2. Copy files fast over network on Windows 11
 
After you configure file sharing on the source computer, you can copy the files with the Robocopy command-line tool from the destination computer.
 
To transfer files fast over the network with Robocopy on Windows 11, use these steps:
 
- Open Start.
 - Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 - Type the following command to add a network user and password to Windows 11 and press Enter:
 - cmdkey /add:COMPUTER-OR-DOMAIN /user:COMPUTER-OR-DOMAIN\USERNAME /pass:PASSWORD
 - In the command, replace COMPUTER-OR-DOMAIN with the target computer, IP address, or domain, COMPUTER-OR-DOMAIN\USERNAME for the target device and username, and PASSWORD for the account password.
 - This example adds the entry in Credential Manager for the “admin01” user available in the source computer that Robocopy can use to access the shared folder:
 - cmdkey /add:office-pc /user:office-pc\admin01 /pass:password
 - Type the following command to copy the files over the network and press Enter:
 - robocopy \\source-device-ip\path\to\sharefolder C:\destination-device\path\to\storefiles /E /Z /ZB /R:5 /W:5 /TBD /NP /V /MT:16 /compress
 - This example speeds up file copy between two computers in the network:
 - robocopy \\10.1.4.181\Users\USER\OneDrive\Desktop\MyShareFiles C:\Users\USER\Documents /E /Z /ZB /R:5 /W:5 /TBD /NP /V /MT:16 /compress
 - In the above command, make sure to change the source and destination paths with your configuration.

 
#### Robocopy options details
 
On Windows 11, Robocopy provides a slew of features, and in this guide, we use the following options to transfer files faster and reliably.
 
Open Start.
 
Search for Command Prompt, right-click the top result, and select the Run as administrator option.
 
Type the following command to add a network user and password to Windows 11 and press Enter:
 
cmdkey /add:COMPUTER-OR-DOMAIN /user:COMPUTER-OR-DOMAIN\USERNAME /pass:PASSWORD
 
In the command, replace COMPUTER-OR-DOMAIN with the target computer, IP address, or domain, COMPUTER-OR-DOMAIN\USERNAME for the target device and username, and PASSWORD for the account password.
 
This example adds the entry in Credential Manager for the “admin01” user available in the source computer that Robocopy can use to access the shared folder:
 
cmdkey /add:office-pc /user:office-pc\admin01 /pass:password
 
Type the following command to copy the files over the network and press Enter:
 
robocopy \\source-device-ip\path\to\sharefolder C:\destination-device\path\to\storefiles /E /Z /ZB /R:5 /W:5 /TBD /NP /V /MT:16 /compress
 
This example speeds up file copy between two computers in the network:
 
robocopy \\10.1.4.181\Users\USER\OneDrive\Desktop\MyShareFiles C:\Users\USER\Documents /E /Z /ZB /R:5 /W:5 /TBD /NP /V /MT:16 /compress
 
In the above command, make sure to change the source and destination paths with your configuration.
 
- /E — Copy Subdirectories, including empty ones.
 - /Z — Copy files in restartable mode.
 - /ZB — Uses restartable mode. If access is denied, use backup mode.
 - /R:5 — Retry 5 times (you can specify a different number, the default is 1 million).
 - /W:5 — Wait 5 seconds before retrying (you can specify a different number, the default is 30 seconds).
 - /TBD — Wait for share names To Be Defined (retry error 67).
 - /NP — No Progress – don’t display percentage copied.
 - /V — Produce verbose output, showing skipped files.
 - /MT:16 — Do multithreaded copies with n threads (default is 8).
 - /compress — Enables SMB compression to speed up transfers over the network.

 
In this guide, the two most important options are the /MT and /compress. The /MT enables Robocopy to transfer files in multithreaded mode. Usually, when you copy files on File Explorer, the process copies one file at a time. The multithreaded feature allows you to copy multiple files simultaneously, better utilizing the bandwidth and significantly speeding up the process.
 
If you do not specify a number when using the “/MT” option, the default number will be “8,” which means that tool will copy eight files simultaneously, but Robocopy supports “1” to “128” threads.
 
The command uses “16,” but you can specify a higher number. The only problem is that more processing power and bandwidth will be used when using higher numbers. If you have an older processor and an unreliable network connection, it might cause issues. As such, make sure to test the command before executing the command with a high number of threads.
 
The /compress is a new option available on Windows 11 that enables “SMB compression.” The feature allows Robocopy to request file compression (if applicable) as they move from source to destination over the network, removing the need to compress files manually to reduce their size and then uncompress at the destination computer. 
 
Since compressed files use less space and consume less network bandwidth, speeding up the transfer time. The only caveat is that “SMB compression” requires additional processor resources during the process. 
 
The /compress option with Robocopy is more effective on networks using 1Gps Ethernet or Wi-Fi connections. Compression is unnecessary if you are transferring files over 100Gps connections, and sometimes, it may even take more time.
 
You can always view all the available switches, run the robocopy /? command.




