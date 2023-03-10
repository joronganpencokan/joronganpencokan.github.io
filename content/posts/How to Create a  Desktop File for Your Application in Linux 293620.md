---
title: "Revolutionize Your Linux Experience: Learn How To Easily Create Desktop Files For Your Applications!"
ShowToc: true 
date: "2023-02-23"
author: "Benny Mazzotta"
---
*****
Revolutionize Your Linux Experience: Learn How To Easily Create Desktop Files For Your Applications!

As a Linux user, you know that the operating system provides you great control and flexibility to customize your experience. However, sometimes you might find yourself struggling to locate a specific application in the vast directory of files or remembering the exact command to open it. But, what if you could create desktop files for your frequently used applications and access them with just a single click?

Desktop files are shortcut files that provide a simple and direct way to launch applications from the Linux desktop environment. With the right knowledge, you can create them in no time and drastically improve your Linux experience. In this article, we will show you how to create desktop files for your applications quickly and seamlessly.

Step 1: Locate The Executable File

To create a desktop file, you'll first need to locate the executable file of the application you want to create a shortcut for. Whether the app is installed via a package manager or was installed from a source, you can find the executable file in the bin directory of the installation.

For example, if you want to create a desktop file for the web browser, Firefox, then type the following command in the terminal to locate its executable file:

$ which firefox

This command will display the file path to the Firefox executable file. Note this path, as we will need it in the next step.

Step 2: Create The Desktop File

Now that we have the path to the executable file, we can create a desktop file using a simple text editor like Gedit or Nano. Here's the basic format:

[Desktop Entry]
Type=Application
Name=<The name of the application as you want it to appear on your desktop>
Exec=<The file path to the application executable>
Icon=<The path to the application icon>
Comment=<A brief description of the application/use case>

Save this file with a .desktop extension, like firefox.desktop, in the directory ~/.local/share/applications/ for the shortcut to be available only for the current user, or /usr/share/applications/ if it's supposed to be a global shortcut.

Note that the Icon field is optional, but it's highly recommended as it provides a better visual representation of the app on the desktop. You can use an existing icon from the system or search online for appropriate ones.

Here is an example of how the desktop file for Firefox should look like:

[Desktop Entry]
Type=Application
Name=Firefox
Exec=/usr/bin/firefox
Icon=/usr/share/icons/hicolor/32x32/apps/firefox.png
Comment=Browse the web with Firefox

Step 3: Enjoy Your New Shortcut!

Once the desktop file is created, you can try it out by searching for the application name in the applications menu, dragging it to the desktop, or adding it to your favorites or dock. The next time you want to use the application, click on the new shortcut, and it will open without any extra effort.

Final Words

Creating desktop files is a simple yet powerful way to streamline your experience in Linux. By knowing how to create them, you can save time and effort, and make your workflow more efficient. Try creating desktop files for your frequently used apps, and see how they improve your Linux experience. Happy computing!

{{< youtube sSWH_G4f-h8 >}} 



A .desktop file is simply a shortcut that is used to launch applications in Linux. Without the .desktop file, your application won’t show up in the Applications menu and can’t be launched with third-party launchers such as Ulauncher and Albert.
 
Most applications, when installed, will create the .desktop files automatically and place themselves in the “Application” menu for quick access. However, if you compile a program from source or download an app in archive format, this may not be the case, and you may have to open the terminal to execute the binary every time you want to use it. Obviously, this can become a very tedious and troublesome step. This tutorial shows how you can create a .desktop file for any application you use that can be launched from the “Application” menu.
 
## How to Create Desktop Launchers
 
A .desktop file is a simple text file that holds information about a program. It is usually placed in “~/.local/share/applications” or “/usr/share/applications/,” depending on whether you want the launcher to be accessible for your local account onlly or for everyone. If you navigate to either directory in your File Manager, you will see quite a few .desktop files that correspond with the installed apps on your computer.
 
For demonstration purposes, we are creating a .desktop file for Super Tux Kart, a kart racing game we like to play sometimes. A version is available in the Ubuntu repos, but this is often behind the latest stable version.
 
The only way to get the latest and greatest release is by downloading a tar archive, extracting it and executing a file which will launch the game.
 
You can follow along with whichever program you want to create a launcher for, and it should work the same way.
 
Note: the following steps assume you have the archive for the program you want to create a launcher for in your “Downloads” folder.
 
- Navigate to the directory where the archive is stored, right-click it and select “Extract here.”

 
- Once the extraction is complete, change to the newly created folder and find the executable. Right-click it and select “Run as a Program” to launch the program just to ensure it is working.

 
- In some cases, you won’t see the “Run” option in the menu, often because the executable is a .text file. You can get around this by executing it via the terminal.

 
- If you’ve confirmed that the application works when you launch it, you can exit it. Launch your text editor and paste the following into the empty text file:

 
Note: You’ll need to change the “Exec” field to the path to the executable and “Name” field to the name of the application. Most programs provide an icon somewhere in the archive, so don’t forget to include that as well. In our case, the launcher file for Super Tux Kart looks like the following image.
 
