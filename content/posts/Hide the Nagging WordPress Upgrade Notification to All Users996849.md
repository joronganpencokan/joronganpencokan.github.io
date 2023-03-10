---
title: "Say Goodbye to Annoying Wordpress Updates - One Simple Trick to Hide The Notification from All Users!"
ShowToc: true 
date: "2023-04-02"
author: "Tara Meyers"
---
*****
# Say Goodbye to Annoying WordPress Updates - One Simple Trick to Hide The Notification from All Users!

As a WordPress user, it's common knowledge that updates are necessary. Updates bring bug fixes, security patches, improved features and functionalities that help keep your site in top shape. While the need for updates is clear, the habitual alert notifications of updates can be tiresome, especially if you're managing a site with multiple users. Fortunately, there's a simple trick that can help hide the notification from all users, and in this article, we'll show you how. 

## The Problem

By default, WordPress notifies you of updates through an alert box at the top of your dashboard. This notification is visible to every user with access to the dashboard, prompting them to perform updates. The issue with this system is that not all users are equal. Some users may not have the necessary expertise to perform an update or might only need access to a specific section of the dashboard. This unnecessary alert notification can be frustrating for non-web-savvy users and can cause confusion in their ability to navigate the dashboard.

## The Solution

Hiding the WordPress update notification is simple, thanks to the "Hide Update Notification" plugin by Samuel Aguilera. This plugin allows you to remove the update notification from the dashboard, preventing it from displaying automatically for all users. 

To install the plugin, follow these simple steps:

1. Log in to your WordPress dashboard.
2. Navigate to "Plugins" in your sidebar.
3. Click "Add New" and search for "Hide Update Notification" by Samuel Aguilera.
4. Install and activate the plugin.

Once you've completed these steps, the update notification will no longer appear in your dashboard. Instead, you'll be responsible for manually updating your website, and you'll need to ensure you stay up-to-date with the latest WordPress updates.

## Additional Functionality

If you're looking for more functionality beyond hiding the update notification, you can try the "Advanced Automatic Updates" plugin by Pionect Studios. This plugin allows you to manage automatic updates for WordPress core, plugins, and themes. With this powerful plugin, you can turn on and off automatic updates and select which types of updates to install automatically. 

## Conclusion

By taking advantage of the "Hide Update Notification" plugin, you can help improve the user experience for your less tech-savvy users while still ensuring your WordPress site receives the latest updates. Additionally, the "Advanced Automatic Updates" plugin provides you with more control over which updates are automatically installed. When it comes to managing your WordPress site, these simple additions can make a big difference.

{{< youtube 29jD2BcBX5w >}} 



If you are a regular WordPress user, you will definitely see the WordPress Upgrade Notification whenever a new version of WordPress is released. With the release of WordPress 4.6, you will see the message “WordPress 4.6 is available! Please notify the site administrator,” prompting you to upgrade to the newest version. This is all fine if you are the only user of your site. In instances where your site has multiple contributors or if you are building a WordPress project for your client, you might want to hide this nagging indismissable message for all users except the administrator (or a user who has the capability to perform the upgrade).
 
The good thing about WordPress is that it comes with many hooks and filters, so you can easily hook on a (php) function to modify the result. And this is how we are going to hide the nagging WordPress upgrade notification message.
 
Note: hiding the message doesn’t mean it is unnecessary to update WordPress. It is important to always keep your WordPress up to date.
 
1. Locate your theme folder and find the “functions.php” file.
 
2. Add the following function to the end of the file.
 
What the above code does is first check if the current user has the capability to update WordPress. If not, then it will remove the message from the queue and won’t show up in the Dashboard.
 
3. Save the functions.php file and upload to your server, replacing the old file.
 
That’s it. Only an administrator or a user with the capability to upgrade WordPress will see the Upgrade notification in the Dashboard.
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




