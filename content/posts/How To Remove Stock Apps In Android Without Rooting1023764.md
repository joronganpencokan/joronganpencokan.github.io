---
title: "Unlock the Secret to Removing Unwanted Android Stock Apps - No Root Required!"
ShowToc: true 
date: "2023-05-12"
author: "Janet Bechtel"
---
*****
+# Unlock the Secret to Removing Unwanted Android Stock Apps - No Root Required!

If you are an Android user, then you may have noticed that some stock apps come pre-installed on your device. While some of these apps may be useful, others are just taking up valuable space on your device.

Removing pre-installed apps or bloatware has been a common practice for Android users. Previously, it required root access on the device, which could void the warranty and cause potential damage. However, now with changes in Android policies, it is possible to delete unwanted apps without rooting your device.

Here is how to get rid of stock apps safely and efficiently without using any third-party apps or rooting your device:

## Disabling Bloatware

Android devices have an in-built option to disable the pre-installed apps which are not required, but it does not delete them completely from the device storage. To disable apps follow these steps:

1. Go to Settings

2. Select the “Apps & notifications” option

3. Select the app you want to disable

4. Click on “Disable”

5. A pop-up will appear, click on “Disable app.”

The app is now disabled, and it will never run, consume battery or use any resources on your device until you re-enable it.

## Using ADB to Remove Bloatware

ADB (Android Debug Bridge) is a command-line tool for Android developers, which can also be used to remove bloatware.

Here is how you can remove pre-installed apps using ADB:

1. First, download the ADB tools on your PC (for Windows, macOS or Linux).

2. Connect your Android phone to your PC with a USB cable.

3. Enable USB debugging on your Android phone by going to “Settings > Developer options” and toggle on the “USB debugging” option.

4. Launch the command prompt on your PC and navigate to the folder where you have downloaded the ADB tools.

5. Type “adb devices” in the command prompt to check if your device is connected.

6. Once your device is connected, type “adb shell pm list packages” to see the list of all apps installed on your device.

7. Find the package name of the app you want to remove.

8. Type “adb shell pm uninstall -k --user 0 PackageName” in the command prompt and replace the “Package Name” with the app’s package name.

9. Press Enter, and the app will be uninstalled from your device.

It is essential to note that some pre-installed apps may be crucial for the proper functioning of the device or other apps.

## Conclusion

Removing unwanted bloatware or pre-installed apps will not only free up space but also improve the performance of your device. With a few clicks, you can disable or uninstall the unwanted stock apps without any root access or third-party apps.

However, be cautious while removing bloatware and ensure that you do not remove crucial apps that could potentially impact the functionality of other apps on your device.

{{< youtube YYMY5dOPV1g >}} 



The first thing to do after getting the new Android smartphone is to remove all those extra apps that you think you don’t need. Well, stock apps depend on your phone and your carrier. Therefore, you might not completely remove all stock apps from your phone. However, you can stop it permanently.

 
## Steps to Remove Stock Apps In Android Without Rooting


However, you can’t just remove bloatware until and unless you have a rooted Android device.
So, in this article, we are going to share the three best methods that would help you to quickly remove any stock app without rooting your Android. So follow the complete guide discussed below to proceed.
Step 1. First of all, open the Settings app on your Android device.

Step 2. Now you need to tap on “Apps.”

Step 3. Now you need to tap on Application Manager

Step 4. Like in the screenshot mentioned below, it’s the game that I got, and you can see it doesn’t have an option of “Uninstall.” So, here you need to tap on “Force Stop” and then tap on “Disable.”

That’s it! Now repeat it for every app that you think you will need. This will disable the app. If you need to uninstall it completely, then you need to follow the next method.

 
### Using Debloater


You can even use the Debloater tool on your PC to remove stock apps from Android. Since Debloater is a PC tool, you would need to have access to a computer. Follow the steps given below.
Step 1. First of all, you need to enable the developer option which you can enable by heading to Settings -> About Phone -> Build Number (Tap on build number 7-10 times, and your developer options will get activated).
Step 2. Now you will see the developer option in your settings and tap on it and scroll down and enable USB Debugging.

Step 3. Now you need to download and install the Debloater tool on your Windows PC. Next, connect your Android device with a USB cable to your PC and wait for the tool to detect your device. Once discovered, the debloater tool would prompt you with a Warning message

Step 4. Now you need to click on “Read Phone Packages” which is located on the top left corner it will start reading all of the applications on your device.

Step 5. Now you will be listed with many applications it detects as blocked and not blocked

Step 6. Now mark the apps that you want to delete from your device and then click on the “Apply” button. This will remove the apps from your device.

You can also undo the process by simply unselecting them. That’s it! You are done, now all those apps will be removed from your device, and your phone’s storage will be free from them.

 
### Using ADB


For those who don’t know, ADB or Android Debug Bridge is a versatile tool that allows users to manage the state of an emulator instance or Android-powered device. For more details about ADB, check What Is ‘ADB’ On Android And What It Does?
In this method, we are going to use ADB Command to remove stock apps from Android without root.
Step 1. First of all, download & install App Inspector on your Android device.

Step 2. Now follow this guide to install Android Debug Bridge on your computer.
Step 3. Open the App inspector app on your Android and tap on the ‘App List’

Step 4. Tap on the app that you want to uninstall and then note down the app path.

Step 5. Connect your Android to the computer and select the ‘Transfer Files’ mode.
Step 6. Now open the Command Prompt and enter the following command
adb devices
Step 7. Once done, type in adb shell to enter the shell mode.
Step 8. To uninstall the app, enter the following command
pm uninstall -k --user 0 <name of package>
Note: Replace <name of package> with the app path that you have copied in the fourth step.
That’s it, you are done! Now you will see a Success message on the command prompt.
So, this is how you can remove stock apps from your Android smartphone. I hope this article helped you! Please share it with your friends also. If you have any doubts related to this, let us know in the comment box below.





