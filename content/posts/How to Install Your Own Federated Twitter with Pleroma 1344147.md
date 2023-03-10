---
title: "Revolutionize your Social Media Game: Learn How to Create Your Own Federated Twitter with Pleroma!"
ShowToc: true 
date: "2023-01-22"
author: "Mandy Luna"
---
*****
Revolutionize your Social Media Game: Learn How to Create Your Own Federated Twitter with Pleroma!

Social media has become an integral part of our lives. It is how we connect with our friends, share our thoughts, and stay informed. However, the mainstream social media platforms are centralized, with power concentrated in the hands of a few companies. This centralized structure has several drawbacks like censorship, data privacy, and the control of the user experience. 

The solution to these problems lies in the federated social media model. In this model, multiple servers (or instances) run the same software, allowing users to connect with others across multiple instances. It's the concept behind the popular Mastodon platform. In this article, we'll learn how to create a federated Twitter-style social network using the Pleroma software.

What is Pleroma?

Pleroma is a free, open-source social media platform that lets you create your own federated social network. It's built on the same principles as Mastodon, but has a smaller footprint and requires less server resources. Pleroma's interface resembles Twitter, and it supports all the features you'd expect from a modern social media platform. However, being federated, it provides an alternative to the centralized social networks of big tech.

Setting up a Pleroma instance

Setting up a Pleroma instance is quite simple. Here's how you do it:

1. The first step is to get a VPS (Virtual Private Server) or a dedicated server. Pleroma requires a Linux server to run, so make sure to get a Linux-based server.

2. Once you have your server, you can install Pleroma by following the instructions on the official Pleroma installation guide.

3. After installation, you need to configure Pleroma. Pleroma comes with a built-in web interface that lets you set up your instance, including how your instance appears to other instances and what features to enable.

4. Finally, to make your instance federated, you need to connect it to the other instances. Pleroma uses ActivityPub, a standard protocol used by Mastodon and other federated social networks.

Benefits of using Pleroma

Pleroma offers several benefits over centralized social networks like Twitter:

1. Privacy: Since Pleroma is federated, it's decentralized, and there isn't a central database for storing user data. This means it's less vulnerable to hacks and data breaches.

2. Control: As the owner of your Pleroma instance, you have complete control over the data, rules, and user experience. You can customize your instance to cater to specific needs, including moderation, filters, and content policies.

3. Censorship-resistant: Federated social networks like Pleroma are resistant to censorship since there isn't a concentrated center of power to control what's being posted.

4. Customizability: Pleroma is highly customizable, and you can change everything from the interface design to the server settings to suit your needs. 

Conclusion

Pleroma provides social media users with an alternative to centralized platforms. By creating your own Pleroma instance, you take control of your social media experience and participate in a decentralized internet ecosystem. While it might take some time and effort to set up, running your Pleroma instance is a rewarding experience that can help revolutionize the way you use social media.

{{< youtube S57uhCQBEk0 >}} 



Microblogging is a wonderful way to express your thoughts. It is short, succinct and sweet. In this regard, Twitter has been one of the most popular microblogging platforms in the world. However, relying on this particular company for your microblogging needs not be the best solution for everyone.
 
Fortunately, there are alternatives such as Pleroma which is a self-hosted Twitter. This is a lightweight federated microblogging platform. Using federation allows the platform to communicate with other federated instances which means that you do not need to gather a lot of people for your own private Twitter to start sharing information. This article aims to help you get started with Pleroma.
 
## The Issue with Twitter
 
Twitter has been known to randomly ban accounts for vague policy infractions. If you are someone who have amassed years worth of posts in Twitter losing that history can be devastating. Not only that, Twitter has also been known to hand over user data to both advertisers and government agencies.
 
This makes Twitter an unsafe platform for people who either want to have complete control over their data or journalists that are reporting on controversial topics.
 
## What Is Federation and How Does it Work
 
One solution to this problem is building a social network through server federation. This is a system where you allow multiple servers running similar software to communicate with each other transparently.
 
Because of that, any federated server can act as a node for the whole network where you can access and participate with other servers.
 
In turn, this creates a resilient ecosystem that is able to easily adapt to any circumstance. For example, if a Pleroma server goes down it would not end the Pleroma federated network. It might reduce the amount of posts within the network but other servers will still be able to communicate with each other.
 
## How to Install Pleroma
 
Pleroma requires a number of things before you can start setting it up:
 
