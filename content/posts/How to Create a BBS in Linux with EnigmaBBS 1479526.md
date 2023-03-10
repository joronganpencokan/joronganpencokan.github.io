---
title: "Unleash Your Inner Linux Expert: Create Your Own Jaw-Dropping BBS with Enigmabbs in Just Minutes!"
ShowToc: true 
date: "2022-12-03"
author: "Carol Carr"
---
*****
+++
title = "Unleash Your Inner Linux Expert: Create Your Own Jaw-Dropping BBS with Enigmabbs in Just Minutes!"
date = 2021-05-10T19:47:13+05:30
draft = false
author = "OpenAI"
tags = ["Linux", "BBS", "Enigmabbs"]

[header]
image = "https://images.unsplash.com/photo-1565607888240-bb75fd082e45?ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8bG9nJTIwZGV2JTIwdHJhbnNmb3JtcyUyMGluJTIwbGF6eSUyMHByb2plY3RzJTIwYmx1ZSUyMGRyb3BzJTIwaW5mb3JtYXRpb24lMjBvZiUyMGNhYmluZXN8ZW58MHx8MHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=60"

+++

Do you want to create your own BBS but don't know where to start or have the time to learn a programming language? Fear not, with Enigmabbs you can create your own jaw-dropping BBS in just minutes!

Enigmabbs is a bulletin board system software that allows you to create your own BBS to share your interests with others, connect with like-minded individuals, and create a community around your ideas.

Let's get started!

## The prerequisites:
- A Linux server
- sudo access
- At least 1 GB of free space

## Installing Enigmabbs:
First, log in to your server as a sudo user and update the packages of your server:

```
sudo apt-get update && sudo apt-get upgrade
```

Next, install the dependencies required for Enigmabbs:

```
sudo apt-get install libncurses5-dev libncursesw5-dev zlib1g-dev bzip2 libreadline-dev libsqlite3-dev mercurial
```

Once you have installed the required dependencies, clone the Enigmabbs repository:

```
hg clone https://bitbucket.org/EnigmaBBS/enigmabbs
```

Change to the enigmabbs directory and run the configure script:

```
cd enigmabbs
./configure
```

Once the configure script has completed, run 'make' to compile Enigmabbs:

```
make
```

Finally, install Enigmabbs:

```
sudo make install
```

## Configuring Enigmabbs:
With Enigmabbs successfully installed, configure your BBS by editing the ~/enigmabbs/bbs.conf configuration file:

```
vi ~/enigmabbs/bbs.conf
```

Inside bbs.conf, you can configure various options like the name of the BBS, user limits, and other features. Once you have finished editing the file, save and close it.

## Running Enigmabbs:
To run Enigmabbs on your server, simply run the following command:

```
~/enigmabbs/enigma
```

You should see the Enigmabbs welcome screen and be prompted to enter your user credentials or register a new account.

Congratulations, you have successfully created your own BBS with Enigmabbs!

## Conclusion:
Enigmabbs is a powerful bulletin board system software that makes it easy to create your own BBS quickly and without having to learn a programming language. With Enigmabbs, you can create a community around your interests, connect with like-minded individuals, and share your ideas with the world. So why wait? Unleash your inner Linux expert today and create your own jaw-dropping BBS with Enigmabbs in just minutes!


Bulletin Board Systems (BBS) used to be the quintessential information hubs of the 90s. These were geographically local machines that users could connect to as a way to access information, obtain files and even communicate with other BBS users. Over the years, however, the know-how that you needed to even connect to one made it challenging for a regular user to participate in a BBS, making it lose its luster and appeal in favor of the more global Web.
 
Despite that, it is still possible to create your own BBS server using Linux. There are numerous projects, such as EnigmaBBS, that use modern languages and technologies to recreate the BBS experience of the 90s.
 
## What Is a BBS and EnigmaBBS?
 
