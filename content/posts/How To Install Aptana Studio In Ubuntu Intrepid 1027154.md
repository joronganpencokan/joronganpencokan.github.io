---
title: "Revolutionize Your Coding Game with This Simple Aptana Studio Installation Guide for Ubuntu Intrepid"
ShowToc: true 
date: "2023-04-25"
author: "Mathew Colon"
---
*****
Revolutionize Your Coding Game with This Simple Aptana Studio Installation Guide for Ubuntu Intrepid

If you're a developer and use Ubuntu Intrepid, you may be looking for a more efficient coding environment. Aptana Studio is an integrated development environment (IDE) that combines multiple tools in one, making it easier to develop web applications. This guide will walk you through the process of installing Aptana Studio on your Ubuntu Intrepid.

Step 1: Download Aptana Studio

Start by visiting the Aptana Studio website (www.aptana.com). Go to the download section and choose the appropriate version for your operating system. In this case, select the Linux 32-bit version.

Step 2: Extract the Package

Now that the package has been downloaded, extract it to your desired location. Simply right-click on the downloaded package and select "Extract Here". You can also extract it via the terminal using the following command:

tar -xzf Aptana_Studio_x.x.x_Setup_Linux_x86.tar.gz

Replace "x.x.x" with the version number that you downloaded.

Step 3: Install Java Runtime Environment (JRE)

You need Java Runtime Environment (JRE) installed on your system to run Aptana Studio. To install JRE, run the following command in the terminal:

sudo apt-get install openjdk-6-jre

Step 4: Set the JAVA_HOME Environment Variable

After installing JRE, you need to set the JAVA_HOME environment variable. This variable is used to point Aptana Studio to the correct directory where the JRE is installed. To set the JAVA_HOME environment variable, run the following command in the terminal:

sudo gedit /etc/environment

This will open the environment file in the text editor. Add the following line to the end of the file:

JAVA_HOME="/usr/lib/jvm/java-6-openjdk/"

Save and close the file. To apply the changes, run the following command in the terminal:

source /etc/environment

Step 5: Launch Aptana Studio

Now that everything is set up, launch Aptana Studio from the extracted folder. Navigate to the folder where you extracted the package and double-click on the AptanaStudio3 executable file.

Step 6: Configure Aptana Studio for First Use

Once Aptana Studio launches, you need to configure it for first use. You will be asked to enter your Name and Email. If you want to skip this step, just check the "Skip" option.

Next, you need to select the default workspace location. This is the directory where all your projects will be saved. You can choose the default workspace or create a new one.

Congratulations! You now have Aptana Studio up and running on your Ubuntu Intrepid system. Use this guide as a reference and start exploring the features of this powerful IDE to revolutionize your coding game. Happy developing!


For those who have read my review of Aptana and wish to install it in Ubuntu 8.10, here is how you can do so. While the installation is not as straightforward as it should be, the overall process is not that difficult either.
 
The instruction below is meant for 32-bit machine. If you are using a 64 bit machine, you’ll have to install Eclipse with the Aptana plugin.
 
1. Download Aptana for Linux
 
2. Unzip the Aptana tar file to your Home folder.
 
3. Install the dependencies:
 
4. Open up a text editor and paste the following lines to the file.
 
Change the filepath to the location where you place the Aptana folder. Save the file as “runAptana.sh” in the Aptana folder.
 
5. Right-click on the runAptana.sh file and select Properties. Go to the Permissions tab. Check the box “Allow executing file as program”
 
That’s it. Whenever you want to run Aptana, simply double click on the runAptana.sh file.
 
## Creating Desktop and Menubar shortcut (Optional)
 
You can also create a shortcut on your desktop or the menubar so that you can easily access it when you want to use it.
 
1. Right-click on the menubar and select “Edit Menus”.
 
2. On the left pane, scroll down till you find the “Programming” entry. Click on it.
 
3. On the right, click on the “New Item” button. Enter the following:
 
4. Close all the windows. You should be able to find the Aptana launcher in “Applications -> Programming -> Aptana”.
 
To create a desktop shortcut, simply drag the Aptana launcher from the menubar to the desktop. If you are using any dock applications, you can also drag and drop the launcher to the dock.
 
Didn’t I say it is easy?
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




