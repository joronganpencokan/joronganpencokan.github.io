---
title: "You Won't Believe How Easy It Is To Map A Webdav Drive In Windows - Let Us Show You How!"
ShowToc: true 
date: "2022-12-16"
author: "Cyril Carruth"
---
*****
---
title: "You Won't Believe How Easy It Is To Map A Webdav Drive In Windows - Let Us Show You How!"
date: 2021-10-01T16:31:26+08:00
draft: false
tags: ["windows", "webdav", "drive mapping"]
---

As more and more businesses move towards cloud-based storage solutions, WebDAV has become an increasingly popular way to access files and folders remotely. WebDAV stands for Web Distributed Authoring and Versioning, and it’s a protocol used to access shared files and manage them over the Internet. One of the more common tasks you may need to perform when using WebDAV is to map a network drive to your PC. Fortunately, this is a quick and easy process in Windows, and we're going to show you how to do it.

### Step 1: Open the Explorer window

The first step is to open an Explorer window. You can use any folder you like for this. In this example, we'll use the Documents folder.

### Step 2: Click on the Computer tab

Click on the "Computer" tab located in the top left corner of the window. A drop-down menu will appear.

### Step 3: Select "Map network drive" from the drop-down menu

Next, select "Map network drive" from the drop-down menu. This will open the "Map Network Drive" dialog box.

### Step 4: Choose a drive letter and enter the WebDAV URL

In the "Map Network Drive" dialog box, you'll be prompted to choose a drive letter to assign to the WebDAV folder. Click on the drop-down menu under "Drive" and select any letter you like. Then, in the "Folder" field, enter the URL of the WebDAV folder you want to map. For example, if the URL is "https://webdav.example.com/files/", enter "https://webdav.example.com/files/" in the "Folder" field.

### Step 5: Check "Reconnect at sign-in" and "Connect using different credentials" (Optional)

If you want the mapped drive to be reconnected automatically each time you sign in to Windows, check the "Reconnect at sign-in" box. You'll also have the option to connect using different credentials if necessary.

### Step 6: Click Finish

Once you've entered the required information, click the Finish button to complete the mapping process.

### Conclusion

Mapping a WebDAV drive in Windows is a quick and easy process that can be accomplished in just a few steps. By following our guide, you'll be able to quickly access your WebDAV files and folders from your PC. So what are you waiting for? Give it a try today!

{{< youtube izJH7fGCmmE >}} 



Web Distributed Authoring and Versioning (WebDAV) is an HTTP extension that provides a collaborative way of editing and managing your files on a remote web server. Here we will show you how to map a WebDAV drive in Windows so you can access your remote files directly in File Explorer.
 
In order to connect to the WebDAV directory in Windows, you’ll need the WebDAV site URL, your WebDAV account login details, and a name for the shortcut or connection. All three allow you to map WebDAV by mounting its folder as a mapped drive so you can view, edit, or delete files from the remote web server using your computer.
 
## How to Map a WebDAV Drive in Windows
 
- Open File Explorer on your computer. Right click “This PC” and select “Show more options.” If you’re using Windows 10, you won’t see a “Show more options” option. Simply skip to Step 2.

 
- Click “Map network drive…”

 
Alternately, you can also use the “Map network drive” drop-down box in the Computer tab of File Explorer. Select “Map network drive” from the list. This is only available in Windows 10.
 
- In the new dialog box, enter the drive letter you want to map to and the folder where you’ll add or edit WebDAV files on your local computer.

 
- If you click the “Browse” option next to the folder mention and get the “Network discovery is turned off. Network computers and devices are not visible…” message, this means you need to enable network discovery in Network and Sharing Center.

 
Change the setting by going to Start and typing “control panel.” Select Control Panel when it appears.
 
Select “Network & Sharing Center.”
 
Select “Change advanced sharing settings” on the left.
 
Turn on Network Discovery and press “Save Changes.”
 
- Check the “Reconnect at sign-in” and “Connect using different credentials” boxes. Checking the “Reconnect at sign-in” box allows the WebDAV connection to be restored when you reboot your computer.

 
- Click the link “Connect to a web site that you can use to store your documents and pictures.”

 
- Click Next.Now click “Choose a custom network location” and click Next.Enter your domain URL in the Internet or Network address field with the WebDAV directory at the end.Type your WebDAV username and password.Click OK. The “Type a name for this network location” data is already filled in but can be changed.Click Next and then click Finish.

 
In File Explorer, the WebDAV folder will be displayed as a mapped drive. You can now add, edit, or delete files or directories through File Explorer.
 
## What to Do When You Cannot Connect to WebDAV Directory
 
Note: should you find difficulties connecting to the WebDAV directory, update the Basic Authentication Level in Windows Registry.
 
- Right-click Start and select Run.Type regedit and press Enter to open Windows Registry Editor.Go to the directory path:

 
- Find “BasicAuthLevel” value. By default, the value is set at 2, but if it’s not, right-click and select Modify and then change to 2.

 
## What to Do If You Can’t Access Your WebDAV Folder?
 
Even if you were able to successfully map a WebDAV drive in Windows, it doesn’t mean you’ll be able to access content within it. The most common cause is the folder is stored on a server using an older version of Windows. 
 
This also happens if you’re not using the latest version of Windows. For example, if you used Windows XP and the folder contains more than 1,000 files, you may not be able to see the file you need.
 
Another issue is experienced when you restart your computer and are not automatically reconnected. This usually means the WebClient service is either disabled or set to Manual. Here’s how to change that.
 
- Go to Start, search for Services, and select the result. Then, scroll until you find WebClient, right-click it and choose “Properties.”

 
- Set the Startup type to “Automatic” and press Apply to apply the changes. You can then click OK and close the Services window.

 
## Frequently Asked Questions
 
Image credit: Sunrise King via Unsplash
 
### Where can I find my WebDAV URL?
 
You’ll typically find the URL in your WebDAV dashboard. If you don’t see it, you may need to check any available documentation or contact the service provider directly.
 
### If I change my password, will I need to remap the drive?
 
Yes. Since the credentials have changed, you’ll need to delete the previously mapped drive and reconnect. Simply follow the same process using your new password.
 
### Can all user accounts access the mapped drive?
 
No. The drive is only mapped under the user account that created it. However, the PC’s administrator will be able to see it. In order for others to see it, they’ll need to map the drive under their account.
 
### If I delete a mapped drive, does that affect the folder itself?
 
Deleting the mapped drive won’t have any affect on the actual drive or folder. This only breaks the link between your Windows PC and the remote drive. All your files will still exist in the original location.
 
### Are mapped WebDAV drives secure?
 
These are only as secure as your PC. Protect your remote files by always logging out of your system before walking away from your computer. Also, use a strong password to protect your Windows account. If there are multiple users on the PC, don’t let others use your account.
 
Also, as a standard rule of thumb, always use some type of antivirus. Once a virus infects your PC, all files, folders, and drives are at risk. For many users, the pre-installed Windows Defender may be enough. If you suspect you do have a virus, you may be able to remove it without using an antivirus app.
 
Crystal Crowder has spent over 15 years working in the tech industry, first as an IT technician and then as a writer.  She works to help teach others how to get the most from their devices, systems, and apps. She stays on top of the latest trends and is always finding solutions to common tech problems.
 
Our latest tutorials delivered straight to your inbox




