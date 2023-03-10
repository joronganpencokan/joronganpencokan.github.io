---
title: "Revolutionize Your Linux Game: Master the Art of Tarball Installation in One Easy Step"
ShowToc: true 
date: "2023-04-25"
author: "Elise Seats"
---
*****
Revolutionize Your Linux Game: Master the Art of Tarball Installation in One Easy Step

Are you tired of trying to install complex programs on your Linux machine? Are you frustrated with the lack of clear instructions and confusing dependencies? Look no further, because the solution to all your troubles is here.

The art of the tarball installation is often overlooked in the Linux community, but it is a powerful and efficient way to install programs with ease. In just one easy step, you can revolutionize your Linux game and become a master of tarball installation.

What is a Tarball?

First and foremost, let's define what a tarball is. A tarball, or a tar archive, is a compressed file that contains many files and directories. Tarballs are often used for distributing source code or software packages, and they are easy to create and share.

The Advantages of Tarball Installation

Tarball installation has many advantages compared to other installation methods. First and foremost, tarballs are platform-independent, meaning that they can be installed on any Linux distribution. Additionally, tarball installation does not require additional software or programs, which can be a hassle with other installation methods.

Finally, tarball installation allows for manual control over the installation process, which can be helpful for advanced users who want to customize their installations. With all these advantages in mind, it's clear that tarball installation is a powerful tool that every Linux user should master.

The One Easy Step to Tarball Installation

Now, let's get to the one easy step that will revolutionize your Linux game: the tar command. The tar command is a powerful command-line tool that can be used to create and extract tarballs. To install a program using a tarball, all you need to do is follow these simple steps:

Step 1: Download the Tarball

The first step is to download the tarball from the program's website or a trusted source. After downloading the tarball, save it in a directory of your choice.

Step 2: Extract the Tarball

Next, open a terminal and navigate to the directory where the tarball is saved. Once you are in the correct directory, use the following command to extract the contents of the tarball:

tar xvzf [tarball_name]

The "x" option tells tar to extract the contents of the tarball, the "v" option shows the progress of the extraction, the "z" option is used to handle tarballs that have been compressed with gzip, and the "f" option specifies the name of the tarball.

Step 3: Install the Program

Once the tarball is extracted, navigate to the newly created directory and run the installation program. Installation programs can vary from program to program, but in most cases, you will need to run the following command:

./configure && make && sudo make install

The "./configure" command will configure the program for installation, the "make" command will build the program, and the "sudo make install" command will install the program on your system.

And that's it! With these simple steps, you can install any program using a tarball on your Linux machine.

In Conclusion

In conclusion, tarball installation is a powerful and efficient way to install programs on your Linux machine. With just one easy step, you can revolutionize your Linux game and become a master of tarball installation. So next time you need to install a complex program on your Linux machine, remember the power of the tar command and give tarball installation a try.

{{< youtube 7JKzC63JAn4 >}} 



Most of the time, installing software in Linux is a breeze.  Package management utilities like Apt, Portage, and Yum have made software installation in Linux even easier than it is in Windows (in my opinion at least).  If you know what you want, you simply tell your package manager that you want it, and it’ll find, download, install, and configure your new package for you.
 
Sometimes, however, the package doesn’t exist in your distribution’s repositories.  Often, in cases like that, your only option is to download a tarball (usually .tar.gz, .tar.bz, or .tgz) which contains the source code for the program that you have to compile yourself.  While it may be a little intimidating at first, compiling from source is normally a quick and easy process.  Today, we’ll learn how.
 
First off, I should note that not all tarballs are the same.  This guide will be assuming that the program you’re trying to install is a normal GNU-style source code collection.  Most require all the steps noted below, but many skip one step or another.  For the purposes of the tutorial I’ll be compiling the source code package of Python 3.0.1 from the Python homepage.
 
### Step 1:  Extract the tarball
 
For those new to Linux, tarball is a term commonly used to refer to a file which contains other files.  It’s a lot like a ZIP or RAR file in Windows, except that the tar program, on its own, does not compress the files.  Tar works with a compression program like gzip to actually compress the files, which is why you commonly see two extensions (.tar and .gz).  This is sometimes abbreviated to just .tgz.
 
Fortunately, we don’t need to run two separate programs to extract the files, we just tell tar to run the files through gzip to decompress.  You can use a graphical utility to extract those files by simply double clicking the tarball from your file manager, or you can do it from the command line with:
 
The options we gave tar are as follows:
 
- -z to tell tar to run this file through gzip to decompress (use -j for bzip files)
 - -x to extract the files
 - -v for “verbose”, so we can see a list of the files it’s extracting
 - -f to tell tar that we’re working with a file

 
For easier unzipping, see the Tips section at the bottom of this page 
 
### Configure
 
Once the files are extracted, open a command terminal and go to the directory where the files have been unzipped.  Before we can compile, we need to run the configure script.  The job of the configure script is to check your system for all the software necessary to compile the program from source code into a usable binary program.  It looks for things like gcc version and other tools needed to build the software.  So once you’re in the directory with all the files that were unpacked from the tarball, type in
 
If all goes well it’ll go through a check of various parts of your system, then drop you back to the command line like below:
 

 
The most common cause of errors in this step is a missing dependency.  Look closely at any errors you may get to determine what package is missing.
 
### Make
 
This is the real meat of the process – where we compile the source code into a runnable program.  This is normally the easiest step, only requiring a single command.  If the configure step completed without errors, simply type in
 
On a large program, this step might take a few minutes.  Once done, you’ll be dropped back to the shell prompt as shown here.
 
Technically, your program is now ready to use.  Under most circumstances, however, you’ll want to run one more step so that she program can be fully installed into the correct locations for it to be run from anywhere.
 
### Make install
 
All this really does is copy the now-compiled program into the system directories like /usr/bin so that it can be run from any directory without having to specify a path to the files.  Since it’s copying to a directory outside your home, you’ll probably need root privileges.  If the make step completed without errors, simply run
 
to copy the files.  At this point, you’re all done!  Your new program can be used like any other.
 
### Tips
 
Chances are, you’ll be compiling from source more than once in your life.  In fact, for those who like to use the latest and greatest software, this can be very common.  To make it a little easier, open your .bashrc file from your home directory, and add the following aliases to the end:
 
Josh Price is a senior MakeTechEasier writer and owner of Rain Dog Software
 
Our latest tutorials delivered straight to your inbox