- First, you need to have a publicly discoverable machine. This could either be a machine in your home that you can port forward or a VPS that you purchased from a provider.Further, if you are using a VPS to install Pleroma you need to have root access to that VPS. This is because you will be installing packages that Pleroma requires for it to work properly.Lastly, you need to have a domain name. This is because certbot, the SSL certificate utility, will require a domain name to generate a certificate for your Pleroma instance.

 
With that in mind, this guide will be focusing on installing Pleroma on a Debian-based VPS from Digitalocean.
 
## 1. Set Up Your A and AAAA DNS Records
 
Before you start, it is wise to first link your domain name to the IP address of your VPS.
 
This ensures that any command that references your domain name below would resolve properly. As such, this becomes especially useful once you set up your SSL certificates later on.
 
- To link your domain name to your VPS’ IP address, you have to edit your domain name’s DNS record. While you might use a different domain registrar service than I do, the process of linking your domain name to your VPS’ address is largely the same.In my case, I linked my domain name: yetanotherpleromaserver.xyz to my Digitalocean VPS through Namesilo. To do that, I first accessed Namesilo’s domain manager window.

 
- From here, you need to click the domain name. This brings up the settings for that specific domain. Next, click the “DNS Records” link. This will show all the available DNS records for your domain name.

 
- Once done, I added an “A” resource to my DNS record by clicking the “A” link on the “Add/Edit a Resource Record” box on Namesilo’s record page.

 
- From there, the only thing that I needed to do was to add the IPv4 address of my Digitalocean VPS.

 
- The process of adding an “AAAA” record is also the same. However, instead of clicking the “A” link I will be clicking the “AAAA” link. Further, instead of adding the IPv4 address I will be adding the IPv6 address.

 
## 2. Obtain the Pleroma Dependencies
 
The next thing that you need to do is to download all of the packages that Pleroma requires. As discussed above, I am only going to highlight the installation process for Debian and Ubuntu-based Linux distributions. As such, I will be using apt to install all of the required packages.
 
With that in mind, Pleroma depends on three major programs: postgresql, elixir and erlang. Therefore, you need to install these programs as well as a couple more which will complement those three on doing their work.
 
To do that, you can run the following command:
 
## 3. Create the Pleroma User
 
With that done, the next thing that you need to do is to create the “pleroma” user account. This is the account that you will use to download and install the Pleroma package. Doing it this way ensures that the Pleroma program would not have any superuser access to your system.
 
To do this, you can run the following command:
 
- The -r option will set the “pleroma” user to be a system account rather than a user account.Further, the -s option will set login shell for this user to “false”. This makes sure that the pleroma user, by itself, cannot run any command from a shell.On the other hand, the -m and -d flags set the home directory for the “pleroma” user. The -m flag explicitly sets the account to have a home directory and the -d flag sets that directory to point to “/var/lib/pleroma”.Lastly, the -U flag creates a user group of the same name and adds the newly created Pleroma user to that group.

 
## 4. Download Pleroma
 
From there, you can now download the Pleroma package from their repositories. To do that, you have to first create the directory where the files will be downloaded to:
 
- The first command will create the “pleroma” directory where you will download all of the files for the program.The second command, on the other hand, will transfer the ownership of that folder from root to pleroma. This will, then, allow pleroma to read and write from this folder without any issues.

 
Once done, the next thing to do is to download the Pleroma source code itself. To do that, you need to use git:
 
## 5. Prepare and Install Pleroma
 
You can now go to the /opt/pleroma directory to start the process of installing the program:
 
From there, you need to run the Mix program to pull all the additional dependencies for Pleroma. To do that, you can run the following command:
 
Once done, you can now proceed with compiling and installing Pleroma. In that, you only need to run one command:
 
This command will do three things:
 
- First, the MIX_ENV=prod option will set the environment variable of the program to target a production setup. This means that the program will not contain any development tools and files.The gen option will create a configuration file that targets the environment variable that you have provided.Lastly, this command will also compile and install Pleroma from its source code. Because of that, this process will take some time depending on the hardware that you are running it on.

 
## 6. Configure the Pleroma Install
 
Once Pleroma is done compiling, it will then ask for some information about your server. 
 
