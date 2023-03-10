---
title: "Protect Your Network Like A Pro: Stop Hackers In Their Tracks With The Ultimate DNS Blockers And Firewalls!"
ShowToc: true 
date: "2023-03-30"
author: "George Harmeson"
---
*****
# Protect Your Network Like A Pro: Stop Hackers In Their Tracks With The Ultimate DNS Blockers And Firewalls!

Are you worried about the safety of your network? Do you fear that hackers may find a way to penetrate your security measures and gain unauthorized access to sensitive information? If so, you've come to the right place. In this article, we'll discuss how to protect your network like a pro by using the ultimate DNS blockers and firewalls.

## What are DNS blockers and firewalls?

Before we dive into the specifics of how to protect your network, let's define what DNS blockers and firewalls are. DNS blockers are services that block access to certain websites based on their IP addresses. By doing so, these services can prevent users from visiting websites that may be malicious or harmful to the network.

On the other hand, firewalls are devices or software programs that monitor and control incoming and outgoing network traffic. They act as a barrier between your network and external networks, preventing unauthorized access and protecting against attacks.

## How do DNS blockers and firewalls protect your network?

Now that we know what DNS blockers and firewalls are, let's explore how they can help protect your network from cyber attacks. DNS blockers work by blocking access to known malicious websites, preventing viruses and other malware from being downloaded onto your network. By blocking access to these harmful websites, DNS blockers can help keep your network safe from cyber attacks.

Firewalls work similarly by monitoring incoming and outgoing network traffic. They can block access to suspicious or unauthorized traffic, preventing hackers from gaining access to your network. Additionally, firewalls can identify and block traffic that is attempting to exploit vulnerabilities in your network, such as a weak password or unsecured file sharing.

## Choosing the right DNS blocker and firewall for your network

There are many DNS blockers and firewalls available on the market, and choosing the right one can be overwhelming. However, there are several factors to consider when selecting the best solution for your needs.

First and foremost, consider the size and complexity of your network. A smaller network with fewer users may not require a complex firewall, while a larger network with multiple users may require a more sophisticated solution.

Additionally, the type of devices accessing your network is important to consider. If you have a mix of Windows and macOS devices, you'll need a firewall that is compatible with both operating systems.

Finally, you'll want to choose a DNS blocker and firewall that is easy to use and manage. Look for products that offer user-friendly interfaces and allow for straightforward configuration and management.

## Conclusion

Protecting your network from cyber attacks is essential in today's digital age. By using DNS blockers and firewalls, you can stop hackers in their tracks and prevent unauthorized access to sensitive information. When selecting a DNS blocker and firewall, consider the size and complexity of your network, as well as the type of devices accessing it. With the right solutions in place, you can protect your network like a pro and safeguard your business against cyber threats.

{{< youtube 2J3idGxCbuc >}} 



I'll assume you already have an antimalware/antivirus solution in place, such as Windows Security, which is built into Windows 10 and Windows 11 (and which I believe works particularly well). But antivirus isn't enough.
Escalating international tensions -- coupled with an ever-increasing number of professionals working remotely -- are driving the need for small-scale solutions and best practices to secure home- and small-business networks and mobile devices from malware, malvertising, and other threats. 
What follows is a brief guide -- with product recommendations and best practices -- for those of you looking to navigate the rapidly evolving cybersecurity landscape. If you have limited network security experience but want to provide additional security for yourself, your small business, or your friends and family, this guide is for you. (If you're looking for more extensive resources on networking security, CISA's guide is a good place to start.) 
Below are the products I am currently using to protect my family's home networks and mobile devices. (I expect to add more product and service recommendations when I have sufficient time to investigate them.)

 
## Mobile and device-based DNS VPN firewall


