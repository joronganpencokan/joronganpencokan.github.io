---
title: "Never Struggle With Python Installation on Windows Again - Learn How To Install Pip Now!"
ShowToc: true 
date: "2023-06-16"
author: "Cheryl Wilson"
---
*****
# Never Struggle With Python Installation on Windows Again - Learn How To Install Pip Now! 

Python is a widely used programming language. It has a vast range of applications in the fields of data analysis, web development, artificial intelligence, and many others. One of the primary reasons for its popularity is the easy-to-use interface, which makes it accessible for both beginners and experienced programmers. However, installing Python on a Windows computer can be a challenging task, especially for beginners who are new to the language.

If you’ve previously tried to install Python on a Windows computer, you may have encountered several issues. Outdated installation files, compatibility errors, and missing packages can all be a nuisance. Fortunately, there is a solution to this problem - Pip.

# What Is Pip? 
Pip is a package management system that simplifies the process of installing and managing software packages in Python. It allows users to download and install pre-built packages from the Python Package Index (PyPI) with a few simple commands. 

Pip is not included in the standard Python installation on Windows. However, it can be easily installed as a separate utility. In this article, we will guide you through the process of installing Pip on a Windows computer.

# How to Install Pip on Windows 

Step 1: Download the Get-pip.py Script
The first step is to download the get-pip.py script, which is a Python script that installs Pip. Go to the following link to download the script: https://bootstrap.pypa.io/get-pip.py

Step 2: Open the Command Prompt 
Open the Command Prompt on your Windows computer. You can do this by pressing the Windows key + R and typing ‘cmd’ in the Run dialog box.

Step 3: Navigate to the Directory 
Navigate to the directory where you downloaded the get-pip.py script. You can use the ‘cd’ command to navigate to the directory. For example, if you saved the script in the Downloads folder, type ‘cd Downloads’ and press Enter.

Step 4: Run the Script 
To run the script, type the following command in the Command Prompt window: 

```
python get-pip.py
```

Press Enter, and the script will start running. 

Step 5: Verify Pip Installation 
After the script finishes running, you can verify the Pip installation by typing the following command: 

```
pip --version
```

Press Enter, and the Command Prompt window will display the version of Pip installed on your computer.


# Conclusion 
Installing Python on a Windows computer can be a challenging task. However, with the help of Pip, the installation process becomes more straightforward, allowing you to focus on learning and developing your Python skills. 

Follow the steps outlined in this article, and you’ll have Pip installed in no time. Once installed, you’ll be able to manage software packages in Python with ease. Don’t let the installation process hold you back from learning this fantastic programming language. Get started today!

{{< youtube dj5oOPaeIqI >}} 




This article explains how to install Package Installer for Python (PIP) on a Windows Vista system and newer. If you have an older machine, you'll need to get the slightly older version of Python, such as v3.4.

 
### 
What to Know
 
- Install: Open installer > select Add Python 3.7 to PATH > Install Now > wait for confirmation.Next, open Command Prompt > enter print ("Hello World!").Inspect PIP commands by entering C:\Users\acpke> pip --help.

 
##   How to Install PIP on Windows 10  
 

PIP is included out-of-the-box in recent versions of Python, and you'll need Python anyway for PIP to be of any use.

 
- Head over to the Downloads page on the website at http://www.python.org to grab the installer for the Python language.
 - The main page should provide a convenient button, but in the event, you land on a page with a list of files, make sure you download the Windows x86-64 executable installer or Windows x86 executable installer, depending on whether you have a 32- or 64-bit machine.
 - Once downloaded, double-click the installer file.
 - On the first screen, select the Add Python 3.7 to PATH option.
 - Select Install Now at the top. You can see this will install a couple extra components: IDLE, a Python Integrated Development Environment; documentation on using Python, and PIP itself.
 - At this point the installer will do its thing and run through the setup process.
 - You'll see a confirmation screen at the end letting you know the install was successful. You can also select Disable path length limit to change a configuration in Windows that doesn't allow access to file paths longer than 260 characters.

 
