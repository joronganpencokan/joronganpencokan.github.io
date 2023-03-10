---
title: "Unlock the Secret to Installing Windows 11 Previews on Any PC - No Technical Skills Required!"
ShowToc: true 
date: "2023-04-11"
author: "George Butts"
---
*****
# Unlock the Secret to Installing Windows 11 Previews on Any PC - No Technical Skills Required! 

Are you excited about trying out Microsoft's new Windows 11 operating system but unsure if your device is compatible with it? Look no further. In this article, we'll show you how to install Windows 11 previews on any PC, regardless of technical expertise.

## Step 1: Check Your PC's Compatibility 

Before embarking on the installation process, it's essential to ensure that your pc meets the minimum system requirements for Windows 11. These include:

- A processor with at least two cores and a clock speed of 1GHz or higher. 
- At least 4GB of RAM.
- At least 64GB of storage, with 32GB free space. 
- A DirectX 12 compatible graphics card or integrated GPU with a WDDM 2.0 driver. 

Microsoft has also introduced specific security requirements for Windows 11, such as a Trusted Platform Module (TPM) version 2.0, which must be enabled in your device's BIOS. To check if your device meets these requirements, you can use Microsoft's PC Health Check app, which is available here: [https://aka.ms/GetPCHealthCheckApp](https://aka.ms/GetPCHealthCheckApp).

## Step 2: Download Windows 11 Preview 

Once you have verified that your device meets the minimum requirements, you'll need to download the Windows 11 Preview from the Microsoft website. You'll need to sign up for the Windows Insider program to access these preview builds. To do this, follow the steps outlined below:

1. Visit the [Windows Insider website](https://insider.windows.com/en-us/) and click "Register."
2. Sign in using your Microsoft account.
3. Follow the prompts to join the Windows Insider Program.
4. Once you've joined the program, click on the "Download Insider Previews" tab to access the Windows Insider Preview builds.

## Step 3: Install Windows 11 

Now that you have the Windows 11 Preview ISO file on your device, you'll need to create a bootable USB drive or DVD to install it. Here's how to do it:

1. Insert a blank USB drive or DVD into your device.
2. Open the Media Creation Tool application, which you can download from the Microsoft website [here](https://www.microsoft.com/en-us/software-download/windows11).
3. Follow the prompts to create a bootable USB drive or DVD.
4. Once the bootable device is ready, reboot your device and enter the boot menu by pressing the appropriate key (usually F2 or Delete).
5. Select your USB drive or DVD from the list of boot options and press Enter.

The Windows 11 installation process will begin, and you'll be prompted to select your language, region, and keyboard settings. Follow the prompts to complete the installation process.

## Step 4: Enjoy Your New Windows 11 Preview 

Congratulations! You've successfully installed the Windows 11 Preview on your device. You can now enjoy all the new features and improvements that Windows 11 brings. Keep in mind that this is a preview build and may contain bugs and other issues. Microsoft releases regular updates to address these issues, so it's crucial to keep your device up to date.

In conclusion, installing Windows 11 Preview on any PC is easier than you might think. By following the steps outlined above, you can enable your device to run the latest version of Windows without the need for technical skills. Happy computing!

{{< youtube sSWH_G4f-h8 >}} 



Although preview builds of Windows 11 are available for supported and unsupported hardware, the early builds of the next version of the OS are only available for devices that do not meet the minimum requirements for testers who have been part of the Windows Insider Program before June 24, 2021.
 
If you never tested previews of Windows, you will need a computer that meets the minimum system requirements with a TPM 2.0, an 8th Gen Intel processor or equivalent from AMD, 4GB of RAM, and 64GB of storage. However, if you have an older computer that does not meet the requirements, you may still be able to download and install builds of Windows 11 by modifying a few registry keys.
 
In this guide, you will learn the steps to bypass the restrictions to install Windows 11 previews on computers that do not meet the minimum hardware requirements. 
 
## Install Windows 11 Insider previews PCs not meeting requirements
 
To install Windows 11 Insider Preview builds on devices that don’t meet the minimum requirements, use these steps:
 
- Open Settings.
 - Click on Update & Security.
 - Click the Get started button.
 - Windows Insider Program settings
 - Click the Link an account button.
 - Link Microsoft account
 - Select the Microsoft account to join the program to install Windows 11 on unsupported hardware.
 - Click the Continue button.
 - Under the “Pick your Insider settings” section, select the Release Preview Channel option.
 - Release Preview Channel
 - Click the Confirm button.
 - Click the Confirm button to agree to the terms to use Windows 11 Insider Preview builds.
 - Click the Restart now button.
 - Sign in to your Windows account.
 - Open Start.
 - Search for regedit and click the top result to open the Registry Editor.
 - Browse the following path:
 - HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Selection
 - Double-click the UIBranch string.
 - Change its value to Dev and click the OK button.
 - UIBranch regedit
 - Double-click the ContentType string.
 - Change its value to Mainline and click the OK button.
 - UIContentType regedit
 - Double-click the Ring string.
 - Change its value to External and click the OK button.
 - UIRing regedit
 - Browse the following path:
 - HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability
 - Double-click the BranchName string.
 - Applicability regedit
 - Change its value to Dev and click the OK button.
 - Double-click the ContentType string.
 - Change its value to Mainline and click the OK button.
 - Double-click the Ring string.
 - Change its value to External and click the OK button.
 - Restart your computer.

 
Once you complete the steps, the device that doesn’t include support for TPM 2.0 or doesn’t have a support processor will start receiving preview builds from the Windows Insider Program.
 
Open Settings.
 
Click on Update & Security.
 
Click the Get started button.
 
Windows Insider Program settings

 
Click the Link an account button.
 
Link Microsoft account

 
Select the Microsoft account to join the program to install Windows 11 on unsupported hardware.
 
Click the Continue button.
 
Under the “Pick your Insider settings” section, select the Release Preview Channel option.
 
Release Preview Channel

 
Click the Confirm button.
 
Click the Confirm button to agree to the terms to use Windows 11 Insider Preview builds.
 
Click the Restart now button.
 
Sign in to your Windows account.
 
Open Start.
 
Search for regedit and click the top result to open the Registry Editor.
 
Browse the following path:
 
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Selection
 
Double-click the UIBranch string.
 
Change its value to Dev and click the OK button.
 
UIBranch regedit

 
Double-click the ContentType string.
 
Change its value to Mainline and click the OK button.
 
UIContentType regedit

 
Double-click the Ring string.
 
Change its value to External and click the OK button.
 
UIRing regedit

 
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability
 
Double-click the BranchName string.
 
Applicability regedit

 
Restart your computer.
 
This process only applies to testing Insider builds, once the final version releases, the device may get opted out of the program automatically. If you plan to install the final version of Windows 11 on unsupported hardware (not recommended), you can at least bypass the TPM requirement with these steps.




