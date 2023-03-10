---
title: "Linux users rejoice! Here's the ultimate guide to effortlessly install Cmake and streamline your development process"
ShowToc: true 
date: "2023-01-01"
author: "Penelope Zimmer"
---
*****
Introduction:
As a Linux user, you might have come across various software development projects that require Cmake as their build system. Cmake is an open-source, cross-platform build system that simplifies the building process of a project. It is widely popular among developers who prefer using Linux/Unix systems for development. Even though Cmake is an essential tool for developers, the installation process can be a bit confusing for new users. In this article, we will guide you through the easy installation process of Cmake on your Linux system.

Step 1: Check if Cmake is already installed
Before we begin the installation process, we must first check if Cmake is already installed on our Linux system. To check for Cmake, open your Linux terminal and type the following command:

cmake --version

If you have Cmake installed on your Linux system, you will see its version number displayed on the screen. However, if you do not have Cmake installed, you will see an error message.

Step 2: Install Cmake
The installation process for Cmake varies depending on the Linux distribution you are using. Here are some of the most commonly used Linux distributions and their corresponding installation methods.

Ubuntu/Debian:
For Ubuntu/Debian users, Cmake can be installed using the apt-get package manager. To install Cmake, open your Linux terminal and type the following command:

sudo apt-get install cmake

Fedora:
For Fedora users, Cmake can be installed using the dnf package manager. To install Cmake, open your Linux terminal and type the following command:

sudo dnf install cmake

Arch Linux:
For Arch Linux users, Cmake can be installed using the pacman package manager. To install Cmake, open your Linux terminal and type the following command:

sudo pacman -S cmake

Step 3: Verify the installation
Once the installation process is complete, it is essential to verify if Cmake has been installed correctly. To check if Cmake is installed, open your Linux terminal and type the following command:

cmake --version

If Cmake is installed correctly, you should see its version number displayed on the screen.

Conclusion:
Cmake is an essential tool for developers who use Linux/Unix systems. Installing Cmake on your Linux system is a simple process that can be completed in just a few steps. In this article, we have covered the necessary steps to install Cmake on your Linux system. We hope this guide will help you streamline your software development process and make it more efficient. With Cmake installed, you can take your software development to the next level.

{{< youtube sNksgCVHYWc >}} 



For many reasons, Linux has always been a programming mainstay, but most PC users are on Windows. This leaves programmers who need to test on the Windows platform with a dilemma: switching between platforms is near impossible. That’s where CMake comes in.
 
## What Is CMake?
 
CMake is an open-source application that allows you to build, test, and package software written in C and C++. It uses scripts called CMakeLists to generate build files on both Unix and Windows systems. This differs from GNU make, which is limited in the platforms it runs on, can be complicated to work with on large projects and doesn’t have a GUI.
 
## How to Install CMake
 
Installing CMake is easy. However, the method is scattered. Here you will find all the information compiled concisely.
 
### Prerequisites
 
You need a C++ compiler, and Clang and GCC are both great options. You can even build your own compiler if you’re skilled enough. The commands to install the compilers mentioned are as follows:
 
Clang:
 
GCC:
 
The three application sets for Clang should install the Clang application set, LLVM debugger (lldb) and LLVM linker (lld). Build essential is the GCC set of tools.
 
### 1. VS Code Integration
 
VS Code (Visual studio code) is the primary IDE for many programmers. The add-ons and terminal make it easy to install additional languages and tools. Integrating CMake into VS code is ideal and one of the best ways to use this tool.
 
First, install VS code if you haven’t already. The application is available in the snap store and on the website. Next, install the C/C++, CMake and CMake tool add-ons. Access the extensions using the keyboard shortcut Ctrl + Shift + X or by clicking the extensions tab on the left toolbar.
 
Check whether CMake or any other tools are installed using the --version command in the terminal.
 
### 2. Standalone Application
 
If you prefer using a different text editor, CMake can be installed as a standalone application as well. It is available in the Snap store and on the CMake website. You will find the shell script and the source code if you want to build and contribute on the website.
 
To install via the shell script, you need to allow it to execute as a program.
 
You can do this by changing the permissions in the file manager or using the following command:
 
You should be able to input the file path in the terminal and execute the script. The script will extract the CMake files to the location you select. You’ll find the CMake application in the bin folder.
 
## How to Configure CMake
 
The lack of documentation can make CMake difficult to use for people new to programming or even senior software engineers. Configuring CMake depends on your project at the time, but generally, select your C++ compiler and linker in the GUI. You can also configure it in the terminal using the following command:
 
Once you’ve set up your configuration, you can generate build files with the GUI or the cmake --build <directory>  command. This will build the source code binaries. Next, make these files accessible to the user with header files, libraries, and executables by using the terminal command, cmake --install. If you’re working within VS code, you can use the --target install command.
 
Depending on what you’ve written in the makefile, organize the files into one or more executables. If you’re using an older version of CMake, you should use make install.
 
## Frequently Asked Questions
 
Image credit: Needpix.  All screenshots by Nathan Meyer.
 
### How do I contribute C++ code to an open source project?
 
If you’re new to C++, it can be difficult to find projects to contribute to and learn more about CMake and programming. GitHub is a great place for that. You can find projects that interest you by using the topics link or by searching GitHub Topics in your search engine.
 
### Can I use CMake to compile C# code?
 
Although it may seem like C# and C++ are close, C# uses a JIT compiler in VS code. JIT (just-in-time) means that the code is compiled while the application is being executed and not before, as with C++, C, and Fortran. Consequently, CMake only supports those three programming languages.
 
### Is CMake still being actively supported?
 
Kitware, the company behind CMake, still supports and updates the application. CMake also has an active community in GitHub, so I would not worry about bugs and security.
 
Our latest tutorials delivered straight to your inbox