##   Using Python on a Windows 10 Machine  
 

Python is a programming language, so to use it you'll need to learn how to code in it. That's beyond the scope of this article, but let's check to see if Python is installed properly.

 

Head over to the Downloads page on the website at http://www.python.org to grab the installer for the Python language.

 

The main page should provide a convenient button, but in the event, you land on a page with a list of files, make sure you download the Windows x86-64 executable installer or Windows x86 executable installer, depending on whether you have a 32- or 64-bit machine.

 

Once downloaded, double-click the installer file. 

 

On the first screen, select the Add Python 3.7 to PATH option.

 

Select Install Now at the top. You can see this will install a couple extra components: IDLE, a Python Integrated Development Environment; documentation on using Python, and PIP itself.

 

At this point the installer will do its thing and run through the setup process.

 

You'll see a confirmation screen at the end letting you know the install was successful. You can also select Disable path length limit to change a configuration in Windows that doesn't allow access to file paths longer than 260 characters.

 
- Open Command Prompt and type the following:
 - C:\Users\acpke> python --versionPython 3.7.4
 - You should see Python display its version number. You can also check if it's working correctly by pasting the following code into an empty text file and naming it "hello-world.py" (note the empty line at the end):
 - print ("Hello World!")
 - Now run it:
 - C:\Users\acpke> python \path\to\hello-world.pyHello World!

 
##   Using PIP to Install Python Packages on a Windows 10 Machine  
 

Now that we know Python is functioning, let's examine PIP.

 

Open Command Prompt and type the following:

 

C:\Users\acpke> python --versionPython 3.7.4

 

You should see Python display its version number. You can also check if it's working correctly by pasting the following code into an empty text file and naming it "hello-world.py" (note the empty line at the end):

 

print ("Hello World!")

 

Now run it:

 

C:\Users\acpke> python \path\to\hello-world.pyHello World!

 
- Although PIP should already be installed, we can check for it by issuing the following at the command prompt:
 - C:\Users\acpke> pip --help
 - This should show you the Help content for PIP, including the available commands. The most basic one is pip search, which will search the Python Package Index (PyPI) for your search term. For example, suppose we want to create our own custom web browser, the following command will show a list of all the packages in PyPI with the keyword "browser":
 - C:\Users\acpke> pip search browser
 - As you can see in the results in the below screenshot, there's a package called FireSnake-Browser, which is a web browser component already coded in Python. So, instead of having to code things like displaying a page, tabs, and bookmarks, we could just download this and customize it to our needs.
 - You can install a package with the following command:
 - C:\Users\acpke> pip install FireSnake-Browser
 - Unfortunately, updating all installed packages isn't as easy as updating Linux distributions; you need to do so for each package. When you see it's out of date run this command to perform the update:
 - C:\Users\acpke> pip install FireSnake-Browser --upgrade
 - Finally, removing a package is as easy as running this command:
 - C:\Users\acpke> pip uninstall FireSnake-Browser

 

Although PIP should already be installed, we can check for it by issuing the following at the command prompt:

 

C:\Users\acpke> pip --help

 

This should show you the Help content for PIP, including the available commands. The most basic one is pip search, which will search the Python Package Index (PyPI) for your search term. For example, suppose we want to create our own custom web browser, the following command will show a list of all the packages in PyPI with the keyword "browser":

 

C:\Users\acpke> pip search browser

 

As you can see in the results in the below screenshot, there's a package called FireSnake-Browser, which is a web browser component already coded in Python. So, instead of having to code things like displaying a page, tabs, and bookmarks, we could just download this and customize it to our needs.

 

You can install a package with the following command:

 

C:\Users\acpke> pip install FireSnake-Browser

 

Unfortunately, updating all installed packages isn't as easy as updating Linux distributions; you need to do so for each package. When you see it's out of date run this command to perform the update:

 

C:\Users\acpke> pip install FireSnake-Browser --upgrade

 

Finally, removing a package is as easy as running this command:

 

C:\Users\acpke> pip uninstall FireSnake-Browser

 

Get the Latest Tech News Delivered Every Day




