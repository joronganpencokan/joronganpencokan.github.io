---
title: "Unbelievable! You can now install and use Microsoft Defender in Linux with just a few clicks!"
ShowToc: true 
date: "2022-12-29"
author: "Alan Dixon"
---
*****
Title: Unbelievable! Microsoft Defender Now Available for Linux with Simple Installation Process

Microsoft Defender, formerly known as Windows Defender, is a popular antivirus software used by many Windows users. However, it was never available for Linux - until now. The tech giant has officially released a version of Microsoft Defender for Linux distributions, and what's more surprising is how easy it is to install.

The news has been met with excitement and incredulity from the Linux community. For years, many have relied on open-source antivirus software, such as ClamAV, to protect their systems. Microsoft's decision to bring its popular antivirus software to Linux users is a game-changer, especially for those who rely on dual-booting Windows and Linux. 

So, how do you install Microsoft Defender on Linux? The process is surprisingly simple. The first step is to add the Microsoft repository to your Linux distribution. The company provides all the necessary commands to add and enable their repository for most popular distributions, including Ubuntu, Debian, and CentOS/RHEL. 

Once the repository is installed, users can download and install Microsoft Defender using a package manager like Apt or YUM. Users simply type in the command prompt "sudo apt-get install mdatp" or "sudo yum install mdatp" to initiate the process. 

After installation, users can start Microsoft Defender using the command prompt "sudo mdatp" in Ubuntu, Debian, and CentOS/RHEL. The software will run quietly in the background as a service, but users can check its status, scan for threats, and perform other actions using the command-line interface.  

Many users will appreciate how lightweight Microsoft Defender is on Linux. It has a minimal impact on system resources, and its command-line interface is efficient and easy to use. Plus, its signature-based scans and machine learning algorithms help protect Linux systems from various types of cyber threats, including viruses, malware, and spyware.

In conclusion, Microsoft's decision to bring its popular antivirus software to Linux has taken the tech world by surprise. With just a few clicks, Linux users can install Microsoft Defender and enjoy its features and protection. The software's availability may represent a turning point in the relationship between Microsoft and the Linux community. Who knows what Microsoft will bring next to Linux? The future looks bright for Linux users. 

So, if you're a Linux user, what are you waiting for? Give Microsoft Defender a try and see for yourself if it's as effective and easy to use as advertised.

{{< youtube UywjKEMjSp0 >}} 



While many Linux users outside of the enterprise may not understand the point of Microsoft tools on Linux, those on the inside will understand that they can be invaluable. The ability to integrate with Active Directory and much of the Microsoft ecosystem that has taken over the workplace is huge for desktop Linux, and it can make your favorite distro a more viable OS in the workplace. One of the most important parts of the enterprise is security. This tutorial shows you how to install and use Microsoft Defender on Linux to make sure your IT department can scan your machine for threats.
 
## How to Install Microsoft Defender in Linux
 
In order to install Microsoft defender on Linux, the instructions differ from distro to distro. Microsoft hasn’t put their packages in the repository, so you’ll have to make sure the right dependencies are installed and add the repos. 
 
### RPM-Based Distros
 
You’ll need yum-utils or dnf-utils:
 
To configure the Microsoft repos, the basic syntax of the Microsoft repos is as follows:
 
You can explore this mirror to see what you’d want. I’m going to be using prod.repo for the sake of consistency, as all distros have prod.repo or prod.list available. So, for my Fedora system, that command will be the following:
 
For the CentOS system I’m using to model, the command would be the following:
 
I’m using the yum command because it’s targeted at RHEL, CentOS, and Oracle Linux, but you could also use dnf. You’ll also need to import Microsoft’s GPG key using the following command:
 
Run a quick update:
 
After that, you should be able to just install the package. The name is mdatp, or Microsoft Defender Advanced Threat Protection. 
 
### Debian/Ubuntu Systems
 
You’ll need a couple of additional dependencies:
 
Then you can follow basically the same process: 
 
Install the repo, GPG key, any dependencies, and mdatp. 
 
## Using Microsoft Defender on Linux
 
### Running Scans
 
One of the main things that you probably want to do is scan your system for threats. To do that, you open the terminal and type the following command:
 
This will scan as many files as it has access to (in my case 329,812) and report on any threats it knows of. You can also run quick or custom scans. The custom option allows you to specify a directory or a file or to ignore any exclusions that you’ve set previously. You could run a scan like this:
 
If you’ve set an exclusion like covered below, you could run the above scan.
 
### Updating Signatures
 
To update the virus signatures on Microsoft Defender on Linux, update it just like any other package. 
 
### Setting Exclusions
 
To create exclusions so that files that are known to be good aren’t reported, you can do that a few ways. To exclude a file type, you can use a command like the following:
 
This will take all .png files and put them on the exclusion list. I wouldn’t necessarily recommend this, but if you have a particular file type that you create that you know will never need to be scanned, you can use that command to do that. 
 
To create an exclusion for a directory, you can use a very similar command:
 
Now, whatever directory you just told mdatp to exclude won’t be scanned. This is helpful if you have some security testing tools on your system, as those contain virus signatures that can trip up antivirus software. 
 
I hope you enjoyed this guide on installing and using Microsoft Defender on Linux. If you are not keen on using Microsoft Defender on Linux, check out some other antivirus software for Linux or learn how to scan for rootkits and viruses in Linux.
 
John is a young technical professional with a passion for educating users on the best ways to use their technology. He holds technical certifications covering topics ranging from computer hardware to cybersecurity to Linux system administration.
 
Our latest tutorials delivered straight to your inbox




