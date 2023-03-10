---
title: "Revolutionize Your Project Management with Wekan: The Ultimate Self-Hosted Trello Killer!"
ShowToc: true 
date: "2023-04-20"
author: "Fredrick Reich"
---
*****
# Revolutionize Your Project Management with Wekan: The Ultimate Self-Hosted Trello Killer!

Are you tired of using Trello or similar project management tools that don't quite meet your requirements? Are you looking for an open-source alternative that you can host on your own servers? Look no further than Wekan!

## What is Wekan?

Wekan is a self-hosted, open-source, Kanban board-based project management tool. It offers features identical to Trello, such as customizable boards, cards, lists, and tasks that can be moved around, labeled, and prioritized as needed to manage your projects.

But unlike other project management software, Wekan is a completely free, open-source solution that can be customized to your team's unique workflow and business needs. You can control and manage your project data's privacy and security since the software is self-hosted.

## Key Features of Wekan

### Customizable Board

A Kanban board is the core of Wekan, and you can create boards for every project or department. You can customize the board's layout, including the number of cards that are displayed in each column, the colors used for each column, and more.

### Multiple Card Types

In Wekan, you can create several card types such as task cards, checklists, voting cards, and many more. With this feature, you can manage your projects efficiently and track progress better.

### Data Filter

Wekan comes with a data filtering option that helps you locate the data you want to view. You can filter cards by title, tags, and members, among other things.

### Support for Subtasks

Wekan allows you to create subtasks under a card, divided into multiple checklists. This feature helps list down a broad task into a detailed breakdown to manage it better.

### Integration with Other Tools

Wekan conveniently integrates with other tools such as GitHub, Trello, and more. This feature provides a seamless experience to track and control project progress simultaneously.

## Why Use Wekan?

### Easy Customization

With Wekan, you can customize everything, even the entire software. It lets you create custom plugins and themes that perfectly match your business needs.

### Enhanced Security

Wekan is self-hosted, meaning you have complete control over your data's privacy and security. You can create a secure network and access the software from any device with the necessary authentication credentials.

### Cost-Effective

Wekan provides a cost-effective solution to businesses looking to streamline their project management process, with no hidden fees or licensing costs.

### Flexibility

Wekan is available on a wide range of platforms, including Linux, Mac, and Windows, and can be self-hosted or integrated into cloud-based infrastructure. Its versatile deployment options make it a preferred choice for small-scale projects and large-scale enterprises.

## Conclusion

Wekan offers a flexible, cost-effective, and secure solution to project management that is easily customizable to meet your team's unique needs. With multiple board types and checklists to support tasks, data filters to streamline data view, and integration with different tools, Wekan is an ideal alternative to Trello or other project management software.

So why wait? Revolutionize your project management process with Wekan today!

{{< youtube N3iMLwCNOro >}} 



When most people think of project management tools, they think of Trello. It’s a web-based tool that lets you use cards (or Kanban) to manage ongoing projects. For most, this app is great and worth the price needed for more advanced features. This article is not for those people. Instead, this article is for those looking to ditch Trello for a self-hosted alternative: Wekan.
 
Wekan, like Trello, is a web-based project management tool that lets users create boards and cards, invite users, send project notifications, etc. In this article we’ll go over everything you need to know to get Wekan working on your server including what hardware to use, how to invite users, installation methods and everything in between! Let’s get started!
 
## Hardware requirements
 
- a Debian server or any other Debian-based Linux distribution to run the automated installer
 - Ubuntu server capable of running Snap packages or a Linux server distribution capable of installing the available tar.gz and necessary dependencies to get Wekan running
 - any moderately powerful old desktop PC (DDR-2 era or better) that can stay on at all times and act as a server
 - a VPS or any other type of enterprise grade server

 
## Debian/Debian-Based installation
 
There are several ways to install Wekan. In this guide we’ll be using an instruction set that is for Debian-based Linux distributions. This does not mean that Wekan will not run on other server operating systems like Redhat, Suse, CentOS, etc.
 
On Debian-based Linux server distributions, there is an auto-installation script for Wekan. This installation tool is meant to remove a lot of the tediousness that usually happens when installing server programs. Ubuntu server running 14.04 LTS should also use this script.
 

 
To start the installation process on Debian, download this script:
 
Then, run the installation tool:
 
Running the script with sudo privileges allows “autoinstall_wekan.sh” to install all necessary dependencies that Wekan relies on, like NodeJS, MongoDB, and other important tools.
 
When the automated installation tool finishes installing Wekan, a prompt appears. This prompt gives the user three choices. The first choice is to start the Wekan service. The second is to reboot the server and have the system take care of it, and the third is to exit the installer. Select #1 by entering “1” in the prompt and pressing the Enter key.
 
## Ubuntu server installation
 
Those running Ubuntu server 16.04+ have the ability to install snap packages. These packages are neat and useful ways of distributing software easily. It is because of this technology that getting Wekan up and running is a snap.
 
## Using Wekan
 
Wekan is installed on the server. Now, it’s time to set it up. First thing’s first: figure out the server’s IP address. This is done with the ifconfig command. Take note of the Internet ipv4 address, and enter it with :8080 on the end into a web browser. For example: http://192.168.1.107:8080
 
From here, just register an account on the page and start working. Additionally, tell other users to register an account on the server from the same page.
 
### Making a new project board
 
Create a new project board on your Wekan server by clicking the “Create new board” on the Welcome page. This board can house new project information you create along with other stuff contributed by other users added to it.
 
### Inviting new users to boards
 
Users are able to create boards, and any user on the server can be invited to a board. Click the “+” icon, then enter the username of the user to add to the board.
 
Note: you must have email set up on your server for the emailing feature to work.
 
### Importing Trello data
 
On the board creation screen, click “Create a new board.” Name it and then click on the “import from Trello” link.
 
Clicking the import link brings the user to a JSON import screen. To import Trello data to a new board, paste your Trello JSON data to it, then click the “Import” button. Soon after, the data will be present in the new board.
 
## Conclusion
 
Though Trello has what is essentially a monopoly on the market, Wekan is a tool many should take note of. While it’s true that it can be a bit of work to maintain your own server, in the end it’s worth it. Instead of paying the freemium fees Trello offers, all of the people using Wekan on your server will get great features at zero cost. And best of all, who doesn’t love an open-source alternative?
 
Do you use Trello? Would you switch to Wekan? Tell us why or why not below.
 
Derrik Diener is a freelance technology blogger.
 
Our latest tutorials delivered straight to your inbox




