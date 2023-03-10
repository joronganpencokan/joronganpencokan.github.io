---
title: "End hackers' domination! Learn how to disappear your server like a ninja with Knockd now!"
ShowToc: true 
date: "2023-06-24"
author: "Charles Jones"
---
*****
# End hackers' domination! Learn how to disappear your server like a ninja with Knockd now!

Are you concerned about the safety and security of your server? Do the constant reports of hacking attempts and data breaches keep you up at night? Fear not, because we have the solution: Knockd.

Knockd is a port-knocking daemon that allows you to hide your server from prying eyes. When properly configured, your server will appear to be completely offline, effectively disappearing from the internet. This makes it extremely difficult for hackers to find and exploit vulnerabilities in your system.

So how does Knockd work? First, you must configure the daemon to listen for a sequence of "knocks" on specified ports. For example, you might set it up to listen for a sequence of three knocks on ports 22, 53, and 80. Once the sequence is received, Knockd will automatically open the necessary ports and allow access to the server.

This "knock" sequence can be virtually any combination of ports and can be changed at any time for added security. This means that even if a hacker somehow manages to figure out your current sequence, you can simply change it and render their efforts useless.

But that's not all Knockd can do. It also has a feature called "silent mode," which allows you to monitor all incoming traffic without responding to any requests. This is useful for detecting and analyzing potential threats without giving away the server's location.

So why haven't you heard of Knockd before? It's because it's the secret weapon of cyber ninjas – experts in the art of online security. But now, you too can use Knockd to protect your server like a pro.

In conclusion, if you're serious about keeping your server safe and secure, Knockd is an essential tool in your arsenal. Its ability to hide your server and detect potential threats make it a must-have for anyone concerned about online security. So don't wait – start using Knockd today and say goodbye to hackers' domination once and for all!

{{< youtube gtkiQNo4XlM >}} 



When you have a server that is publicly accessible, hackers can easily scan your IP address and check for open ports (particularly port 22 that is used for SSH) on your server. One way to hide your server from hackers is knockd. Knockd is a is a port-knock server. It listens to all traffic on an ethernet or other available interfaces, waiting for special sequences of port-hits. Clients such as telnet or Putty initiate port-hits by sending a TCP or packet to a port on the server.
 
In this article we will look at how we can use knockd to hide services running on a Linux server.
 
## Install Knockd on a Linux Server
 
Knockd is available in most distro’s repositories. On a Debian/Ubuntu/Ubuntu-based server, you can use the apt-get command to install knockd.
 
For Fedora, CentOS, or REHL users, you can use the yum command:
 
## Install and Configure Iptables
 
If you don’t have Iptables installed on your server, install it now.
 
The package iptables-persistent takes over the automatic loading of saved iptables.
 
Next, you need to allow already established connections as well as current sessions through iptables. Use the following command to achieve this task:
 
Next, you need to block all incoming connections to port 22 SSH.
 
Now let’s save the firewall rules via the following commands:
 
You can go ahead and check whether you have indeed blocked port 22 by connecting to your server via your computer.
 
## Configure  Knockd
 
Now it is time to configure knockd default settings. It is located at “/etc/knockd.conf.” To do so, change to the knockd configuration file using the following command:
 
For illustration purposes, I am using the leafpad editor. On your server you can use nano or Vi.
 
The screenshot shows the knockd configuration file.
 

 
- Options: You can find configuration options for Knockd in this field. As you can see in the screenshot above, it uses syslog for logging.
 - OpenSSH: This field is made up of sequence, sequence timeout, command and tcp flags.
 - Sequence: It shows the port sequence that can be used as a pattern by the client to initiate an action.
 - Sequence Timeout: It shows total time allocated to Clients to complete the required port knock sequence.
 - Command: This is the command that will be executed once the knocking sequence by the client matches the pattern in the sequence field.
 - TCP_FLAGS: This is the flag that must be set on the knocks issued by the client. If the flag was incorrect but the knock pattern bcorrect, the action will not be triggered.

 
Note:  The iptables command in the OpenSSH section in Knockd configuration file uses the -A option to append this rule to the end of the INPUT chain. This causes all the remaining connections to drop. 
 
To prevent it, replace it with the following below:
 
This command ensures that a new rule will be added to the top of the INPUT chain to accept ssh connections. 
 
## Enable and Start Knockd Service
 
Use the following procedure to enable the knockd service in “/etc/default/knock.”
 
Change value from 0 to 1 as shown in the screenshot.
 
Afterwards, save and close the file “/etc/default/knockd.”
 
Next, you can start the knockd service by using one of the following commands:
 
or
 
## Time to Knock-Test Your Linux Server
 
Now it’s time to test your Linux SSH server. To open port 22 at a specified IP address, use the following on your computer. (You will need to install knockd on your computer, too)
 
You need to replace “my-server-ip” with your server’s IP address.
 
You can now connect to port 22 SSH by using the following command:
 
After you have finished with whatever you wanted to do via port 22, you can close it using the following command:
 
## Conclusion
 
With knockd, you are well-assured that your SSH server is secured nad safe from attackers with sophisticated scanners. In addition, you are completely in charge of your SSH server.
 
Michael wears many hat in the opensource industry. He is based in Accra, Ghana. He revels in anything Linux and Devops.
 
Our latest tutorials delivered straight to your inbox




