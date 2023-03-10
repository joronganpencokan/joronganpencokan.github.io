---
title: "Revolutionize Your Email Game: Learn How to Get Instant Login Notifications on Windows!"
ShowToc: true 
date: "2023-01-26"
author: "Tiffany Rivers"
---
*****
# Revolutionize Your Email Game: Learn How to Get Instant Login Notifications on Windows!

Are you tired of constantly refreshing your email inbox to check for new messages? What if you could receive instant notifications every time you log into your email account? With Windows, you can revolutionize your email game and stay on top of your messages with ease.

Here's how to get started:

## Step 1: Enable Login Notifications on Windows

The first step to getting instant email notifications is to enable login notifications on your Windows device. To do this, follow these simple steps:

1. Click on the Start menu button in the bottom left corner of your screen.
2. Select "Settings" from the menu.
3. Click on "Accounts."
4. From the "Accounts" menu, select "Sign-in options."
5. Under "Notifications," toggle the switch next to "Show me the Windows welcome experience" to turn on login notifications.

## Step 2: Set Up Your Email Account

Once you've enabled login notifications on your Windows device, it's time to set up your email account. Here's how to do it:

1. Open your preferred web browser.
2. Type in your email provider's website URL and log in to your account.
3. Navigate to your account settings.
4. Look for the "notifications" section.
5. Choose the types of alerts you want to receive. 

## Step 3: Start Receiving Notifications

Now that you've enabled login notifications on your Windows device and set up your email account, you're ready to start receiving notifications. Every time you log into your email account, you'll receive an instant notification on your Windows device.

By setting up your email account to send notifications for new messages, you can stay on top of your inbox and never miss an important email again. This feature is especially useful for those who receive a high volume of emails and want to stay organized and efficient.

In conclusion, revolutionize your email game by learning how to get instant login notifications on Windows. By following these simple steps, you can receive real-time updates on your email activity and stay on top of your messages with ease. Give it a try and experience the benefits for yourself!

{{< youtube Ut2w3cVxc7U >}} 



If you are managing multiple user accounts or multiple computers, then getting simple email notifications when a user logs in is a neat way to keep track of login activities. Moreover, it is also a good way to monitor a system that you don’t want others to log into.
 
Here is how you can make Windows send email notifications when a user logs into a computer.
 
## Make Windows Send Email Notifications on User Login
 
To make Windows send email notifications when a user logs in, we are going to use a third party program called SendEmail. SendEmail is a simple, portable, and lightweight command line email program that can send emails. Download the application from the official website, and only download the version that supports TLS.
 
Alternatively, you can also use Blat, but it doesn’t support TLS which is a requirement for almost any major email service like Gmail.
 
Once you’ve downloaded the file, extract it to someplace like Program Files in the C drive so that other users (if you have any) cannot access it without admin privileges. In my case, I just placed it in my E drive.
 

 
Now, search for Task Scheduler in the Start menu and open it.
 
After opening the Task Scheduler, click on the option “Create Task” in the right pane.
 
The above action will open the Create Task window. Here, enter the name of the task, description, and select the “Run whether the user is logged on or not” radio button. Don’t save the task yet.
 
Now, navigate to the Triggers tab and click on the “New” button appearing at the bottom of the window to create a new trigger.
 
In the “New Trigger” window select the option “At log on” from the drop-down menu next to “Begin the task,” and then make sure that the “Any user” radio button has been selected. Once you are done, click on the “Ok” button to save the changes.
 
Now, navigate to the “Actions” tab, and click on the “New” button to add a new action.
 
In the “New Action” window, enter the SendEmail application path under the “Program or Script” field, and then add the below command as the arguments in the “Add arguments” field.
 
While adding, don’t forget to replace “yourEmail@gmail.com” with your actual email address and PASSWORD with your actual email account password. If you want to you can also edit the email subject [-u] and the message part [-m].
 
Note: if you are using other email services, then you also have to change the SMTP server address and the port number.
 
Here is what the command line options actually mean.
 
- -f  – From email address
 - -t – To email address
 - -xu – Username
 - -xp – Email account password
 - -s – SMTP server address with port number
 - -u – Email subject
 - -m – Email body

 
Once you are done with the changes, click on the “Ok” button to save the changes.
 
This is how it looks after adding the said action to the task.
 
If you are adding this task to a laptop or something of that sort then you might want to uncheck the “Start the task only if the computer is on AC power” checkbox so that the task can run even when the system is running on battery.
 
Once you are done with everything, just click on the “Ok” button to complete the procedure.
 
If you want to test the task, simply select the task in the middle pane of the Task Scheduler, and then click on the “Run” button, and this should send the email.
 
That’s all there is to do. Every time a user logs into the system, you will receive an email notification (provided that your system is connected to the Internet).
 
Do comment below sharing your thoughts and experiences about using the above method to receive email notifications when someone logs into your system.
 
Vamsi is a tech and WordPress geek who enjoys writing how-to guides and messing with his computer and software in general. When not writing for MTE, he writes for he shares tips, tricks, and lifehacks on his own blog Stugon.
 
Our latest tutorials delivered straight to your inbox




