---
title: "Unlock the Secret to Lightning Fast Computer Speed with this One Simple Trick for Increasing Icon Cache in Windows!"
ShowToc: true 
date: "2023-01-10"
author: "Mary Mccloskey"
---
*****
---
title: Unlock the Secret to Lightning Fast Computer Speed with this One Simple Trick for Increasing Icon Cache in Windows!
date: 2021-11-19
description: Learn how to increase your computer speed by optimizing your icon cache in Windows.
---
Do you often find your computer running sluggishly? Have you ever wondered why your desktop icons take forever to load? If so, it's time to unlock the secret to lightning-fast computer speed with this one simple trick for increasing icon cache in Windows!

Icon cache is a small database in Windows that stores images of icons, thumbnails, and other graphical elements. When you open a file or a folder on your computer, Windows fetches the corresponding icon from the icon cache. The icon cache is designed to speed up the process by keeping a copy of the icon close at hand, so it doesn't have to load the icon every time you access it.

However, over time, the icon cache can become bogged down with obsolete or corrupted data, slowing down your computer in the process. Fortunately, you can increase your computer speed by optimizing your icon cache in Windows using this simple trick.

Step 1: Clear the Icon Cache
The first step in optimizing your icon cache is to clear it of all the old and unnecessary icons. To do this, follow these simple steps:

1. Open File Explorer and navigate to your Local disk (C:).
2. In the search box, type "Disk Cleanup" and click on the Disk Cleanup app from the results.
3. Select "Temporary files" and "Thumbnails" checkboxes.
4. Click "Clean up system files" and let it finish the process.

This will clear the icon cache and temporary files, freeing up space on your computer and improving its performance.

Step 2: Increase the Icon Cache Size
Once you've cleared the icon cache, the next step is to increase its size to ensure that your computer has enough resources to load icons quickly. Follow these simple steps to increase the icon cache size:

1. Press "Windows + R" and type "regedit."
2. Navigate to HKEY_LOCAL_MACHINE > SOFTWARE > Microsoft > Windows > CurrentVersion > Explorer.
3. Right-click anywhere in the right-hand panel and select "New" > DWORD (32-bit) Value.
4. Name the new value as "Max Cached Icons".
5. Double-click on the new value and change the Base to Decimal.
6. Enter a value between 4096 to 8192 in the Value data field to increase the icon cache size. The default value is 500. We suggest entering a value between 4096 to 8192.

By increasing the icon cache size, you're allowing Windows to store more icons, which means it can access them more quickly, resulting in faster loading times and improved overall computer speed.

In conclusion, by optimizing your icon cache, you can unlock the secret to lightning-fast computer speed by using this one simple trick. Clearing the cache and increasing its size can help reduce the load on your computer's resources and improve its performance. Give it a try today, and you'll be amazed at the difference it makes!

{{< youtube H9hNCy6z1Zs >}} 



For most media files like videos, photos, etc., and documents like PDFs, Windows tries to show you a preview of the file as a thumbnail instead of a generic icon. This helps you to quickly recognize the files without actually opening each and every file.
 
However, the downside of this approach is that your File Explorer may be slow to load all the thumbnails or may even freeze at times. Of course, this all depends on how many files are there in a given folder. In those situations you can do two things: rebuild the icon cache or increase the icon cache so that Windows can store more thumbnails without removing the old ones.
 
When you allow Windows to store more thumbnails by increasing the icon cache, the file-loading process in File Explorer will be much faster, and you can view all the file previews without waiting for the infamous green loading bar.
 
Note: I’m showing this in Windows 10; the procedure is the same for Windows 7 and 8.
 
## Increase Icon Cache in Windows
 
By default, the icon cache size in Windows is 500KB. This is good enough if you don’t have a lot of media files and documents. When dealing with a lot of media files, you can easily increase the icon cache size with a simple registry edit. To start, search for regedit in the Start menu and open it. If you are using the system as a standard user, then right-click on “Regedit” and select the option “Run as Administrator.”
 

 
After opening the Windows Registry Editor, navigate to the following location. If you are using Windows 10, then simply copy the below path, paste it in the address bar and press the Enter button.
 
Once you open the required key, you need to create a new String value. To do that, right-click on the right panel and select the “New” option and then “String Value.”
 
Name the new value as “Max Cached Icons” and press the enter button to save the changes.
 
Now, double-click on the newly-created value to set the value data. In the “Edit String” window, enter the cache size in KiloBytes. For instance, if you want the cache size to be 4MB, enter the value data as 4096 and click on the “OK” button. If you want the cache size to be 8MB, then enter 8192. However, don’t try to enter several MBs worth of cache size. In fact, after 8MB all you get is diminishing returns.
 
Once you are done editing, this is how it looks like in the registry editor.
 
Just close the Registry Editor and restart your system to make the changes take effect. You should now see that the File Explorer is loading fast with necessary file previews.
 
If you ever want to revert back, simply change the value data to 500 or delete the newly created value.
 
Do comment below sharing your thoughts and experiences about using the above to increase the icon cache in Windows.
 
Vamsi is a tech and WordPress geek who enjoys writing how-to guides and messing with his computer and software in general. When not writing for MTE, he writes for he shares tips, tricks, and lifehacks on his own blog Stugon.
 
Our latest tutorials delivered straight to your inbox




