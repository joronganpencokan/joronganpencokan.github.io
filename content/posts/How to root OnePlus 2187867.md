---
title: "Unlock the Secret Power of Your Oneplus 2: Learn How to Root Like a Pro!"
ShowToc: true 
date: "2023-03-24"
author: "Cleo King"
---
*****
Unlock the Secret Power of Your OnePlus 2: Learn How to Root Like a Pro!

Have you ever felt like your OnePlus 2 isn't living up to its full potential? Do you want to access hidden features and applications? If so, then it's time to unlock the secret power of your device with root access.

Rooting is the process of obtaining administrative privileges on your Android device. By rooting your OnePlus 2, you can install custom ROMs, tweak system settings, and even overclock your CPU for more power-packed performance.

In this guide, we'll show you how to root your OnePlus 2 like a pro, step-by-step. We'll cover everything from preparation to installation so that you can get started with rooting in no time!

Step 1: Prepare Your Device

Before rooting your OnePlus 2, it's essential to back up all your data. There are chances of data loss during the rooting process, so it's better to be safe than sorry. You can use the OnePlus Switch app to backup all your data, including contacts, messages, apps, and data. Please ensure that your device is fully charged before you begin the rooting process.

Step 2: Unlock the Bootloader

The first step towards rooting your OnePlus 2 is to unlock the bootloader. To do this, you need to enable Developer Options and USB Debugging under Settings>>System>>Developer Options. Then, you need to connect your device to your computer and boot it into fastboot mode. Once you're in fastboot mode, open the command prompt on your computer, and type in the following command: "fastboot oem unlock," and hit enter. This command will unlock the bootloader of your OnePlus 2.

Step 3: Install TWRP Recovery

After unlocking the bootloader, the next step is to install a custom recovery app called TWRP. TWRP (Team Win Recovery Project) is a popular custom recovery app that allows you to flash custom ROMs and other modifications.

To install TWRP, you need to download the latest TWRP recovery image for your device from the official website. Make sure you download the correct image file for your device's model number. Once downloaded, open the command prompt on your computer, and type in the following command: "fastboot flash recovery <recovery_image filename.img>." This command will install TWRP recovery on your device.

Step 4: Root Your OnePlus 2

With TWRP installed, you're now ready to root your device. To do this, you need to download the latest version of Magisk from official sources. Magisk is a popular rooting tool that allows you to root your device without modifying the system partition.

Once you've downloaded Magisk, transfer it to your device's internal storage. Boot your device into TWRP recovery mode by pressing the Power and Volume down buttons simultaneously. Once you reach the TWRP recovery screen, tap on the Install button, navigate to the location where you have saved the Magisk file, and select it. Swipe to confirm the installation process.

Once the installation process finishes, restart your device. Congratulations! You've successfully rooted your OnePlus 2. You can now enjoy the full potential of your device without any manufacturer-imposed limitations.

In conclusion, rooting your OnePlus 2 is a simple process that can unlock the true power of your device. With a rooted device, you can install custom ROMs, tweak system settings, and overclock your CPU for better performance. Remember that rooting your device can void your warranty, so proceed with caution. With the steps outlined in this guide, you can root your OnePlus 2 like a pro and take full control of your device.

{{< youtube TC99Ev4beZU >}} 



One of the advantages of owning the OnePlus 2 is that it is very easy to root and has a flourishing developer community surrounding it. The handset is almost as easy to root as a Nexus device, so if you are looking for a device to tinker around with, but don’t want to spend a fortune on, the OnePlus 2 is your best bet.
However, if you are new to the Android ecosystem, rooting an Android device can turn out to be an intimidating and complex experience. Worry not though, as below I have provided the detailed steps on how you can easily gain root access on your OnePlus 2.
Note: Before you proceed further, it is highly recommended that you create a backup of all your important data on the OnePlus 2. Rooting the handset requires you to unlock the bootloader first, which will wipe the internal storage of the device clean.
Step 1: Download all the files linked below on your PC.

 

ADB/Fastboot: Windows | Mac
Windows 7/8.1 drivers for OnePlus 2
TWRP recovery (Rename to something simple like ”recovery.img” after downloading it)
SuperSU



If you are using a Mac, extract the contents from the ADB/Fastboot ZIP file inside a new folder called ‘oneplus’ on your desktop.
For Windows, users simply need to follow the instructions shown on the screen to install the ADB/Fastboot files on their PC. When prompted, make sure to install the them system wide. There is no need to install the drivers from ADB/Fastboot installer, since you will be installing them separately. Once ADB/Fastboot is installed, proceed to install the drivers on your PC.
Step 2: On your OnePlus 2, head over to Settings -> About Phone and tap on ‘Build Number’ 7 times to enable the hidden ‘Developer Options’ menu. Then, go back to the Settings menu followed by Developer Options. Enable the ‘Allow OEM Unlock’ option from this menu. Also enable the ‘Advanced Reboot menu’ option.
Step 3: Now, long press the Power button to bring up the Power menu. Tap on Reboot and then select the ‘Bootloader’ option.

 
### Unlocking the bootloader


Step 4: Connect the device to your PC and start a new Command prompt or Terminal window. Use the ‘cd’ command to navigate to the ‘oneplus‘ folder on your desktop. The below command should work for majority of the users:
Alternatively, you can simply drag ‘n’ drop the ‘oneplus’ folder to the Terminal or Command Prompt window as well.
Step 5: Run the following command to first make sure that the OnePlus 2 is being detected by your PC.
Mac users will need to prefix a “./” before every Fastboot or ADB command you run. Therefore, the above command will look something like this for you:
If your device is detected, you will receive a valid response along with the device ID of the handset. If not, you will get a timed out error in which case you need to repeat Steps 1-4 mentioned above.
Step 6: Finally, unlock the bootloader of your OnePlus 2 by running the following command:
You’ll need to confirm the selection on your handset by pressing the Volume Up button. Your device will reboot during the process. Once done, your OnePlus 2 should automatically boot back into Android. If not, use the Volume buttons to highlight the ‘Start’ option and then confirm it by pressing the Power button. The first boot can take a significant amount of time so be patient.

 
### Flashing TWRP recovery


Step 7: Transfer the SuperSU ZIP file to the internal storage of your OnePlus 2. Then repeat steps 2 and 3 from above to boot your the device back into Bootloader mode.
Step 8: Connect the device to your PC, and then execute the below command to install TWRP recovery on it.
Step 9: You now need to boot your OnePlus 2 into TWRP recovery. You can either do that manually by selecting the ‘Recovery’ option from the bootloader menu or by executing the below command:
Step 10: After your OnePlus has booted into TWRP recovery, tap on ‘Install’ and then navigate and select the SuperSU zip file. Confirm your selection by swiping the arrow to the right.
Step 11: Once the SuperSU zip file has been installed, select the ‘Reboot system’ option. The first boot after installing the zip file will take notably longer, but this will be a one-off incident.
Make sure to open the SuperSU app once after your OnePlus 2 has boot back into Android to update its binary.
Now that you have successfully rooted your OnePlus 2, you can try out some amazingly powerful apps for Android that require root access to work. Make sure to check out our list of the top five root apps for Android.





