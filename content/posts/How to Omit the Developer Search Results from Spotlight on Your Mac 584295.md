---
title: "Stop Annoying Developers from Taking Over Your Spotlight Search on Your Mac with This Simple Guide!"
ShowToc: true 
date: "2023-04-23"
author: "Thomas Arndt"
---
*****
Introduction
If you're a Mac user, you're likely familiar with Spotlight Search- a powerful tool that helps you quickly find files, apps, and other information on your computer. However, if you're a developer, there's a chance that your code projects and files are dominating your search results, making it difficult to find anything else. Here's a simple guide to help you stop annoying developers from taking over your Spotlight Search on your Mac.

Step 1: Exclude Developer Folders from Spotlight Search
The first step is to exclude developer folders from Spotlight Search. This can be done easily by following these steps:
1. Open “System Preferences” on your Mac.
2. Click “Spotlight” in the Preferences window.
3. Click on the “Privacy” tab.
4. Click on the “Add folder” icon in the bottom left.
5. Navigate to the folder you wish to exclude and select it.
6. Click “Choose.”

By adding your developer folder to the list of excluded items, Spotlight Search will now omit these files from its search results.

Step 2: Change Spotlight Preferences
You can also change Spotlight preferences to place less emphasis on developer files. To do this:
1. Open “System Preferences” on your Mac.
2. Click “Spotlight” in the Preferences window.
3. Click on the “Search Results” tab.
4. Uncheck the boxes next to “Developer,” “System Preferences,” and “Calculator.”
5. Drag the categories up or down to change the order in which the search results appear.

By making these changes, Spotlight will now prioritize other categories over developer files, resulting in more diverse search results.

Step 3: Use a Third-Party Search Tool
If you're still having trouble with your Spotlight Search, you may want to consider using a third-party search tool that can be customized to your preferences. Tools like Alfred, LaunchBar, and QuickSilver offer more advanced searching options and can be tailored to fit your specific needs.

Conclusion
Developers are a crucial part of the tech industry, but that doesn't mean their files should take over your Spotlight Search. By following these simple steps, you can ensure a better search experience on your Mac. Whether you choose to exclude developer folders, change Spotlight preferences, or use a third-party search tool, the choice is yours. Don't let annoying files distract you from finding the information you need. With these tips in mind, you can take back control of your Spotlight Search and improve your productivity.

{{< youtube tBIBSmTj74A >}} 



Spotlight is a great tool to search for files on your Mac, as it lets you quickly find a file no matter where it is saved. When the tool shows results, they are categorized for you to quickly get to the exact file you were looking for. While the search results are almost always the ones you wanted, sometimes you will see some developer files appearing there, and it is mostly because of Xcode. These developer files may not be of much use to you unless they were the ones you were trying to find.
 
If you wish to not see these developer results when you search using Spotlight, there is a way to omit these results.
 
## Omitting the Developer Search Results from Spotlight When Xcode Is Installed
 
If you have Xcode installed on your Mac, you can use the following steps to prevent its files from appearing in the Spotlight search.
 
1. Click on the Apple logo in the top-left corner of your screen and select “System Preferences…”
 

 
2. Click on “Spotlight” when the System Preferences panel opens.
 
3. When the Spotlight settings panel launches, click on the tab that says “Search Results.” That is where you can decide what results will appear.
 
On this panel what you need to do is uncheck the checkbox for “Developer.”
 
If you have uninstalled Xcode but the developer files still appear in the Spotlight search results, then you need to use the following steps to get rid of them.
 
## Omitting the Developer Search Results from Spotlight When Xcode Is Not Installed
 
Since Xcode has been uninstalled from your Mac, you will not see the “Developer” checkbox which you saw in the above section. That means you cannot control the developer results that appear in Spotlight.
 
To tackle the issue what you need to do is create a dummy Xcode app file, and that will force the system panel to show the “Developer” checkbox which you can then uncheck.
 
1. Launch Terminal on your Mac.
 
2. When Terminal launches, type in the following command and press Enter. It will change your current working directory to “/Applications.”
 
3. Next, type the following command into Terminal and press Enter. It will create a new app file called Xcode which tricks your Mac into thinking that this is the real Xcode app.
 
4. You will not get a confirmation or anything in Terminal, but the job is done.
 
5. Click on the Apple logo in the top-left corner of your screen and select “System Preferences…” Then click on the option that says “Spotlight” followed by “Search Results.”
 
You should be able to see the “Developer” checkbox which was not shown before. Uncheck it and close the panel.
 
## Conclusion
 
If you find developer files to be useless when you are looking for more important files using Spotlight, the guide above should help you stop those developer files from appearing in the search results.
 
Mahesh Makvana is a freelance tech writer who's written thousands of posts about various tech topics on various sites. He specializes in writing about Windows, Mac, iOS, and Android tech posts. He's been into the field for last eight years and hasn't spent a single day without tinkering around his devices.
 
Our latest tutorials delivered straight to your inbox




