---
title: "Surprising Method Revealed: Install Microsoft Edge on Linux in Just Minutes!"
ShowToc: true 
date: "2023-04-29"
author: "Joseph Lewis"
---
*****
Surprising Method Revealed: Install Microsoft Edge on Linux in Just Minutes!

For many years, Microsoft's browser, Internet Explorer, was heavily criticized for its lack of standards compliance and security vulnerabilities. In response, Microsoft introduced the Edge browser in 2015, which promised better performance, security, and compatibility with web standards.

While Edge has been available on Windows 10 for several years, it was only recently that Microsoft released a version for Linux. However, installing Edge on Linux requires a bit more effort than just clicking a button. But don't worry; we've got you covered with this simple guide that will help you install Edge on Linux in just minutes.

The first step is to add Microsoft's repository to your system. Open the terminal on your Linux machine and enter the following command:

sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/edge stable main" > /etc/apt/sources.list.d/microsoft-edge-dev.list'

This command will add the Microsoft Edge repository to your system's list of repositories.

Next, import Microsoft's GPG key using the following command:

wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
sudo install -o root -g root -m 644 packages.microsoft.gpg /etc/apt/trusted.gpg.d/
sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/edge stable main" > /etc/apt/sources.list.d/microsoft-edge-dev.list'

Finally, update your system's package list and install Edge using the following commands:

sudo apt update
sudo apt install microsoft-edge-dev

And voila! You now have Microsoft Edge installed on your Linux machine. It's important to note that Edge is only supported on 64-bit versions of Ubuntu, Debian, Fedora, and openSUSE.

In conclusion, while installing Edge on Linux requires a bit more effort than just clicking a button, the process is relatively straightforward, and you can have Edge up and running on your Linux machine in just a few minutes. This move by Microsoft to release Edge for Linux is a welcome one, as it adds more choice and competition to the browser landscape, and should benefit users in the long run.

{{< youtube 6KqqNsnkDlQ >}} 



Microsoft Edge has become one of the fastest, user-friendly and secure browsers for the modern Web. With the implementation of the Chromium engine on the browser, Edge is now stable and comes packed with tools and extensions. In this article, we discuss how to install the Microsoft Edge browser on Linux.
 
## Install Microsoft Edge Using Deb Package
 
The easiest way to set up the Edge browser on your Debian/Debian-based/Ubuntu/Ubuntu-based system is to use the deb package.
 
1. Start by navigating to the Microsoft Edge Insider Channel.
 
2. You can download either the beta version, which is most stable and suitable for most users or the dev channel package, if you would like an early release of the package.
 
3. Once you have the .deb package downloaded to your local machine, right click the package and select “Open with Other Application.”
 
4. This will take you to a window to choose your desired application for opening the file. Select “Software Install.”
 
5. Finally, click on the Install button to start the installation process. You may require an administrative password to install.
 
If you prefer to use the terminal to install the Edge deb package, you can do so with the following commands.
 
Ensure you have .deb package from the resource provided above.
 
Next, open the terminal and navigate to the location of the package.
 
Using the dpkg command, install the package as:
 
Replace the name of the package to match your downloaded package version.
 
## Install Edge Browser on Linux Using Repositories
 
We can also use the Microsoft Edge repositories to install the Edge browser. To do this, start by installing various required dependencies:
 
With the above requirements met, proceed to add the the Microsoft GPG key.
 
Once imported, enable the repository using the command:
 
Finally, update the packages and install the Edge browser using the commands:
 
Note: replace the asterisk with either “beta” or “dev”, allowing you to install either the beta or the dev version of the browser.
 
## Installing Edge Browser on Arch/Manjaro
 
To install the Edge browser in Manjaro, you can use the AUR repositories.
 
To enable AUR repositories on Manjaro Linux:
 
1. Open the application’s menu and search “pamac”. 
 
2. Select “Add/Remove Software”. 
 
3. Open the preferences menu using the hamburger icon on the top-right corner.
 
4. In the preferences window, navigate to the AUR option and toggle the icon to enable AUR repositories.
 
5. Close the preferences window and search for “microsoft-edge-dev-bin”.
 
6. Select the entry that show up and click “Install”. 
 
This should install the Microsoft Edge browser on Manjaro.
 
For Arch and other Arch-based distro, you can install the Edge browser with yay
 
1. Open a terminal and type:
 
2. Once yay is installed, enter the command to install Microsoft Edge:
 
## Installing Microsoft Edge on Fedora/OpenSUSE
 
To install Microsoft Edge on Fedora or OpenSUSE, use the provided RPM packages. 
 
1. Start by navigating to Microsoft Edge Insider and download the RPM file for your desired channel.
 
2. Next, launch the terminal and navigate to the location of the downloaded RPM file.
 
3. Finally, use the command:
 
Note: replace the asterisk with the version of the downloaded RPM package. 
 
## Launching the Edge Browser
 
To launch the browser, launch the activities search bar and type edge.
 
Click on the Edge icon and launch the browser.
 
You can also launch it by typing the command microsoft-edge in the terminal.
 
## Frequently Asked Questions
 
### Is Microsoft Edge free?
 
Yes, Microsoft Edge is a free browser. 
 
### 2. How is Microsoft Edge different from Firefox?
 
Although not very noticeable to your average user, Firefox comes with additional tools compared to the Microsoft Edge browser, such as Eye Dropper, Web Developer Extensions and more. However, due to the implementation of the Chromium platform, MS Edge provides an advantage over Firefox with support for Chrome extensions.
 
### 3. How frequently will I receive browser updates?
 
Depending on the channel from which you installed Microsoft Edge, you are likely to get updates as frequently as every week for the Dev channel and every six weeks for the Beta channel.
 
## Wrapping Up
 
In this guide, we discussed various methods to set up the Microsoft Edge browser. Once set up, you can add browser extensions or import bookmarks, history and passwords from other Chromium-based browsers.  
 
John is a technical writer at MTE, when is not busy writing tech tutorials, he is staring at the screen trying to debug code.
 
Our latest tutorials delivered straight to your inbox




