---
title: "Windows 10 Hackers Rejoice: Modify Your Action Center Like a Pro with This One Simple Trick for Note Buttons!"
ShowToc: true 
date: "2022-12-25"
author: "Clifford Allen"
---
*****
# Windows 10 Hackers Rejoice: Modify Your Action Center Like a Pro with This One Simple Trick for Note Buttons!

If you're a fan of hacking the Windows 10 operating system, then you're probably already familiar with the Action Center. This handy feature displays all of your notifications in one place, and makes it easy to take action on them. However, did you know that you can also modify the Action Center in some pretty cool ways? In this article, we'll show you how to use a simple trick to customize the Note Buttons in your Action Center like a pro.

## What are Note Buttons?

Before we dive into the trick, let's first explain what we mean by Note Buttons. When you receive a notification in your Action Center, you'll often see a button that you can click on to take action. For example, if you receive an email notification, you might see a "Reply" button. These buttons are called Note Buttons, and they allow you to quickly and easily respond to the notification without having to open the app that the notification came from.

## How to Customize Your Note Buttons

Now that you know what Note Buttons are, let's talk about how you can customize them. By default, Windows 10 comes with a set of pre-defined Note Buttons that are associated with different types of notifications. However, you can easily add your own Note Buttons for any app that you want.

Here's how to do it:

1. First, open up the Settings app by clicking on the Start menu and selecting "Settings".

2. Click on the "System" option, and then select "Notifications & actions" from the left-hand menu.

3. Scroll down until you see the "Quick actions" section. This is where you can add your own Note Buttons.

4. To add a new Note Button, simply click on the "+" button next to the "Add a quick action" heading. This will bring up a list of all of the apps on your system.

5. Select the app that you want to create a Note Button for, and then choose the action that you want to associate with the button.

6. Once you've selected your app and action, you'll have a new Note Button added to your Action Center that you can use to take action on that notification quickly and easily.

## Conclusion

Customizing your Note Buttons can really help streamline your workflow and make it easier to take action on your notifications. Whether you're a hacker or just someone looking to customize their Windows 10 experience, this simple trick is a great way to get more out of your Action Center. So why not give it a try today and see how you can improve your productivity?

{{< youtube KcN41s-wXKo >}} 



Windows 10’s Action Center has multiple quick action buttons that can perform various actions like enabling night light, opening the Settings app, creating quick notes, enabling quiet hours, modifying location settings, enabling tablet mode, etc. Of all the options, there is a Note button that allows you to quickly open the OneNote app. But what if you are not a fan of OneNote? Here is how you can map the Note button to open other note-taking apps.
 
Windows 10 has no built-in option to customize the button, but you can make a single change to Windows Registry to modify the Note button.
 
## Modify Note Button in Windows 10 Action Center
 
To open Windows Registry, press Win + R, type regedit and press Enter. Alternatively, you can also search for “regedit” in the Start menu and open it.
 

 
After opening the Registry Editor, navigate to the following location. To make things easier, you can also copy the below path, paste it in the address bar appearing on top of the window and press Enter. This action will automatically take you to the target key without fumbling around.
 
On the right panel, find and double-click on value “Uri”.
 
As you can see, the Uri is configured to open OneNote. For safe keeping, copy the default URI, paste it in a text file and save it. This allows you to easily revert back in the future.
 
To customize the button, you can either enter the URL of a web service or URI of an app. I will show both approaches; follow the one that matches your needs.
 
- For a web service, enter the URL of that note-taking service in the Value Data field and click on the “OK” button to save the changes. Since I regularly use Google Keep for simple note-taking and to-do tasks, I’ve entered the Google Keep URL. If you are using some other service like Evernote or Simplenote, then enter that URL.
 - For Windows Store apps, you have to enter the exact app URI, not the regular URL or file path. For instance, if you are using the Microsoft To-do app, enter “ms-todo:” in the Value Data field. For Evernote enter “evernote:,” for Wunderlist enter “wunderlist:,” etc.

 
Do take notice that these apps must be modern UWP apps, i.e. you cannot open regular “.exe” apps by entering the file path in the Value Data field, at least it didn’t work for me. Also, you need to have these apps installed beforehand from the Windows 10 Store, and the URI is different for each app. Generally, you can find the app-specific URI on the developer’s website.
 
If you want to restore the Note button’s default behavior, open the “URI” value, enter the previously saved URI and click on the “OK” button.
 
Do comment below sharing your thoughts and experiences about using the above method to modify the Note button.
 
Vamsi is a tech and WordPress geek who enjoys writing how-to guides and messing with his computer and software in general. When not writing for MTE, he writes for he shares tips, tricks, and lifehacks on his own blog Stugon.
 
Our latest tutorials delivered straight to your inbox




