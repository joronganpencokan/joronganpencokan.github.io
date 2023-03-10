---
title: "Secret Hack Revealed: Move Your Favorite PC Games Between Hard Drives Effortlessly!"
ShowToc: true 
date: "2023-03-17"
author: "Edwin Vincent"
---
*****
Secret Hack Revealed: Move Your Favorite PC Games Between Hard Drives Effortlessly!

Have you ever had to uninstall some of your favorite PC games just because you ran out of storage space? It is frustrating to let go of games that you love and have invested a lot of time and effort in achieving milestones on. Fortunately, you don't have to do that anymore! In this article, we will show you how to move your favorite PC games between hard drives seamlessly.

Before we dive into the hack, we must first understand how games are installed on our computers. When you install a game, it not only installs the game files but also creates an entry in the Windows Registry that links to the game's location on your hard drive. It is this entry that tells Windows where to look when you click on a game shortcut to launch it.

Now, imagine if you could change that location without uninstalling the game. In other words, you want to shift the game's entire directory from one hard drive to another without breaking the link to the Registry.

The good news is that this is possible, and you can do it in three easy steps.

Step 1: Copy the Game Folder

The first thing you need to do is copy the entire game folder from its current location to the new hard drive where you want to move it. To simply copy the folder, open a window of the source drive directory where your game is installed, like "C:\Program Files (x86)\Steam\steamapps\common" and then open a second window of the target location where you want to move the game. Then drag the game folder from the first window to the second window.

It's important that you do not delete the folder on the original hard drive until the entire copy is complete.

Step 2: Create a Symbolic Link

Next, you need to create a symbolic link between the old game location (the one you just copied) and the new game location. This way, when you launch the game through its shortcut, the Registry will redirect to the new folder automatically.

To create this link, open the Command Prompt with administrator privileges and enter the following command:
mklink /D "C:\OldGameLocation" "D:\NewGameLocation"

Do note that "C:\OldGameLocation" is the old location of the game folder that you copied, while "D:\NewGameLocation" is the new location where you want to move the game. Ensure that the folders are typed correctly.

Step 3: Verify the Game Launches

Now that you have created the link, the game should launch without any issues. Test this by double-clicking on the game's desktop shortcut or by launching it from your Steam library.

If the game launches successfully, congratulations! You have successfully moved your PC game from one hard drive to another without uninstalling it.

In conclusion, this hack can be a lifesaver for those who love to play games but are always struggling with storage space. Just remember to create a symbolic link between the old game location and the new game location, and you won't lose any game progress or achievements. So go ahead and transfer those games to your heart's content without any worries. Happy gaming!

{{< youtube AOHI9U8phDw >}} 



It’s a common scenario. You’ve just bought yourself a swanky new hard drive (SSD, I’m guessing) and want to transfer your biggest games to it so you can say goodbye forever to horrendous loading times. But uninstalling and reinstalling the games again could take hours, especially when you take into account the fact that you’ll probably need to re-download them as well.
 
The solution is to move your installed PC games over directly instead of reinstalling them. Sadly, it’s not quite as simple as just copying and pasting them where you want, but it isn’t too much more complicated either.
 
## The Manual Method
 
Whether you’re looking to move a game that’s on Steam, Origin or Uplay, you can do it without third-party software. We’ll use Steam as an example because it’s the most popular platform, but the same principle applies across other platforms as well.
 
First, go to the game’s installation directory and cut and paste it to where you want it on the new hard drive. (If you’re pasting a Steam game, make sure it’s in the folders “steamapps/common,” as Steam automatically looks for those subdirectories. So paste the games to, for example, “My Games/steamapps/common” or “Steam Games/steamapps/common.”)
 

 
Once you’ve done that, uninstall the game from your PC using Steam by navigating to it in your Steam library, right-clicking it and clicking “Delete Local Content.”
 
Go to your Steam download settings, (In Steam, click Steam at the top left -> Settings -> Downloads.) click “Steam Library Folders -> Add Library Folder,” then select the directory where you pasted your game. (Don’t include the “steamapps/common” part here, as Steam will apply that automatically.)
 
Close the Settings window, go to your (uninstalled) game in your Steam library, then click install and select the new install directory you just added to Steam. Because all the game files are there, Steam will skip the download process and get on with installing your game to the new drive.
 
The exact details will vary, but you can do pretty much the same thing – copy and paste the game, uninstall it, then reinstall it without re-downloading – on Uplay, Origin, etc.
 
## Use Steam Mover
 
Alternatively, you can use an extremely lightweight but useful little tool called Steam Mover. The way Steam Mover works is by moving all the game files to a location of your choice while leaving a Junction Point in the original location. This means you shouldn’t delete the game folders that get left at the game’s original location, as that’ll delete the junction point, and Steam won’t be able to find them when you try and run them. Despite the name, you can also use Steam Mover for Origin, GOG, Uplay or other games – and any other programs and files that you want for that matter!
 
You can download Steam Mover here. (You need to scroll down quite a bit to the ‘Download’ subhead.) Once you’ve done that, extract and install it wherever you like.
 
Open Steam Mover, and it should automatically detect and list all the Steam games in your library. If not, click the three dots next to “Steam Apps Common Folder” to manually find your Steam library on your hard drive, then select it and click “Refresh.”
 
Next, click the three dots under “Alternative Folder” in Steam Mover to select the location that you want to move your Steam games to (presumably, somewhere on your swanky new hard drive).
 
Next, with your games listed, select all the ones you want to move by holding Ctrl while clicking each one so they’re all highlighted. Once you’ve done that, click the blue, right-pointing arrow at the bottom of the window to move all your selected games to the new drive. A command prompt window will show up, speeding through all the files as it moves them. When the command prompt closes, and you see the blue arrows for each game in the right-hand column, the job is complete.
 
## Conclusion
 
Being able to move your installed PC games easily between hard drives is a handy skill, not only because it saves time, but because it potentially saves you gigabytes upon gigabytes of frustrating re-downloads. If you have caps on your downloads, or your connection gets throttled if you do too much downloading in a short space of time, then this could save you a lot of headaches!
 
Content Manager at Make Tech Easier. Enjoys Android, Windows, and tinkering with retro console emulation to breaking point.
 
Our latest tutorials delivered straight to your inbox




