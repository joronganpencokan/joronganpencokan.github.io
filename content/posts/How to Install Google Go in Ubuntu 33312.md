---
title: "Unleash the Full Potential of Ubuntu with This Simple Trick to Install Google Go!"
ShowToc: true 
date: "2023-02-13"
author: "Donald Patterson"
---
*****
Ubuntu is one of the most popular Linux distributions in the world, with a huge user base and a vibrant community. With its powerful terminal, countless software options, and high level of customizability, Ubuntu is an ideal choice for anyone who wants to run a Linux-based operating system on their computer.

However, even with all of its great features, there are always ways to make Ubuntu even better. One way to do this is by installing Google Go, a programming language developed by Google that is designed for speed and efficiency.

In this article, we'll show you a simple trick for installing Google Go on your Ubuntu system, which will allow you to unlock the full potential of your machine and take your programming skills to the next level.

Step 1: Add the Google Go Repository

The first step in installing Google Go on Ubuntu is to add the Google Go repository to your system. This can be done using the following command in your terminal:

```bash
sudo add-apt-repository ppa:longsleep/golang-backports
```

This command will add the repository to your system, allowing you to easily install Google Go and its associated packages.

Step 2: Install Google Go

Once you have added the Google Go repository, you can easily install Google Go using the apt package manager. To do this, run the following command in your terminal:

```bash
sudo apt-get update && sudo apt-get install golang-go
```

This will update your system and install Google Go, along with any necessary dependencies.

Step 3: Check Your Installation

After installing Google Go, you should check that it has installed correctly by running the "go" command in your terminal. This will open the Go interactive shell, where you can test your installation and run Go programs.

```bash
go version
```

This command will output the current version of Google Go that you have installed on your system. If you see a version number, then your installation was successful.

Step 4: Start Using Google Go

Now that you have installed Google Go on your Ubuntu system, you can start using it for programming and development. Google Go has many features and benefits that make it an ideal choice for building fast and efficient applications, and it is becoming increasingly popular among developers around the world.

Conclusion

By following these simple steps, you can easily install Google Go on your Ubuntu system and start taking advantage of its powerful features and benefits. Whether you are a beginner or an experienced developer, Google Go is a great programming language to learn, and it can help you take your coding skills to the next level. So what are you waiting for? Start exploring the endless possibilities of Google Go today!

{{< youtube CRXbjLbepqc >}} 



What do you get when you mix Python and C? According to Google, it’s Go – a new programming language developed in-house and later open sourced. Go was created by a small team inside Google, including the well known Ken Thompson, co-inventor of Unix and major influence on C. It was created out of a lack of satisfaction with existing languages, mainly the excessively (in the minds of Go’s developers) long compile times needed for other languages. With Go, even a very large and complex application can compile in a few seconds, often less. Additionally, Go has built in concurrency support, so you can code for multiple CPUs without resorting to outside libraries of unknown quality.  While we don’t usually cover much programming here at MakeTechEasier, Go is such an interesting language that we just had to dip in a bit, and where better to start than by covering the system setup needed to get Go up and running on your Linux box.

Note:  This guide will cover the steps needed to get the Go compiler working in Linux.  It will not address how to write programs for Go, however if there is reader interest, we certainly could create such a tutorial.  
 
### Quick Overview
 
Go is a compiled language like C or C++, not interpreted like Python. This is course means that to do anything you need a Go compiler. Since Go is only officially available in source form, that means we’ll need to compile the Go compiler with gcc. When everything is done, you will have two Go compilers available, 6g and 8g. The only difference between them is that 6g creates 64-bit binaries and 8g creates 32-bit. Once you know which compiler you want, just code and compile for Go much like you would for gcc.  
 
There are technically other compiler options, but 6g and 8g are the official compilers and will be used exclusively in this guide.  
 
Update: A PPA is now available for Google Go. To install, open a terminal and type: 
 
### Preparing the System
 
There are a few quick easy things we’ll need to do in order to get our environment prepared. First, Go requires a few environment variables to be set in the shell so that it knows where to find and place files. You could type all the following commands directly into the terminal, but since some of them may be needed later, we’ll put them all in our .bashrc file. 
 
Open your ~/.bashrc file, and enter the following lines at the end:
 
Then at the command line type
 
to make sure it reads the file and creates those environment variables.  
 
### Installing Build Dependencies
 
We need a C compiler (such as gcc) along with some other utilities to create the Go compilers (6g and 8g). At your command prompt, run the following commands to install all needed build dependencies.  
 
### Getting and Compiling the Go Source Code
 
Now that we’ve got everything we need to install Go, we’re ready to get the code itself. To fetch the files, enter the following command:
 
Your output should approximately match the following:
 

 
And now we’re ready to compile Go into a usable language. To begin, enter the following in your terminal:
 
Remember, this part is gcc compiling Go, so this will not have the speed benefits associated with writing and compiling actual Go code and will likely take a few minutes.  
 
If you get a message about $GOBIN, make sure you remembered to create the directory that you put in your .bashrc file. Similarly, for other errors, double check the variables you put in your .bashrc file.  
 
### Test Your Installation
 
Save the following into a file called test.go
 
Now at the command line…
 
If all went well, you should see something like this:

 
And you’re ready to start coding!
 
Josh Price is a senior MakeTechEasier writer and owner of Rain Dog Software
 
Our latest tutorials delivered straight to your inbox