At its core, a BBS is a suite of programs that allow multiple users to access a computer over a remote network. These computers, in turn, often contain programs that a system operator made to highlight a feature of their BBS. For example, most BBS machines in the 1990s provided games that are unique to their server.
 
EnigmaBBS is a modern adaptation of the traditional BBS software. It aims to recreate the original ’90s BBS experience with modern coding standards and technologies. EnigmaBBS also contains a number of features, such as WebSockets and SSH, which allow you to easily host and use a BBS.
 
Unlike traditional BBS, EnigmaBBS provides a platform for easy communication with other similar services through FidoNET. This approach enables you to seamlessly interact with other servers without the need to explicitly connect to each other.
 
Lastly, EnigmaBBS fully supports third-party Door Games through DoorParty, Exodus and CombatNet, so loading games through it is as simple as providing the dropfile for that particular game. It is possible to turn EnigmaBBS to a dedicated BBS gaming server for your friends and family.
 
## Installing EnigmaBBS
 
- Create a separate user account for the BBS server to make sure that it will not have any access to your personal files. To get started, run the following commands:

 
- Run su enigma to switch to the new user account.Download the EnigmaBBS installation script: an all-in-one script that fetches, compiles and installs all the necessary tools to create a copy of the BBS. Run the following commands:

 
- Enable the script’s execute bits and run it through your shell by running the following commands in your terminal:

 
- EnigmaBBS will begin by downloading all the packages that it needs to compile NodeJS. From there, it will download all the necessary packages to install the BBS software.

 
## Generating Your EnigmaBBS Configuration
 
Next, open a new terminal window to make sure that the machine will detect all of the programs that you just installed. 
 
- Since we’re using Ubuntu, we pressed the “New Tab” button in the current terminal window.

 
- Go to EnigmaBBS’s root directory. This is the folder that contains all the files and details for your BBS server. Run the following command to access it:

 
### Creating a New Configuration File
 
- Once inside, you can now create your BBS server’s configuration file with this command:

 
- EnigmaBBS will ask where you want to place your configuration file. For the most part, you only need to press Enter here to ensure that you can find all of the configuration files in their default directories.

 
- You’ll be asked to name your new EnigmaBBS instance. We named ours “Hello, world!”

 
- Provide a name for your first message conference, similar to a category in a forum website. We pressed Enter twice to use the default “Local” name.

 
- The script will ask you to name your first message area. Similar to a message conference, this is a way to further categorize the messages in your BBS. Once again, we pressed Enter twice to use the default values.

 
- Set the amount of logs that the program should keep while running. By default, EnigmaBBS recommends that you only keep diagnostic information in the server. Despite this, you can choose to either increase or decrease the amount of logging in your server, which can be especially useful if you are diagnosing a problem. We’ve picked the default “Info” level for our server.

 
## Connecting and Using Your New BBS
 
With your basic configuration done, you can start your EnigmaBBS server. Unlike other webservers, running a BBS instance is incredibly easy. 
 
- Run the following command:

 
- This will boot up EnigmaBBS and expose it to your local network. To connect to it, however, you’ll need to either use a telnet client or SSH. We used the former.

 
- Similar to starting up EnigmaBBS, connecting to it through telnet is quite straightforward, as Ubuntu ships with a BBS-compatible telnet client out of the box. Connecting to your local instance only requires that you run a single command:

 
- Once you are connected, EnigmaBBS will print a splash screen along with three options: “Login,” “Apply” and “Logout.”

 
### Creating the Sysop User
 
By default, EnigmaBBS reserves the first user account in the server as the Sysop user. 
 
- To create your administrator account, select “Apply” in the splash screen.

 
- Provide a username and other information about yourself. We used “ramcesr” as our username.

 
- One important thing to note is that you do not need to provide any real information in most of the fields in this page. For example, you can provide an email that does not exist, and EnigmaBBS will still create the account. This can be helpful in situations where do not want to leave any contact information in the BBS.

 
### Sending and Reading Your First Message
 
