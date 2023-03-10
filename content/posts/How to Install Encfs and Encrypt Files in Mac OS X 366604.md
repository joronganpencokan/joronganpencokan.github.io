---
title: "Unlock the Secrets of Secure Mac File Encryption with this Simple Encfs Installation Guide!"
ShowToc: true 
date: "2023-04-29"
author: "Ronnie Wolcott"
---
*****
# Unlock the Secrets of Secure Mac File Encryption with this Simple Encfs Installation Guide!

In today's digital age, data privacy and security are more critical than ever. With the increasing frequency of cyber-attacks and data breaches, securing sensitive information is a top priority for individuals and businesses alike. One of the best ways to protect data is through encryption, which transforms data into unreadable code. Encfs is an open-source, powerful file encryption tool that provides an easy way to secure your data on a Mac. This article will guide you through the process of installing Encfs and using it to encrypt your files.

## Step 1: Install Encfs

The first step in using Encfs is to install it on your Mac. Here's how to do it:

1. Open the Terminal app on your Mac by pressing `⌘+space` to open spotlight search and typing "Terminal."
2. In the Terminal window that appears, type the following command and press `Enter:`

    ```sh
    brew install --cask osxfuse
    brew install encfs
    ```

    This command will install both Encfs and the OSXFUSE framework, which is required for Encfs to work on your Mac. You may be prompted to enter your password to continue with the installation.

## Step 2: Create an Encrypted Directory

Now that Encfs is installed, the next step is to create an encrypted directory to store your files. Follow these steps:

1. In the Terminal window, type the following command and press `Enter:`

    ```sh
    mkdir ~/encrypted
    ```

    This command will create a new directory called "encrypted" in your user directory.

2. Next, create a new encrypted directory using Encfs by typing the following command and pressing `Enter:`

    ```sh
    encfs ~/encrypted ~/secured
    ```

    This command will create an encrypted directory called "secured" inside the "encrypted" folder. You will be prompted to set a password for the directory, so make sure to choose a strong password that you can remember.

## Step 3: Mount the Encrypted Directory

Once you have created the encrypted directory, you need to mount it to access your files. Here's how to do it:

1. In the Terminal window, type the following command and press `Enter:`

    ```sh
    encfs ~/encrypted ~/secured
    ```

    This command will mount the "secured" encrypted directory to your computer, allowing you to access its contents.

2. To access the directory, open the Finder app on your Mac, navigate to your user directory, and look for the "secured" folder.

## Step 4: Encrypt Your Files

With Encfs installed and the encrypted directory set up, you can now encrypt your files. Here's how to do it:

1. Drag and drop the file or folder that you want to encrypt into the "secured" folder in the Finder window.

2. Once the file or folder is inside the "secured" folder, it will automatically be encrypted by Encfs.

Every time you access the "secured" folder, you will be prompted to enter the password you set up during the creation of the encrypted directory. This provides an extra layer of security, ensuring that only you can access your encrypted files.

## Conclusion

Encfs offers an easy way to encrypt your files on a Mac, providing an extra layer of protection against prying eyes. By following the simple installation guide outlined in this article, you can keep your sensitive information safe and secure. With Encfs, you can enjoy peace of mind knowing that your data is protected from unauthorized access.

{{< youtube C25VWAGl7Tw >}} 



Encfs is an open-source software that is widely used to create encrypted filesystem. It is particularly useful for encrypting files that you want to store in the cloud, such as Dropbox or Google Drive. Using encfs in Linux and Windows is pretty straightforward as there are installers for both platforms. However, for Mac OS X, installing encfs is not as easy as it should be. Here is how you can install and use encfs in Mac OS X.
 
## Installing encfs in Mac OS X
 
There are a number of ways to install encfs in Mac OS X. In this tutorial, we will show you the homebrew and OSXfuse installation method. It will require the use of terminal, so be prepared to get your hands dirty. 
 
Homebrew is a useful package manager for Mac OS X. It allows you to install plenty of applications with a single command.
 
1. Open Terminal in Mac OS X. If you are not aware of where it is located, you can find it at “Applications -> Utilities -> Terminal”. Type the command:
 
This will install Homebrew in your system. If you have already installed Homebrew, you can ignore this step.
 
To install encfs (in El Capitan), simply run the command in the terminal:
 
Once the installation is completed, you will have encfs running in your system.
 
## Using encfs in Mac OS X
 
Still in the terminal, you can create an encrypted filesystem in Dropbox using this command:
 
Go through the setup process. You will be prompted to enter a master password. Make sure you use a strong password and remember it. Once completed, you should see a “Private” folder in your Home directory. Any file you place in this folder will be encrypted and stored in the “Dropbox -> Private” folder.
 
## Automount encrypted directory on startup
 
It is very troublesome if you have to mount the encrypted directory everytime you login. Use the steps below to automount the encrypted directory when you login. 
 
1. Open “Keychain Access”. We will be adding your encfs master password to Keychain so the script can automount the encrypted directory without prompting you for password. Add a new entry. Enter “encfs” for both the “Item name” and “Account Name” field. Once you have added the password, you can close Keychain Access.
 

 
2. Open a text editor and copy the following text into it. 
 
Save the file as “encfslogin.sh” in your User directory.
 
Make the script executable:
 
3. Next, open AppleScript editor and paste the line:
 
and save it as an application in your User directory.
 
4. Lastly, go to “System Preferences -> Users & Groups”, click on your User account and select “Login items”. Add the encfslogin application to the startup list. 
 
Log out and login again. Your encrypted directory should be auto-mounted now. 
 
Image credit: security concept with a lock by BigStockPhoto
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