To begin using it, simply visit nextdns.io, and start a new configuration. The first thing you will want to take note of is your randomly-issued ID, which is how you and your family members will identify yourself to the service and how it will apply specific security settings you choose to them.
When installed as an app on a device, the service creates a private encrypted connection (VPN) to its cloud servers. Its basic functionality includes proxying Domain Name Services (DNS) queries against a large database of potentially malicious sites and blocking them, depending on how restrictive the service is set up. This means if you try to access a site listed on its blocklists, it will stop the connection. This also includes blocklists for advertisements and pornography, if enabled. 
It should be noted that NextDNS is not a VPN service (such as these covered recently by David Gewirtz) for creating anonymized private connections to the public internet and for end-to-end enterprise VPN connectivity (such as with OpenVPN) even though it uses its own VPN for the service to work. However, it can work in tandem with those services as needed.
The service has native clients for iOS, MacOS, Android, Windows, Linux, and Chrome OS, and can be set as the default DNS on a broadband router or an IoT device. And best of all, the lowest tier of service is absolutely free. The "Pro" service has unlimited devices, unlimited queries, unlimited configurations, and is a whole $20 per year.
The only main drawback of this service is that it is client-based -- meaning you need to install this software on every device you use it on. So it's ideal for smartphones, tablets, and laptops when you are on a mobile network or using a public Wi-Fi or ethernet connection, but not suitable for "blanket" device coverage on a home or small office broadband network. It is also a DNS-based solution rather than an IP-based and connection-oriented solution, so it is not a true intrusion prevention solution such as a hardware firewall.
The clients all have similar configuration screens and are all easy to install, but the key thing to remember is the Configuration ID and to "Send Device ID", because that ensures you are using the service with your specified configuration and that when the system logs activity, you will be able to narrow down to which device is having an event.
Once you have the clients connected to the NextDNS VPN, you can verify they are using the service and that it is logging the connections with the Logs tab at the top of the web portal UX. The logs page allows you to look at traffic logs on a device per device basis, for all DNS queries or just blocked queries.
Security protection options can be set in the Security menu tab where various services can be enabled, such as for AI-Driven Threats, Google Safe Browsing, Cryptojacking, DNS Rebinding, IDN Homograph Attacks, Typosquatting, Domain Generation Algorithms, Newly Registered Domains, Parked Domains, and Child Sexual Abuse Material. I have all of these currently turned on in my own configuration.
Tracking and Ad blocking are enabled in the Privacy menu tab. The two blocklists I currently have enabled are NextDNS's maintained list and OISD, which covers enough ground to protect mobile devices for most regular browsing and mobile app use while keeping functionality the least restrictive as possible. If you enable too many lists, you may find that certain apps (such as Facebook, with its Graph API) may begin to misbehave, and then you will need to disable NextDNS for them to work again temporarily. So I would only start adding more blocklists such as AdGuard and a few others on their curated list one at a time to see how it affects your usability. 
NextDNS also has a Parental Controls menu for locking out specific websites, apps, and games, as well as the ability to lock out pornography, piracy, dating, and social networks. NextDNS has the ability to have multiple Configuration IDs per account, so if you want to configure your children's devices, you might want to assign them a separate Configuration ID as well as enter a Parental Passcode in their NextDNS app settings screen so it cannot be altered. You'll also want to set Parental Controls on their devices using native app restrictions (Such as the Content and Privacy Restrictions menu on iOS) so the NextDNS app cannot be deleted.

 
## Open Source wide-spectrum DNS blocking