- Save the file in the “~/.local/share/applications” folder as “application-name.desktop”. The “.local” folder is a hidden folder in your “Home” directory and “Show Hidden Files” mode will have to be enabled for you to view it. If you want it to be globally accessible, run the following command in the terminal:

 
Note: don’t forget to change <application-name.desktop> to the actual name of the .desktop file.
 
- Once done, open the “Applications” menu on your desktop to find the .desktop app.

 
The method described here should work on all mainstream Linux-based operating systems. Here’s another screenshot showing Super Tux Kart in Xubuntu’s application launcher (XFCE).
 
## How to Copy .Desktop Files
 
As discussed above, you can obtain a .desktop file from a program that you have installed through a repository. This is helpful if you want to create a custom .desktop file as a way of fixing a broken package in Ubuntu.
 
For the most part, each Linux distribution is largely similar in its structure, so while this section will heavily focus on Ubuntu 22.04, you can still use these instructions in your favorite desktop environment.
 
- To start, open a File Manager from your desktop. In this case, we are opening Nautilus, as it is the default for Ubuntu.

 
- Press the “Other Locations” entry in Nautilus’s left side bar.

 
- This brings up a list of all the system locations in your machine. Press “Computer.”

 
- Go to “/usr/share/applications.” This directory contains the .desktop files that your desktop manager uses to create its Application Menu.

 
- Copy the application you want to create a shortcut to. For instance, right-click on “firefox-esr.desktop” and select “Copy.”

 
- Go back to your desktop and place the .desktop file by right-clicking and selecting “Paste.”

 
- Right-click on your .desktop file and select “Allow Launching.” Doing this will set the permission bits so that your desktop environment can use this file to launch your program.

 
## How to Create .Desktop Files With a Third-Party Program
 
Aside from editing and copying .desktop files, it is also possible to create shortcuts in Linux through a Graphical User Interface (GUI) program. This is useful if you are not comfortable with editing configuration files.
 
Unlike the previous methods, this will require you to install a program like Arronax, which may not be present in your distribution’s repository. Despite that, it is still possible to use it by obtaining a copy from the developer’s website. To install the GUI in Ubuntu, follow the below instructions.
 
- Add a third-party repository by running the following command:

 
- Iinstall the GUI program by running the following command:

 
- On the other hand, if you are installing it through a tarball, you need to unpack the archive using tar:

 
- Run Arronax by either running the command below or typing “arronax” while in the Application Menu. This will bring up a window where you can create and save .desktop files.

 
- To create your first shortcut using Arronax, click the “New” icon in Arronax’s Menu Bar to create a template that you can use for your shortcut.Provide the shortcut’s name and a file path to your program. For example, we are creating a .desktop file for Firefox by typing “Firefox” in the “Title” field and /bin/firefox-esr in the “Command” field.

 
- Press the green arrow in Arronax’s Menu Bar to save the shortcut.

 
- In this example, we’re saving it as “Firefox.desktop” in our desktop directory.

 
- Right-click this .desktop file and select “Allow Launching” to set the permission bits for it, as shown above.

 
## Frequently Asked Questions
 
Image credit: Charles-Adrien Fournier via Unsplash All screenshots by Ramces Red.
 
### Is it possible to use a .desktop file even if I am using a window manager?
 
No, a .desktop file will not work on most window managers, as it lacks the necessary support for the “XDG Menu” specification. While it is possible to create a .desktop file in a window manager, it will not show up as a desktop shortcut. One way to recreate this mechanism is by using shell scripts alongside the Simple X Hotkey Daemon.
 
### Is it possible to create a .desktop file for CLI and TUI applications using Arronax?
 
Yes! You can easily create a .desktop file for a program that runs in the terminal, which is useful if you are already using TUI programs and want to have a quick way to access them.
 
To do this using Arronax, create a new .desktop shortcut by providing both a “Title” and a “Command,” then toggle the “Run in Terminal” option and save the new shortcut.
 
### Is it possible to hide a desktop shortcut from an Application Menu?
 
Yes! It is possible to modify a .desktop file to not show on your Applications Menu by adding a single line of code in the file that you want to edit. For example, if you want to hide Firefox from your Applications Menu, open the “firefox-esr.desktop” file in “/usr/share/applications”. From there, add Hidden=true at the end of the file, then restart your computer to apply the changes.
 
Ramces is a technology writer that lived with computers all his life. A prolific reader and a student of Anthropology, he is an eccentric character that writes articles about Linux and anything *nix.
 
Our latest tutorials delivered straight to your inbox




