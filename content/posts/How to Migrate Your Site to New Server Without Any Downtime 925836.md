---
title: "You Won't Believe How Easy It Is To Move Your Website To A New Server Without Losing A Single Visitor!"
ShowToc: true 
date: "2023-06-17"
author: "Luis Setzer"
---
*****
Moving your website to a new server can be a daunting task for any website owner. The fear of losing website visitors during the migration process can be overwhelming. Fortunately, with the right tools and knowledge, you can easily move your website to a new server without losing a single visitor. In this article, we will share with you the Hugo writing format on how to move your website to a new server successfully.

Step 1: Backup your website files and database

The first step in moving your website to a new server is to back up your website files and database. This is crucial, as any data loss during the migration process can result in a loss of website visitors, and ultimately, revenue. There are various tools available online that you can use to back up your website files and databases. However, ensure that you have a copy of your files and database in case of problems.

Step 2: Choose the right web host

The next step is to choose the right web host. A web host is a company that provides the hardware and software to run your website. When choosing a web host, consider their server location, security measures, uptime, and customer support. Also, ensure that the web host provides adequate resources to run your website. You can compare various web hosts based on their features and pricing.

Step 3: Move your website files and database

After selecting a web host, you can move your website files and database to the new server. This process involves transferring the website files and databases from the old server to the new one. You can use file transfer protocol (FTP) clients or website migration tools to transfer your website files and database. This process may take time depending on the size of your website.

Step 4: Configure your domain name server (DNS) settings

Before your website can be accessible to users, you need to configure your DNS settings. DNS is a system that translates domain names into IP addresses. The DNS settings contain information about the domain name, IP address, and other parameters relevant to your website. You can contact your domain registrar or web host for assistance in configuring your DNS settings.

Step 5: Test your website on the new server

Once you have moved your website to the new server and configured your DNS settings, you need to test your website on the new server. Check your website's functionality, links, and pages to ensure everything works correctly. You can also use website testing tools to check your website's speed, performance, and security.

Conclusion

Moving your website to a new server is easy if you follow the right steps. By backing up your website files and databases, choosing the right web host, transferring your website files and database, configuring your DNS settings, and testing your website on the new server, you can move your website without losing any visitors. Always seek professional help or contact your web host for assistance if you encounter any problems. With these tips in mind, moving your website can be a hassle-free process.

{{< youtube SptOnY4EoqM >}} 



If you own/manage a website, it is inevitable that you will have to change your web host one day. It could be due to the poor services of your current host, or that your site traffic exploded and you need to move on to a bigger host to accommodate the traffic. Whatever the case, most people will agree that it is never a joyous event to switch server. Your site will be down/unstable/inaccessible during the migration period and it could potentially lead to loss of sales. In this article, we are going to show you how you can migrate your site to a new server effortlessly and without any (or minimal) downtime. 
 
There are two main type of web hosting: Shared hosting and VPS/Dedicated hosting. Shared hosting means that the site is hosted in a shared environment and share the same IP address as hundreds (or even thousands) other sites. In shared hosting, the administrative control given to the user is usually very limited, so there is practically no way to manipulate the DNS feature. On the other hand, VPS/dedicated hosting gives the users absolute control over their servers and they can play around with the DNS feature to reduce the downtime. Let’s take a look below at how we can reduce the downtime for these two hosting environments.

Note: This tutorial assumes that you are using cPanel/WHM for your site hosting.

 
### Migrating site in a shared hosting environment
 
1. Back up all the files in the old server. You can easily do this with any FTP programs. If you are running a dynamic site (like WordPress), remember to backup your database as well (via the PhpMyAdmin->Export)
 
2. Set up the new server. Copy all the files from the old server to the new server. Pay extra attention to keep the file structure intact. For dynamic website, set up a new database (with the exact same name and password) and import the whole database in. Again, make sure that the database structure is intact.
 
For static website
 
3. Go to your domain registrar and change the nameserver to the new server. That’s it. The DNS will take 24-48 hours to propagate. During this period of time, your site will be unstable, oscillating between the new and old server, but since it is a static website, so your visitors won’t see any differences. Avoid making any changes during this period of time.
 
For dynamic website
 
4. You will need to configure your site to point to the database at the new server (some web hosts don’t allow remote access to their database, so check with your web host before you begin). Open your cPanel in the new server. Scroll down until you see the icon Remote MySQL. Click on it.
 

 
Enter your domain name in the field and click “Add Host“.
 
Log out of cPanel. In your old server, open your database configuration file (for WordPress, it is the wp-config.php file). At the field where it asks you for database hostname detail, change it to the IP address of the new server. In WordPress:
 
Save and upload to the old server.
 
5. Go to your domain registrar and change the nameserver to the new server. That’s it. While the DNS is propagating, your visitors will see content from the old server. However, as the database is pointed to the new server, all changes make on the site will be updated in the new server. Once the migration is done (24-48 hours time), your new server will be up and running with all the changes make during the migration.
 
### Migrating site in a VPS/Dedicated hosting environment
 
Before we start, it is assumed that all users have root access to their servers and both the old and new servers are running cPanel/WHM.
 
1. Log in to the WHM in the old server. On the left panel, scroll down till you see the “Edit DNS Zone” link. Click on it. 
 
2. Select the domain that you are migrating.
 
3. Look out for this field where it shows the domain name and the IP address. 
 
Change the 86400 (or 14400) to 300. Save the changes. 
 
What you have just done is set the TTL (Time To Live) value to 5 minutes so the DNS client will only cache the information in that record for 5 minutes (the common setting are 24 hours and 4 hours). Now you have to wait for 4-24 hours for this TTL value to propagate, depending on the original value.
 
4. Meanwhile, you can backup your old server and migrate all your files and databases to the new server. Test the new server to make sure that everything is working fine.
 
5. When you are ready to migrate the site, log into your old server WHM again. Go to the DNS zone page. This time, change the IP address to the new server’s IP. Save the changes. 
 
What you have just done is to set this as a relay and point it to the new server.
 
6. Go to your domain registrar and change the nameserver to the new server. That’s it. In as little as 5 minutes, your new server will be up and running. As in all cases, the DNS will take 24-48 hours to propagate, so meanwhile, keep your old server intact (do not delete any files or terminate the service) until the DNS propagation has finished. 
 
Let us know in the comments if this is useful to you.
 
Image credit: EJP Photo
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