The easiest way to run it is to download Docker Desktop for your operating system (Windows, Mac), or Docker Engine for Linux, and then install Pi-Hole into a Docker Container. 
This sounds scarier than it actually is – the Docker Desktop is an easy wizard-based install, and the Pi-Hole part involves issuing a single command line to pull the Pi-Hole repository (docker pull pihole/pihole), and another command line to fire up the container:
You will want to change the bolded sections to reflect your actual local IP address for ServerIP, the desired password, and the Time Zone (I used America/New_York). More elaborate instructions for Windows documented by Andrew Denty on his blog can be found here and Mac can be found in Nathan Alderman's article at iMore here.
You will also want to make sure the system you intend to run it on has a static rather than a dynamic IP. The three DNS IP addresses I have chosen here for the Pi-Hole container are the two Cloudflare and Google servers.
Once you have Pi-Hole installed, you'll want to connect via browser to the administrative interface on the system running it. 
As you can see, I have over two million domains set to be blocked. How do you do the same? You go into Group Management, choose Adlist (this is what Pi-Hole uses to refer to community-sourced lists of domains to be blocked), and then plug in the URL of the Adlist.
Which Adlists should you use? Well, there are many lists you can choose from, all of which have different purposes such as Advertising, Suspected Malware, Malvertising, and others. But I consulted with Jason Ford, a principal engineer at a prominent Silicon Valley-based infosec company, and asked him what he used on his Pi-Hole. He was nice enough to give me his lists and his regular expressions for domain blocking. These include some very popular ones such as OISD, Steven Black, and some curated ones from Firebog. 
If you decide to use all of his lists, you'll have over 2 million domains blocked on your Pi-Hole.
Once you have pasted the URLs of the Adlists into the UX, you'll want to go into Tools and choose Update Gravity. This is what refreshes the local database and populates the blocking engine. 
If there are specific domains you want to block or permit, you want to go into the Blacklist or Whitelist menus and put them in individually.
To begin using Pi-Hole on your devices and clients, change your DNS settings to reflect that of the Pi-Hole machine. So, for example, my Pi-Hole is running on my 192.168.1.78 Windows machine – so I've set my Mac and my wife's Windows PC and a few other things to use it as the DNS.
If you find the Pi-Hole is blocking a specific site or functionality that you need to use (such as a needed tracking cookie or script), simply whitelist the site, or temporarily, click on Disable from the left-hand administrative menu. You can choose to disable it indefinitely, for 10 seconds, for 30 seconds, for 5 minutes, or a custom time.
EDIT: Pi-Hole developer Dan Schaper has communicated the following: "As an aside, we're not aware of any appliances that are planning to embed Pi-hole. Would you be able to share that information? It would be helpful to others to know that there are major changes planned and that some coordination may be in order."
While there are many hardware firewall and network intrusion protection products available in the medium/large SMB and the Enterprise space (such as Cisco Meraki, Sonicwall, Palo Alto Networks, Fortinet, Ubiquiti, Watchguard, and Sophos), there are very few priced for home and smaller SMBs. What I currently use for myself, my immediate family, and have recommended to friends and colleagues is the Firewalla series of products, which is a company founded by a group of former Cisco  engineers.
I like Firewalla because it is very easy to install, it isn't particularly expensive, and it has no ongoing fees. Unlike the DNS blocking solutions above, it is a true embedded Linux, IP-based rules firewall with advanced intrusion detection capabilities that can monitor every device on your home network. 
Firewalla also has a very good user interface and app for mobile devices for administrating it and receiving alerts and a pretty robust remote management web interface. You don't need to be a network security genius to set rules and protect your network. 
You can certainly do some very granular protections and permissions on a per-device basis and set block lists of different target groups and lots of other things, but for the most part, the default configuration when applied to all devices on the network is likely sufficient for most home users. 
Firewalla's CEO and founder, Jerry Chen, has published a best practices guide (Part 1, Part 2, Part 3) that I suggest you review once you get your box running. Additionally, if you are not sure which router mode to use with your Firewalla (Router, Bridge, DHCP, Simple) read this guide, and if you want to understand how it intercepts network traffic, read here.

 
## Open Source Firewalls: OPNSense and pfSense


If you are inclined to set up an actual software-based firewall on a border gateway on your premises and want something that is robust but not expensive, then look no further than OPNsense. 
The complete feature list of what this software project can do extends far beyond this list. It is downloadable as a 64-bit x86 ISO or USB installer image so that you can install it on a PC with (at least two) Ethernet ports. The project also sells it pre-installed on a hardware appliance in multiple configurations, starting with 4-port gigabit networking, a 600mbps IPsec VPN, 16GB of flash storage, 4GB RAM, and a fanless casing and mainboard for 549 EUR.

 
Traffic Shaper Two-factor Authentication throughout the system Captive portal Forward Caching Proxy (transparent) with Blacklist support Virtual Private Network (site to site & road warrior, IPsec, OpenVPN & legacy PPTP support) High Availability & Hardware Failover ( with configuration synchronization & synchronized state tables) Intrusion Detection and Prevention Built-in reporting and monitoring tools including RRD Graphs Netflow Exporter Network Flow Monitoring Support for plugins DNS Server & DNS Forwarder DHCP Server and Relay Dynamic DNS Encrypted configuration backup to Google Drive Stateful inspection firewall Granular control over state table 802.1Q VLAN support


Similar to OPNSense is pfSense, which has a comparable feature set and similar hardware requirements. As with OPNSense, pre-configured appliances are available, from as low as $189 for a small office/branch office configuration. You could certainly use one of these for a home firewall solution, but you'd need a considerable amount of networking and network security experience to administrate it.





