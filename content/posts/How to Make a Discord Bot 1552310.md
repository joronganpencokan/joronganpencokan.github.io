---
title: "Unleash Your Inner Programmer with this Step-by-Step Guide on Creating your own Discord Bot!"
ShowToc: true 
date: "2022-11-28"
author: "Jose Terman"
---
*****
# Unleash Your Inner Programmer with this Step-by-Step Guide on Creating your own Discord Bot!

Are you a gamer or involved in some other internet community? Chances are you’ve heard of Discord, a platform for gamers, user groups, and many others with communication features accessible by web, mobile, desktop app, and voice chat. Discord has a lot to offer, but what if you could make your experience even better? Did you know you can create your own Discord bot to automate simple tasks on your server?

Creating your bot is not as difficult as it may seem. Anyone can create their own bot using only a bit of coding knowledge and patience. In this step-by-step guide, we’ll be showing you how to create your own Discord bot using Node.js.

Before we dive in, let's talk about why you should consider creating a Discord bot for yourself. A bot can make life easier in many ways, such as automating moderation tasks or welcoming new users. It can even be used to generate content! You could write a bot for a multiplayer game that would give users information about their stats. A Discord bot could make your server more polished and attractive to others, and it’s a fun project for users familiar with coding.

Here’s how you can create your very own Discord bot:

Step 1: First things first, create your bot in the Discord Developer Portal

1. Log in to the Discord Developer Portal.
2. Create a new application by clicking the “New Application” button. Give your new application a name.
3. Click the “Bot” link on the left-hand side of the page.
4. Click the “Add Bot” button.
5. Customize your bot’s name and icon if you wish, then click the “Save Changes” button.

Step 2: Get your bot’s token

Once you’ve created your bot, you’ll need its token to add it to your server. Follow these steps to get the token:
1. Click on the “Bot” tab on the sidebar
2. Click the “Copy” button to copy your bot’s token to your clipboard.
3. **Important: Make sure you keep this token a secret!**

Step 3: Create your bot application

Now that we have our bot token, let's create our bot application. 

1. Open an IDE (Integrated Development Environment). We suggest using the popular Visual Studio Code.
2. Create a new folder on your computer to keep all of your bot’s files in one place.
3. Open a terminal inside your new folder.
4. In the terminal, run “npm init”. This will create a new package.json file in your folder.
5. Install discord.js by running “npm install discord.js” in your terminal.

Step 4: Write and Run Your Bot’s Code

It's now time to start writing your bot's code. Here are a couple of basic commands to get you started:

```javascript
const Discord = require('discord.js');
const client = new Discord.Client();

client.on('ready', () => {
  console.log(‘Bot is now online!’);
});

client.on('message', msg => {
  if (msg.content === 'ping') {
    msg.reply('pong');
  }
});

client.login('token');
```

In this example, our bot listens for a message that says “ping” and replies with “pong”. 

Once you’ve written your own code, run it by typing “node filename.js” in your terminal.

Step 5: Add Your Bot to Your Discord Server

Now that you’ve written your bot’s code, it’s time to add the bot to your Discord server. Follow these steps:

1. Navigate to the Discord Developer Portal.
2. Select your application.
3. Click the “OAuth2” tab.
4. Under the “Scopes” section, select “bot”.
5. Under the “Bot Permissions” section, select the permissions you’d like your bot to have. 
6. Copy the OAuth2 URL generated in the “scopes” section.
7. Visit the URL you copied in step 6 and follow the prompts to add your bot to your server.

Congratulations, you’ve now created and added a bot to your server! Keep in mind, this is just the beginning. Now that you have a basic understanding of creating and adding bots to your server, you can experiment with adding more commands and making your bot more effective.

Creating a bot is a rewarding experience that can be used in many different ways. Your bot can be used to automate tasks and manage moderation in your server, among other things. And best of all, it creates a sense of accomplishment knowing that you’ve created something from scratch. So go on, unleash your inner programmer and create your very own Discord bot today!

