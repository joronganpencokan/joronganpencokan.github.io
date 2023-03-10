---
title: "Say Goodbye to YouTube Clutter: The Ultimate Hack to Mass Unsubscribe Channels Instantly!"
ShowToc: true 
date: "2023-06-02"
author: "James Dangelo"
---
*****
Say Goodbye to YouTube Clutter: The Ultimate Hack to Mass Unsubscribe Channels Instantly!

If you spend considerable time on YouTube, then you know how annoying it is to see your feed cluttered with unwanted channels. From those channels with content you no longer have an interest in to inactive channels, these subscriptions fill your dashboard with irrelevant content that you would rather not see.

However, there is good news for those who want to clean their YouTube feed without having to spend hours on it. This article provides the ultimate hack to mass unsubscribe YouTube channels instantly.

Firstly, you will need to go to your YouTube homepage and click on the “Subscriptions” tab located on the left-hand side of the page. A list of all the channels you have subscribed to will appear on the screen. 

Next, press “control/Command + Shift + K” on your keyboard. This command will open the console window, which will allow you to apply a JavaScript code that will perform our ultimate hack. 

Then, you will need to copy the following code and paste it into the console window:

var x = document.querySelectorAll("[aria-label^='Unsubscribe from']"); 
for (var i = 0; i < x.length; ++i) { x[i].click(); }

Finally, hit the enter button, and voila! The script will instantly click on every “unsubscribe” button on the page, resulting in the system automatically unsubscribing you from all the channels you are presently subscribed to!

In less than a minute (depending on how many channels you have subscribed to), you will have wiped out all the unwanted channels from cluttering your YouTube feed. You can now enjoy a more streamlined viewing experience with improved browsing, and have more relevant videos found within your reach.

Bear in mind, however, that the ultimate hack function may not work in every instance, and certain factors may affect its working nature. For example, your computer must have the necessary software patches and scripts to execute the command successfully. Also, it's essential to note that this solution does not cover channels you may be subscribed to on platforms other than YouTube, such as Google Chrome.

In conclusion, the ultimate hack we have discussed in this article is the perfect solution for any individual who wants to cut down on YouTube clutter. By utilizing the straightforward process that we have provided, you can begin enjoying a cleaner and more relevant YouTube feed in no time.

{{< youtube OXBnkIDUtzw >}} 



YouTube is one of the most used and the most popular video streaming platforms. So, if you are home alone or super bored while traveling, YouTube is always there to entertain you. There are millions of content creators on this platform that create engaging content for their subscribers. You get the option to subscribe to your favorite content creators on YouTube to get regular updates about their latest posts.
 
However, it is possible that you subscribed to a number of YouTube channels some time ago; but no longer watch any of those. Since these channels are still subscribed, you will keep receiving tons of notifications. The solution to this problem is to unsubscribe the said channels individually. Wouldn’t it be a hassle? Wouldn’t it be extremely time-consuming?
 
Hence, the better option is to Mass Unsubscribe from these channels. Unfortunately, YouTube does not support any mass unsubscribe feature. Fortunately, there is a workaround to this problem. Through this guide, you will learn how to mass unsubscribe YouTube channels at once.
 

 
## How to Mass Unsubscribe YouTube Channels at Once 
 
Follow any of the following methods to unsubscribe from the YouTube channels that you no longer watch.
 
Contents
 
- How to Mass Unsubscribe YouTube Channels at Once
 - Method 1: Unsubscribe YouTube Channels Individually
 - Method 2: Mass Unsubscribe YouTube channels

 
### Method 1: Unsubscribe YouTube Channels Individually
 
Let us first discuss the steps to unsubscribe from YouTube channels.
 
Doing so for all subscribed channels would consume a lot of your time and effort. Since YouTube does not offer any feature to mass unsubscribe from multiple channels simultaneously, most users follow this method. This option would be beneficial if you want to choose specifically which channels to retain and which to get rid of.
 
On Desktop Browser
 
If you are using YouTube on your desktop, you can follow the given steps to manage your subscriptions. 
 
