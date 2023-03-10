---
title: "Discover the mind-blowing secret to easily convert Deb Files to RPM with just a few clicks!"
ShowToc: true 
date: "2023-07-01"
author: "Oscar Delapaz"
---
*****
Title: Discover the Mind-Blowing Secret to Easily Convert Deb Files to RPM with Just a Few Clicks!

Introduction:

When it comes to Linux distributions, there are two major packaging systems - Debian and Red Hat. Debian-based distributions use .deb files, while Red Hat-based distributions use .rpm files. If you have a Debian-based system and need to install an application that comes in .rpm packaging, what do you do? The answer is to convert it to a .deb file. In this article, we'll show you how to make this conversion quickly and easily.

Body:

Firstly, let's understand what .rpm and .deb files are. RPM (Red Hat Package Manager) is a package management system for Red Hat-based systems like Fedora, CentOS, and OpenSUSE. It is used to install and manage software packages, resolve dependencies and update packages when needed. Deb (Debian package) is a package management system for Debian-based systems like Ubuntu, Mint, and Debian itself. It also allows software to be installed, managed, and updated.

To convert .rpm files to .deb files, we need to use a tool called Alien. Alien is a command-line tool that can convert between different packaging systems such as .deb, .rpm, and .tar.gz. To install Alien in a Debian-based system, open a terminal and type the following command:

sudo apt-get install alien

Once Alien is installed, you can easily convert .rpm files to .deb files using a single command. For example, to convert the google-chrome-stable current version, use the following command:

sudo alien -d google-chrome-stable_current_x86_64.rpm

This command will convert the .rpm file to a .deb file and place it in the current working directory. The "-d" option tells Alien to create a .deb file, and "-v" allows the conversion process to be verbose, giving a detailed description of the process.

Similarly, to convert multiple .rpm files stored in a directory, use the following command:

sudo alien -d -v *.rpm

This command will convert all the .rpm files in the current directory to .deb files.

Conclusion:

Converting .rpm files to .deb files is an uncomplicated process with Alien. It not only allows you to install applications that only come in .rpm packaging but also opens up the door to running applications on different Linux distributions. However, it's worth remembering that not all .rpm files can be converted to .deb files, especially if they have dependencies not available in the Deb system. But for simple applications, Alien is an effective tool that gets the job done.

{{< youtube woFtdIS6x0Q >}} 



RPM-based distributions are great. They offer a different way of doing things compared to Debian-based ones. Still, if you’re using one, you’ll no doubt be aware of its single greatest weakness – package availability. RPMs are just not as abundant as DEB files. It’s a fact.
 
Some users have combated this in a few ways: the OpenSUSE build service or by using repositories like  RPMFusion. For the most part, this helps close the gap. However, sometimes this just doesn’t cut it. Sometimes you still need a package, and you can’t find it anywhere.
 
Sure, you can always find the source of the program you want to install and compile it on your own, but sometimes that’s just not going to happen, especially for proprietary programs. Most of the time those kind of programs are only released with binary packages, so compiling them is out of the question.
 
How do we solve this issue? Simple. Just convert the package files to the format you need using Alien. It allows you to take one package of one format and convert it to another format. For the most part, doing this works. Most of the time packages get converted and can be installed with no problem. Other times their are errors. Try this at your own risk.
 
## How to convert DEB files to RPM
 
Before we begin, you’ll need Alien. Check your distro’s repository. It may be in there. If not, get it here. You’ll need to look for the package specific to your operating system. 
 

 
Once you’ve got it downloaded, install it and then open a terminal window.
 
Find the Deb package you’d like to convert and download it to your PC. Once you’ve got it downloaded, go back to the terminal you opened previously. Then, just enter the command below.
 
You’ll notice that in the command above, there’s more than one switch. Most people, when using alien to convert DEB to RPM, only use the -r switch. It’s not enough. This switch only tells the program to convert the package. If you add the -c and -v switch to the command, things will go a lot smoother (most of the time).
 
The -c switch will include all of the scripts that may or may not be inside the package. Most of the time, you’ll want to use this switch. It will help with converting packages better. Sometimes packages don’t come with scripts included, or just don’t work with the -c switch. In this case, just don’t use it. Do some experimentation.
 
There’s another switch that most people won’t use either. It’s -v. What does it do? It’ll display each and every command that Alien runs during the conversion. This will allow you to troubleshoot the conversion process.
 
Once you run the command, if successful, your new RPM file will be created, and after which, you’ll be able to take it and install it to your system. It’ll be located in the exact same place that the DEB file is. The RPM file will have the exact same name too.
 
## Conclusion
 
Alien is a very useful program. It helps close the massive gap that has been plaguing Redhat-based distributions for a very long time. Perhaps one day the time will come when developers recognize RPMs just as much a DEBs. Until then, this program will always serve a purpose.
 
Derrik Diener is a freelance technology blogger.
 
Our latest tutorials delivered straight to your inbox




