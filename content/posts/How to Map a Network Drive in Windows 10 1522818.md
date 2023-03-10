---
title: "5 Mind-Blowing Hacks to Master Network Drive Mapping in Windows 10 like a Pro!"
ShowToc: true 
date: "2023-04-19"
author: "Kayla Lewis"
---
*****
# 5 Mind-Blowing Hacks to Master Network Drive Mapping in Windows 10 like a Pro!

Network drive mapping in Windows 10 can be a tricky task to master. But with the right tips and tricks, you can become a pro and take advantage of all the benefits of this feature. In this article, we’ll share five mind-blowing hacks that will help you get the most out of network drive mapping in Windows 10.

## Hack #1: Use Command Prompt to Map Network Drives

One of the quickest and most efficient ways to map network drives in Windows 10 is to use the Command Prompt. You can open the Command Prompt by pressing the Windows key + R, typing “cmd,” and pressing enter.

Once you’re in the Command Prompt, type the following command:

`net use z: \\servername\sharename /user:username password`

Replace `z` with the drive letter you want to map, `servername` with the name of the server, `sharename` with the name of the shared folder, `username` with your username, and `password` with your password.

## Hack #2: Map Network Drives Using PowerShell

If you prefer using PowerShell over Command Prompt, you can also use it to map network drives in Windows 10. You can open PowerShell by pressing the Windows key + X and selecting “Windows PowerShell (Admin).”

Once in PowerShell, type the following command:

`New-PSDrive –Name “Z” –PSProvider FileSystem –Root “\\servername\sharename” -Credential $cred`

Replace `Z` with the drive letter you want to map, `servername` with the name of the server, `sharename` with the name of the shared folder, and `$cred` with your credentials.

## Hack #3: Create a Shortcut to Map Network Drives

To make it even easier to map network drives in Windows 10, you can create a shortcut that will do it for you with just one click. Here’s how:

1. Right-click on your desktop and select “New” > “Shortcut”.
2. In the “Type the location of the item” field, type the following command:

`net use z: \\servername\sharename /user:username password`

3. Replace `z`, `servername`, `sharename`, `username`, and `password` with the corresponding values.
4. Click “Next” and give the shortcut a name.
5. Click “Finish.”

You can now double-click on the shortcut to map the network drive.

## Hack #4: Map Network Drives as Local Drives

If you want to make network drives look and act like local drives, you can map them as local drives in Windows 10. Here’s how:

1. Open File Explorer and click on “This PC.”
2. Click on “Map network drive”.
3. In the “Drive” dropdown, select any available drive letter.
4. In the “Folder” field, type the following:

`\\servername\sharename`

5. Check the box next to “Connect using different credentials.”
6. Click “Finish.”
7. In the “Windows Security” dialog box, enter your credentials and click “OK.”

The network drive will now be mapped as a local drive in File Explorer.

## Hack #5: Map Network Drives Automatically on Startup

If you always use the same network drives and want to have them mapped automatically every time you start your computer, you can use the “Startup” folder in Windows 10. Here’s how:

1. Press the Windows key + R, type “shell:startup,” and press enter.
2. Right-click on an empty space and select “New” > “Shortcut”.
3. In the “Type the location of the item” field, type the following command:

`net use z: \\servername\sharename /user:username password`

4. Replace `z`, `servername`, `sharename`, `username`, and `password` with the corresponding values.
5. Click “Next” and give the shortcut a name.
6. Click “Finish.”

The network drive will now be mapped automatically every time you start your computer.

## Conclusion

With these five mind-blowing hacks, you can become a network drive mapping expert in Windows 10. Whether you prefer using Command Prompt, PowerShell, shortcuts, or the “Startup” folder, there’s a method for everyone. Stop struggling with network drives and start using them like a pro!

{{< youtube LfHtMt1-NwI >}} 



Accessing files from your local hard drive is about the easiest thing you can do on your computer. Taking this to another level and accessing files on hard drives on another system is a bit more complicated. Mapping a network drive is one way of achieving this.
 
Mapping your location will imply that you can create a shortcut to another drive or folder shared on your network. Doing this means that the mapped network drive will display under “This PC” in file explorer.
 
You can map a network drive using the file explorer or from the control panel.
 
## Turn on Network Discovery
 
Before we map a network drive, we need to turn on the “Network Discovery” feature so that it can detect other computers in the network.
 
1. Open Settings and navigate to “Network & Internet -> Sharing Options.”
 
2. Under the “Network Discovery” section, select the “Turn on network discovery” option.
 

 
3. Click “Save Changes.”
 
## Mapping network drive: File Explorer
 
These next steps will help you map a network drive in Windows 10 using File Explorer.
 
1. Open “File Explorer” and click on “This PC” on the right pane.
 
2. Select the computer tab, and in the ribbon menu at the top, click on “Map network drive” and select “Map network drive.”
 
3. Select an alphabet to represent the drive folder from the drive drop-down list. click Browse. (The other computer has to be in the network and have the “Public folder sharing” option turned on before it shows up in the list.)
 
4. In the pop-up displayed, locate the folder you want to map, and hit the OK button after selecting it.
 
5. Once you have confirmed your selection, hit the “Finish” button at the lower-right corner. Note that on the “map network drive” window, you have the option to choose between reconnecting at signin or connecting using different credentials.
 
At the end of this process, the new drive will appear any time you navigate to this PC in File Explorer, and you will be able to access its content from there.
 
## Mapping network drive: Command Prompt
 
You can achieve the same results you did with File Explorer using the command prompt. Just follow the nest steps to map a network drive using your command prompt.
 
1. Open the command prompt. You can do this simply by typing cmd and hitting the Enter key on the Run window.
 
2. On your command prompt, type the following command:
 
Note that “x” represents the name you want to assign to the shared folder.
 
3. You can slightly tweak the above command to insert some additional parameters. You can insert a different set of credentials using the following command:
 
4. After restarting the computer, the drive will no longer exist. To avoid this and make the drive permanent, you can use the command:
 
5. Using the command net use x: /delete will delete the mapped drive, while using the command net use * /delete will delete all mapped drives.
 
## Conclusion
 
Mapping a network drive in Windows 10 is really a basic process that you will find very handy when sharing files on a network. Whatever way you opt for to achieve this should depend on your personal preferences and what you find easier.
 
Afam is a writer with a passion for technology amongst many other fields. Aside from putting pen to paper, he is a passionate soccer lover, a dog breeder and enjoys playing the guitar and piano.
 
Our latest tutorials delivered straight to your inbox




