---
title: "Unlock The Secret To Launching Your Website In Seconds With This Revolutionary Method - How To Move Wordpress From Localhost To Production Server!"
ShowToc: true 
date: "2023-05-26"
author: "Maria Webre"
---
*****
# Unlock The Secret To Launching Your Website In Seconds With This Revolutionary Method - How To Move Wordpress From Localhost To Production Server!

If you're looking to launch your website, you're going to want to know about this revolutionary method. With it, you can move your WordPress site from localhost to a production server in no time at all. 

The process is simple and efficient, but it's important to follow the steps carefully so you don't lose any data along the way. Here's how to do it.

## Step 1 - Export the Database

The first thing you need to do is export the database from your localhost. This is where all your website data is stored, so it's essential that you take a backup of it.

To export the database, go to your localhost phpMyAdmin, select the database you want to export, and choose the "Export" option. This will generate a .sql file that you can download.

## Step 2 - Create the Production Server Database

Next, you need to create a new database on the production server. This can be done through cPanel or any other control panel that your hosting provider offers.

Once you've created the database, you need to import the .sql file that you exported in Step 1. Go to phpMyAdmin on the production server, select the database you created, and choose the "Import" option.

## Step 3 - Upload Files to the Production Server

Now that the database has been created and populated, it's time to upload your WordPress files to the production server. This includes all your website themes, plugins, and media.

You can do this using an FTP client like FileZilla. Connect to the production server using FTP credentials provided by your hosting provider, and upload everything to the root directory of your website.

## Step 4 - Update the Config File

Once your website files are uploaded, you need to update the WordPress config file to match the production server credentials. This is important to ensure that your website is able to connect to the new database.

To do this, locate the wp-config.php file in the root directory of your website and update the database name, username, and password to match the production server credentials.

## Step 5 - Test Your Website

Finally, it's time to test your website on the production server. Navigate to your website's URL and check that everything is working as it should be. 

If you've followed all the steps carefully, your website should now be successfully migrated from localhost to the production server.

## Conclusion

Migrating your WordPress site from localhost to production server doesn't have to be a complicated process. By following this revolutionary method, you can launch your website in seconds and start reaching your target audience.

Export the database, create the production server database, upload files to the production server, update the config file, and test your website. These easy steps will ensure that your website is set up correctly and ready to go live.

{{< youtube tIurrwfsCOg >}} 



WordPress is arguably the most used CMS in the world. From simple personal blogs to complex ecommerce sites, it has proven to be a winner. This being the case, many developers often create their WordPress website on a local host or personal computer, then finalize development before transferring to a live server and making it available to the world.
 
If you belong to this group of people and have finished the development on the localhost, here are the steps to move your WordPress from localhost to a live server.
 
Note: there are plugins that can automate this process. This tutorial will cover the manual steps without requiring the help of a plugin.
 
## Create new database on live server
 
If your web host comes with cPanel, log in to the Cpanel, and click on “MySQL databases” in the Databases section.
 

 
Under the new database text box, name your database and click the “Create Database” button. On the new window that is displayed, click “Go back.”
 
### Create new database user
 
In the next window you have to fill the textbox with a username and (strong) password, then click the “Create user” button. Record the username and password, as you will need it later.
 
Once again, hit “Go back” in the newly displayed window.
 
### Add user to database
 
Scroll down to “Add user to database,” select the user just created from the user dropdown list and also select the database just created from the database dropdown list. Next, click the “Add” button.
 
On the next window that opens, click the “All Privileges” checkbox, followed by the “make changes” button. Once again, click “Go Back” on the window that opens.
 
In the window that is displayed, double-check to see that your database contains the user you have just created. Once you are done, click on the Home button at the topmost left corner of the page.
 
## Migrate database from localhost
 
On the local host open phpMyAdmin, or whatever database management program you are using.
 
Locate your WordPress database.
 
Select the database, scroll down and click on “Check all.”
 
On the “Select with” dropdown menu, select “Export.”
 
In the next screen ensure that the format is on SQL, then click on “Go.” Save the exported database with the extension “.sql.”
 
### Importing the database
 
Go back to cPanel on your live server, and under “Databases” click on “phpMyAdmin.”
 
On the left pane you should see a list of databases. From this list click on the name of the database you created at the start of the tutorial and click “Import.” Navigate to the sql file you saved on your local computer and import.
 
If everything went well, it should bring you back to the phpMyAdmin main screen. You are now done migrating the database to the live server.
 
## Move localhost files to Cpanel
 
In your localhost, open your file manager and navigate to the WordPress folder (the folder that contains the “wp-admin,” “wp-content” and “wp-includes” folders). Compress the whole WordPress folder into a zip file.
 
In the cPanel in the live server, open the “File Manager” under the “Files” section. Select “Document root for” and make sure the domain you need to move your website to is selected and hit “Go.”
 
Make sure in the next window that “public_html” is selected on the left pane. Click on “Upload.”
 
Navigate to the location of the compressed zip file and upload it. Once complete, click the “Back to” link.
 
Your zip file at this point should display as a file in your “public_html” folder. If it doesn’t, click “Refresh.”
 
Select the zip file and click “Extract” at the top-left corner. Once the extraction is complete, delete the zip file.
 
## Editing the wp-config File
 
The last and final step is to edit the wp-config.php file to change all local host settings to production settings.
 
Return to your “public_html” in the File Manager. Select the file “wp-config.php,” and click “code editor.”
 
Replace the database name with the name of the database you created in your cPanel. Also, change the “DB_USER” and “DB_PASSWORD” to the one that you created earlier.
 
Check for the “WP_HOME” and “WP_SITEURL” values. If they don’t exist, add the following lines to the wp-config.php file:
 
Do remember to change the “your-live-url” to your actual domain URL.
 
Save the wp-config.php file and exit.
 
Once this is done, type your domain name in the address bar of your browser, and your site should be up and running. Go through every single page and log in to the admin panel to make sure everything is working fine. If not, refer to this tutorial to troubleshoot your WordPress installation.
 
## Conclusion
 
This is a comprehensive tutorial, and it may seem confusing. But after repeating this process once or twice, it becomes easy to follow for all your WordPress installations. Also, this method is more advisable when you do not have very large databases to upload.
 
Afam is a writer with a passion for technology amongst many other fields. Aside from putting pen to paper, he is a passionate soccer lover, a dog breeder and enjoys playing the guitar and piano.
 
Our latest tutorials delivered straight to your inbox