- First, it will need the domain name that you want to use for the program. In my case, I used my domain name: “yetanotherpleromaserver.xyz”.

 
- From there, the configuration script will ask for the name that you want for your Pleroma server. In my case, I used the same name: “Yet Another Pleroma Server” for my server.

 
- Next up, input your admin email address. This should be a proper email that can receive and send emails.

 
- Now select whether you want your Pleroma instance to be searchable by search engines. This is useful if you want to create a public Pleroma instance that other people can join and login to. In my case, I wanted this server to be private so I selected “n”.

 
- After that, the script will ask whether you want to save your configuration in a database file. For the most part, you will want to select “yes” here and select the default options that it will ask for.

 
- Lastly, the script will require you to add some details about which port and address to listen to. If you are installing Pleroma on the same machine that you are configuring it on, it is safe to leave the defaults here.

 
## 7. Media-specific Configurations
 
- Now, the configuration script will require you to select where you want to save the media files that will be uploaded to the server. Similar to the settings above, it is safe to leave these on default.

 
- Next, decide whether you want to strip any geolocation from the EXIF data of the photos that you’ll receive. This is useful if you want to preserve the privacy of the uploader. Since I will only be using this as a private instance I selected “no” here.

 
- Further, you will have to decide whether you want to anonymize the filenames of the uploads. This is especially useful if you want to remove any association with the uploader and what they uploaded. In my case, I also selected “no” here.

 
- Lastly, the configuration script will let you choose if you want to create multiple copies of the files that are uploaded to your server. In my case, I selected “no”.

 
## 8. Finalize Your Pleroma Configuration
 
- You can now view your configuration file. This is located in “/opt/pleroma/config/generated_config.exs”. You can use less to view it:

 
- To finalize this configuration you need to rename this file as “prod.secret.exs”. You can do that by running the following command:

 
## 9. Start the Pleroma Database
 
- The next thing that you need to do is to start the database program. To do that, you can use the database that Pleroma provided. You can load that database by running the following command:

 
- From there, you can now link postgres and Pleroma by migrating the postgres database to Pleroma. To do that, you can run the following command:

 
## 10. Start Your Pleroma Server
 
Now, it’s time to run your Pleroma server. You can do this by running the following command:
 
However, this server is still inaccessible from the regular browser. To allow that, you need to first configure certbot and nginx.
 
### Configuring Certbot for Pleroma
 
- Configuring certbot is relatively straightforward. First, you have to create the folder where the certificates will be saved. You can do that by running the following command:

 
- With that done, you can now generate a certificate for your Pleroma server. To do that, you can run this command:

 
### Configuring Nginx for Pleroma
 
- From there, the next thing you need to do is to configure your nginx webserver for Pleroma. The Pleroma installation already provides a template that you can copy to nginx’s configuration directory. To do that, you can run the following command:

 
- Next, you then need to edit this configuration file to suit your Pleroma server. For most cases, this will only involve changing four variables: server_name, ssl_trusted_certificate, ssl_certificate and ssl_certificate_key.For the first variable, you need to change the “example.tld” value to the domain name of your server. In my case, I changed this to “yetanotherpleromaserver.xyz”.

 
- From there, the next three variables all point to the location of your domain’s SSL certificate. If you made your certificate through this guide, that path will be “/etc/letsencrypt/live/yourdomain.name/”.This is already provided by the nginx template and the only thing left to do is to change the “example.tld” value to your domain name.

 
- With that done, you can now enable your nginx configuration by creating a symbolic link to the active nginx directory. To do that, you can run the following command:

 
- After that, you can now start nginx by enabling its systemctl service:

 
## 11. Final Configurations
 
- From here, you can now configure the system service for Pleroma and create your first user. By default, Pleroma includes a systemctl template to enable its service through systemd. To use that template, you can run the following command:

 
- Now, you can then enable Pleroma through systemctl by running this command:

 
- Lastly, you can now create your first user for your Pleroma instance by running the pleroma.user command:

 
## Frequently Asked Questions
 
### 1. The pictures that I upload still has geolocation data in them. What did I do wrong?
 
This can be due to a number of things. However, the most common reason why this happened is because you do not have the exiftool package. For the guide above, exiftool was not a package that was installed by default.
 
As such, to remove the geolocation for the images that you upload, you need to add that package manually. To do that, you can run the following command:
 
### 2. I can’t generate a Letsencrypt Certificate. What did I do wrong?
 
This can also be due to a number of things. The most common cause for this, however, is that nginx is still running.
 
For the certbot command to work, you need to have the common web ports open and not taken by any program. To disable nginx, you can run the following command:
 
Image credit: Pleroma
 
Ramces is a technology writer that lived with computers all his life. A prolific reader and a student of Anthropology, he is an eccentric character that writes articles about Linux and anything *nix.
 
Our latest tutorials delivered straight to your inbox