EnigmaBBS will immediately redirect you to your account’s main menu, where you can interact with various features of your BBS instance.
 
- Press M, then P to tell EnigmaBBS that you want to create a new message post. Press Enter on the next screen to write the subject of your message. We wrote “Hello world!”

 
- Press Enter again to write the body of your message.Press Esc, then “Save” to submit your message to the BBS.

 
- Viewing messages in EnigmaBBS is also relatively simple. Press M, then L in the Main Menu to list all the new messages in the current message conference.

 
## Communicating with a Different BBS
 
As mentioned above, EnigmaBBS also allows you to seamlessly communicate with other BBS servers. It can be especially useful if you want to introduce additional activity in your BBS instance.
 
- Turn off your EnigmaBBS instance by either pressing Ctrl + C or closing its terminal window.Edit your server’s configuration file. You can find this HJSON file under the “config” folder of the EnigmaBBS root directory.

 
- Find the “chatServers” option. This controls the Multi-Relay Chat function of EnigmaBBS. Look for this option by pressing / and typing “chatServers.”

 
- Change the “enabled” value from “false” to “true.”

 
- Save this file and restart EnigmaBBS.

 
- Access the Multi-Relay Chat by typing MRC and pressing Enter in the Main Menu. A new windows will load where EnigmaBBS will connect you to a chatroom with other BBS servers.

 
## Creating a Web Content Server
 
Aside from sending messages, EnigmaBBS is also a highly flexible piece of software that can be extended to do whatever you want. For example, it is possible to create a content server that will display all the messages and files in the BBS.
 
- Open your server’s “config.hjson” file.

 
- Look for the “contentServer” function, a block that contains all the necessary settings that you need to set to create a Web-based content portal. We pressed / in Vim and typed “contentServer” to jump to that particular section.

 
- Provide a domain name for the web server that you are creating. We wrote “localhost” since we only intend to run this server in the local network.

 
- Tell EnigmaBBS that you want to enable its web server by changing the “enabled” value under “http” to “true.”

 
- Save the “config.hjson” file and restart your BBS server to apply the new settings. Once done, you can then visit the BBS web portal by typing localhost:8080 in your web browser.

 
## Frequently Asked Questions
 
Image credit: Unsplash All screenshots by Ramces Red
 
### The  EnigmaBBS installation script is not working
 
This is most likely because you are using a different shell in your system. By default, the EnigmaBBS install script uses Bash to compile the necessary programs. The script relies on Bash-specific functions to perform the installation properly. One way to solve this issue is to run the Bash shell from your current terminal by running: /bin/bash. Doing this will change the prompt in the screen indicating that you are now using Bash. From there, you can run the installation script again.
 
### EnigmaBBS is reporting a MODULE_NOT_FOUND error
 
This happens when there is a difference between the library versions that EnigmaBBS expects and what it can find in your computer.
 
To fix this, you need to do three things: First, you need to run rm -rf /home/$USER/enigma-bbs/node-modules to remove all the objects that EnigmaBBS just compiled.
 
Then add the official NodeJS repository to your package manager in Ubuntu by running the command:
 
curl -sL https://deb.nodesource.com/setup_14.x | sudo bash -. 
 
Once done, install the appropriate version of NodeJS as well as rebuild all the objects for EnigmaBBS by running this single command:
 
sudo apt install nodejs && nvm install v14.19.3 && npm install && npm rebuild.
 
### Is it possible to change the default port of EnigmaBBS?
 
Yes. The BBS server uses port 8888 for telnet connections because most Linux distributions disable the default telnet port and do not allow any traffic through it. Despite that, you can still change the port that EnigmaBBS uses by changing a few settings in the “config.hjson” file.
 
Look for the port: variable under “loginServers,” then change it to any number that does not conflict with any running service in your system.
 
Ramces is a technology writer that lived with computers all his life. A prolific reader and a student of Anthropology, he is an eccentric character that writes articles about Linux and anything *nix.
 
Our latest tutorials delivered straight to your inbox




