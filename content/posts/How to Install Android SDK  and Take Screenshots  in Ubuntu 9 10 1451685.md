---
title: "You Won't Believe How Easy It Is To Install Android SDK And Take Screenshots In Ubuntu 9.10 - Click Now To Learn The Trick!"
ShowToc: true 
date: "2023-01-19"
author: "Vicki Saucedo"
---
*****
You Won't Believe How Easy It Is To Install Android SDK And Take Screenshots In Ubuntu 9.10 - Click Now To Learn The Trick!

If you are an Ubuntu 9.10 user, you might be wondering how you can install Android SDK and take screenshots easily. Thankfully, the process is not as complicated as you might think. In fact, it's pretty easy once you know the trick.

Before we get started, make sure that your Ubuntu 9.10 computer has an active internet connection. Also, make sure that your device is connected to your computer via USB.

Step 1: Install JDK

To install Android SDK, you will first need to install JDK. Open up a terminal window and type the following command to install JDK:

sudo apt-get install sun-java6-jdk

Step 2: Download and Extract Android SDK

Next, you need to download Android SDK. To do this, go to the Android Developer website and download the appropriate version of Android SDK for your operating system.

Once you have downloaded Android SDK, extract the contents of the zipped file to a suitable directory. For example, you could extract the contents to /opt/android-sdk-linux.

Step 3: Install Necessary Packages

Now that you have Android SDK installed and extracted to an appropriate directory, you need to install some necessary packages. Open up a terminal window and type the following command:

sudo apt-get install ia32-libs lib32ncurses5 lib32stdc++6

This command will install the necessary packages required to run Android SDK on your Ubuntu 9.10 computer.

Step 4: Add Android SDK to Your PATH

In order to use Android SDK from the command line, you need to add its location to your PATH environment variable. To do this, open up the .bashrc file in your home directory and add the following line:

export PATH=$PATH:/opt/android-sdk-linux/tools:/opt/android-sdk-linux/platform-tools

Step 5: Enable USB Debugging on Your Device

Before you can take screenshots from your device, you need to enable USB debugging. To do this, go to Settings > Applications > Development and check the USB debugging option.

Step 6: Take a Screenshot

Now that everything is set up, you can take a screenshot of your device by running the following command:

adb shell screencap /sdcard/screenshot.png

This command will take a screenshot of your device and save it to the /sdcard/screenshot.png file on your device.

Step 7: Save the Screenshot to Your Computer

To save the screenshot to your computer, run the following command:

adb pull /sdcard/screenshot.png ~/Desktop

This command will download the screenshot from your device and save it to your computer's desktop.

In conclusion, installing Android SDK and taking screenshots on Ubuntu 9.10 is not as complicated as you might think. By following these simple steps, you can easily get started with Android development and take screenshots of your devices for testing and documentation purposes. So what are you waiting for? Click now to learn the trick and get started with Android development on Ubuntu 9.10!

{{< youtube 3BZW0x7J190 >}} 



If you are an Android developer, looking to root your Android phone, or just a blogger who wants to take screenshots of your latest Nexus One phone, you will need to install Android SDK in your computer. I know that it is kind of troublesome to download/install the SDK just to take screenshots in your phone, but luckily it can be done easily. This article will show you the way to install Android SDK and take screenshots in Ubuntu 9.10 Karmic.

First, go to the Android website and download the SDK. Make sure you choose the Linux version.
 

 
Extract the downloaded file to your home folder. You should see a folder with the name “android-sdk-linux_86”.
 
Open your .bashrc file and add the filepath to the end of the file. In a terminal, type the following:
 
Add the following line to the end of the file:
 
Replace <your_sdk_dir> with the actual filepath of the SDK folder. If you have extracted the file to your home folder, it should be something like /home/your_username/android_sdk_linux_86/
 
Next you need to install Ecplise. For Ubuntu 9.10 users, the latest version of Eclipse (Eclipse Classic 3.5.1) is already included in the repository, so you can easily install via the command:
 
Once the installation is completed, open Eclipse (Application -> Programming -> Eclipse)
 
On the menubar, click on Help -> Install new software
 


 
At the Work with field, enter http://download.eclipse.org/releases/galileo and click Add.
 
You will see that there are several software now available for installation. Ignore them.
 
Next, erase away the entry in the Work With field and add https://dl-ssl.google.com/android/eclipse/. Click Add.
 
Check all the entries in the bottom pane and click Next to install.
 
Once the installation is done, restart Eclipse.
 
Go to Windows -> Preferences. On the left, select the Android entry.
 
Enter the Android filepath in the SDK location field. Click Apply follow by OK.
 
Update: The latest version of Android SDK requires you to install the SDK API before you can create a new Android project.
 
Go to WIndows -> Android SDK and AVD Manager.
 
On the left pane, select the “Available Packages” entry. On the right, place a check on the version of the Android SDK that you want to install. Once done, click the Install Selected button.
 
That’s it. You have install and set up Android SDK in your Ubuntu. To create a new Android project, simply go to File -> New -> Project and choose Android project in the Wizard window.
 
### Taking screenshots of your Android phone
 
First enable the USB debug mode in Settings ->Applications->Development
 
Connect your Android phone to your computer via the USB cable.
 
Make sure that Eclipse is closed, navigate to your Android SDK folder. Go to the Tools folder and open the ddms.bat file. When prompted, select RUN.
 
Highlight the entry of your phone.
 
Go to Device -> Screen Capture.
 
That’s it.
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