1. Open your web browser and navigate to youtube.com.
 
2. Click on Subscriptions from the panel on the left.
 
3. Click on MANAGE visible on top of the screen, as shown below.
 
4. You will get a list of all your subscribed channels in alphabetical order. 
 
5. Start unsubscribing to all the unwanted YouTube channels by clicking on the grey SUBSCRIBED button. Refer to pic below for clarity.
 
6. In the pop-up box that now appears, click on UNSUBSCRIBE, as depicted. 
 
Also Read: How to Change Your YouTube Channel Name
 
On Mobile App
 
If you are using the mobile YouTube app, follow these steps to unsubscribe: 
 
1. Open the YouTube app on your device and tap on the Subscriptions tab from the bottom of the screen. 
 
2. Tap ALL from the top-right corner of the screen, as shown. You can view all your subscriptions in A-Z, the Most relevant, and New activity order. 
 
3. Tap MANAGE from the top-right corner of the screen.
 
4. To unsubscribe from a YouTube channel, swipe LEFT on a channel and clicked on UNSUBSCRIBE, as depicted below. 
 
Also Read: How Do I Unsubscribe from Quora Digest
 
### Method 2: Mass Unsubscribe YouTube channels
 
This method will unsubscribe all the subscribed YouTube channels on your account at once. Therefore, proceed with this method only if you want to clear all the subscriptions.
 
Here is how to mass unsubscribe on YouTube at once:
 
1. Open any web browser on your desktop or laptop. Head to youtube.com 
 
2. Navigate to Subscriptions > MANAGE as instructed earlier. 
 
3. A list of all the channels subscribed from your account will be displayed. 
 
4. Scroll down till the end of the page and right-click anywhere on the empty space. 
 
5. Select Inspect (Q) option. 
 
6. A new window will appear on top of the bottom of the Manage Subscriptions page. Here, switch to the Console tab, which is the second tab in the list. 
 
7. Copy-paste the given code in the console tab. Refer to pic below.
 
var i = 0;

var myVar = setInterval(myTimer, 3000);

function myTimer () {

var els = document.getElementById(“grid-container”).getElementsByClassName(“ytd-expanded-shelf-contents-renderer”);

if (i < els.length) {

els[i].querySelector(“[aria-label^=’Unsubscribe from’]”).click();

setTimeout(function () {

var unSubBtn = document.getElementById(“confirm-button”).click();

}, 2000);

setTimeout(function () {

els[i].parentNode.removeChild(els[i]);

}, 2000);

}

i++;

console.log(i + ” unsubscribed by Saint”);

console.log(els.length + ” remaining”);

}
 
8. After pasting the above code into the console section, hit Enter and wait for the process to complete. 
 
9. Finally, your subscriptions will start to disappear one-by-one.
 
Note: You may encounter errors while running the code in the console.
 
10. If the process slows down or gets stuck, refresh the page and rerun the code to mass unsubscribe the YouTube channels.
 
Also Read: Fix Youtube Not Working Issue on Chrome
 
Q1. How do I unsubscribe to multiple YouTube channels?
 
YouTube does not have any feature that allows you to unsubscribe from multiple YouTube channels at once, but you can easily manage and unsubscribe from YouTube channels one by one. All you have to do is go to the subscriptions section and click on MANAGE. Finally, click on UNSUBSCRIBE to remove specific channels from your subscription.
 
Q2. How do I mass unsubscribe on YouTube?
 
To mass unsubscribe on YouTube, you can run a code into the console section on YouTube. It can be a bit tricky, but you can follow our detailed guide to run the code for unsubscribing to YouTube channels at once.
 
Recommended:
 
- 2 Ways to Cancel YouTube Premium Subscription
 - How to Delete Multiple Instagram Photos at Once
 - How to Fix YouTube Comments Not Loading
 - How to Leave a Discord Server

 
We hope our guide on how to mass unsubscribe YouTube channels at once was helpful, and you were able to get rid of all the unwanted subscriptions on YouTube. If you have any queries or suggestions, let us know in the comments below.