{{< youtube 1jtAWZK3Bbk >}} 



Creating a custom Discord bot is a fun and engaging way to sustain the interest of your community server. When you invite your friends over to your channel, the bot will manage their interactions in your absence. For example, if a user is misbehaving, the bot can kick him or her out. 
 
To do that, you have to acquaint yourself with some programming and steps to create your bot and add it to your server. The following guide simplifies what has to be done with easy-to-understand screenshots. 
 
## Creating Discord Bot on Developer Portal
 
Log in to your Discord account and go to the developer portal. Here, you can create a new bot “application.”
 
Give your application a desired name and click “Create.” 
 
In the next step fill in some details regarding what this application is all about. You can choose an app icon. Remember to save the changes. 
 
Now add a bot using the “build-a-bot” feature of the portal. 
 
Give your consent to adding a bot to the app. The action is irrevocable. 
 
After you complete the above steps, a wild bot is created. However, it is not ready to be shared yet. For that, you need to provide additional information. 
 
Make a checklist of what your bot can do. You should not give it administrator privileges, as then it can control your server. Feel free to let it mute or ban members, prioritize speakers, add reactions, embed links, manage nicknames, and much more. Each level of permission provided by you has its own unique ID you can see on the dashboard itself.
 
## Creating the Code for Your Discord Bot
 
If you are a programmer, you will want to modify the bot’s functions quite a bit. This demonstration uses node.js, a JavaScript runtime environment. Once installed for Windows, you may want to install “additional tools,” which can be done directly from the command terminal. It will install Chocolatey, Visual Studio, and other programs in Windows Powershell. 
 
Download and install Node.js for Windows x64 and then run the following specific program from the Start menu. It’s a Node.js command prompt. (Don’t run the other Node.js application file, as it has a different use.) 
 
Once the environment has been set up for using Node.js, you will have to install “discord.js with voice support” using the following code.
 
You should see a success status for the number of packages created. 
 
Install nodemon as shown below.
 
Go back to your Discord bot on your developer portal webpage. Click the icon for “click to reveal token,” and it will display an alphanumeric key, which is your private Admin. Don’t share the token with anyone, as it is easily hackable. 
 
Check the code example shown at the official Discord site. 
 
Instead of a token in the last line of code, copy-paste your own Discord bot token. 
 
Save the file as “Index.js” in any folder which is directly accessible from the Command prompt. It can have any name as long as it is a .js file. 
 
Now, to run the bot, enter the following code.
 
When it’s ready, the Node.js will then log you into your Discord API. There is also an editor mode in Node.js which you can access from .help option. This is where you can introduce further edits to your bot. 
 
## Adding the Bot to Your Server
 
Once your bot has been created, you will want to add it to your Discord server. For that, you will need a link such as the following:
 
 https://discordapp.com/oauth2/authorize?client_id=123456789012345678&scope=bot
 
The “client ID” is found in General information under the Application where you have saved the bot. 
 
In the below screen, you can see the client ID for the bot that was created in the first section. 
 
Open a browser and enter the link shared above. Simply replace the client ID with yours. You can choose the server where you can add the bot. 
 
If the bot is successfully created, you will see an “authorized” message which shows the app has been connected to your Discord server. If you have the Discord server installed for Windows, you should see an alert in the system tray as shown here. 
 
The created bot has been successfully added to the Discord server. 
 
Discord bots are an interactive means to build interest in your server. For more information on working with custom Discord bots, refer to this official manual. 
 
Have you created your own Discord bot? What was its purpose? Please share your ideas in the comments. 
 
Sayak Boral is a technology writer with over eleven years of experience working in different industries including semiconductors, IoT, enterprise IT, telecommunications OSS/BSS, and network security.  He has been writing for MakeTechEasier on a wide range of technical topics including Windows, Android, Internet, Hardware Guides, Browsers, Software Tools, and Product Reviews.
 
Our latest tutorials delivered straight to your inbox




