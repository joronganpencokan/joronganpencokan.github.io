---
title: "Create Your Ultimate Discord Companion: Learn How to Make a Bot in Minutes!"
ShowToc: true 
date: "2023-07-03"
author: "Kevin Radabaugh"
---
*****
# Create Your Ultimate Discord Companion: Learn How to Make a Bot in Minutes!

Discord is a messaging and voice chat platform that has grown in popularity in recent years. Millions of people use it to connect with each other, form communities and have fun. But did you know that you can enhance your Discord experience by creating your own bot?

Bots are computer programs that can automate tasks, provide information, moderate chat and much more. They can be a great addition to any Discord server and help you manage it more efficiently.

In this article, we will show you how to create a bot for your Discord server in just a few minutes. What’s more, you don’t need any coding experience to do this!

## Step 1: Create a Discord Bot Application

To create a bot, you need to first create a Discord Bot Application. This can be done using Discord’s developer portal. Here are the steps:

1. Go to [Discord’s Developer Portal](https://discord.com/developers/applications) and click on ‘New Application’
2. Give your application a name and click on ‘Create’
3. Click on ‘Bot’ in the sidebar and then on ‘Add Bot’
4. Add a username and avatar for your bot and save the changes
5. Copy the bot token as you will need it later

## Step 2: Add the Bot to Your Server

Now that your bot application has been created, it’s time to add it to your Discord server. Here are the steps:

1. Go to the ‘OAuth2’ section in your bot application and select ‘bot’ in the ‘scopes’ options
2. Choose the permissions you want for your bot and copy the generated URL
3. Paste the URL in a new browser tab and select the server you want to add the bot to
4. Click on ‘Authorize’ and complete the captcha
5. Congratulations, your bot has been added to your Discord server!

## Step 3: Customize Your Bot

Your bot is now up and running, but you can customize it further to make it more useful. Here are some ideas:

1. Use a bot template: If you’re not sure where to start, you can use a bot template to get some inspiration. There are many templates available that you can customize to suit your needs.
2. Add commands: Commands are the main way users interact with your bot. You can add commands to perform specific tasks, such as displaying information or moderating chat.
3. Enable automatic responses: You can configure your bot to automatically respond to certain events or messages. For example, you can set it to welcome new members or respond to certain keywords in chat.

## Step 4: Test and Deploy Your Bot

Before deploying your bot to the public, it’s important to test it first. You can do this by running it on your own server or on a test server. This way, you can make sure it’s working properly and make any necessary changes before releasing it to your Discord community.

To deploy your bot, you can use a hosting service such as Heroku or Glitch. These services allow you to run your bot 24/7 and ensure that it’s always available to your users.

## Conclusion

Creating a bot for your Discord server can be a fun and rewarding experience. With just a few steps, you can create your very own bot that can help you manage your server and interact with your community. Whether you’re a beginner or an experienced developer, creating a bot is easy and accessible to anyone. So why not give it a try and create your ultimate Discord companion today!

{{< youtube Z8ND1XcUomU >}} 




Discord bots come in all shapes and sizes and can be used for a wide array of purposes that range from moderating user behavior on your server, automatically doling out punishments like muting or banning gamers who step out of line, to playing music for everyone to enjoy. 

 

While Discord bots are written in the JavaScript language, you don’t have to be an experienced coder to create them. In fact, the process is a lot less intimidating than you might imagine. Keep reading to learn how to make a Discord Bot that does your bidding.

 
The instructions below assume that you already have a Discord account and server in place. If not, you should set this up at discordapp.com before continuing. 
 
##   Download and Install Node.js  
 

Before getting started with Discord bot creation you’ll first want to install Node.js, a JavaScript runtime environment built on Google Chrome’s V8 engine. 

 
This tutorial is intended for users running macOS or Windows operating systems.
 
- Open a web browser and navigate to the official Node.js download page.
 - Select the appropriate installer package for your particular platform (macOS or Windows) and click on its download link.
 - Open the downloaded file and follow the on-screen prompts to install Node.js.
 - Once complete, launch the Command Prompt (Windows) or Terminal (macOS) application.
 - Type the following text at the prompt and press Enter on your keyboard: node -v
 - If a version number is returned, then Node.js is installed correctly. If not, revisit the above steps and ensure that installation is completed.

 
##   Create a Discord Application  
 

Now that you’ve gotten the prerequisites out of the way, it’s time to create a new application that your bot can later be added to. 

 

Open a web browser and navigate to the official Node.js download page.

 

Select the appropriate installer package for your particular platform (macOS or Windows) and click on its download link.

 

Open the downloaded file and follow the on-screen prompts to install Node.js.

 

Once complete, launch the Command Prompt (Windows) or Terminal (macOS) application.

 

Type the following text at the prompt and press Enter on your keyboard: node -v

 

If a version number is returned, then Node.js is installed correctly. If not, revisit the above steps and ensure that installation is completed.

 
- Open a browser and navigate to the Discord Developer Portal for your server, logging in if necessary.
 - Click New Application.
 - Enter a name for your new application in the edit field provided and click Create when ready.
 - The General Information screen for your new application should now be displayed, as shown in the accompanying screenshot. Select Bot, found in the left menu pane.
 - Click Add Bot.
 - A message will now appear, asking if you’re sure you want to add a bot to your application. Click Yes, do it!
 - Your new bot should now be created, with its information and options displayed in the BUILD-A-BOT section. Select Click to Reveal Token.
 - A long string of characters should now be displayed in place of the aforementioned link. Click Copy to send this token to your clipboard.
 - Paste this token into a text file for now using Notepad, TextEdit or a similar application.
 - You should delete this file and remove it from your Recycle Bin or Trash once you’ve completed this tutorial.

 
##   Coding Your Bot  
 

You’ve created a bot and added it to your server. Next comes the fun part, actually coding your bot to do what you want it to.

 

Open a browser and navigate to the Discord Developer Portal for your server, logging in if necessary.

 

Click New Application.

 

Enter a name for your new application in the edit field provided and click Create when ready. 

 

The General Information screen for your new application should now be displayed, as shown in the accompanying screenshot. Select Bot, found in the left menu pane.

 

Click Add Bot.

 

A message will now appear, asking if you’re sure you want to add a bot to your application. Click Yes, do it!

 

Your new bot should now be created, with its information and options displayed in the BUILD-A-BOT section. Select Click to Reveal Token.

 

A long string of characters should now be displayed in place of the aforementioned link. Click Copy to send this token to your clipboard.

 

Paste this token into a text file for now using Notepad, TextEdit or a similar application. 

 
You should delete this file and remove it from your Recycle Bin or Trash once you’ve completed this tutorial.
 
- Launch the Command Prompt (Windows) or Terminal (macOS) application.
 - Type the following text at the prompt and press Enter or Return on your keyboard: mkdir discord-test-bot
 - You can replace discord-test-bot with a name of your choosing.
 - Next, type the following command to traverse into your newly-created directory: cd discord-test-bot
 - The command prompt should now be updated, displaying the name of your bot’s folder project folder. Type the following and hit Enter or Return: npm init -y
 - A file named package.json should now be created in your project folder, as shown in the above screenshot. Type the following at your command prompt and hit Enter or Return: npm install --save discord.js
 - A list of WARN messages may now be displayed, which can be ignored as long as there are no errors (ERR) shown and the message toward the bottom of your Command Prompt or Terminal window reads “added 7 packages” or “added 8 packages”. Type the following and hit Enter or Return to create the auth.json file: touch auth.json
 - If you receive an error message when trying to use the touch command, you may first need to install it by entering the following syntax at your command prompt: npm install touch-cli -g
 - There will be a confirmation message noting that this file was created, but you can type ls -al (macOS) or dir (Windows) to see the contents of your project directory and confirm for yourself that auth.json is in fact listed.
 - Launch your preferred code or text editor such as Atom, Notepad or TextEdit, and navigate to your new project folder.
 - Open the auth.json file and enter the text shown in the accompanying screenshot, replacing AUTH-TOKEN with the authentication token string that you stored earlier in the tutorial. Save the file when done.
 - You must copy and paste the entire authentication string within the quotes shown. If you are missing even one character then your bot will not function as expected.
 - Return to the editor and create a new file in your project folder named bot.js.
 - The bot.js file will contain the code that dictates your bot’s behavior, which is completely up to you. For the purposes of this tutorial, however, we recommend using the following code and testing your bot end-to-end to make sure that everything is working as expected. You can then go back and edit the contents of bot.js as you see fit.
 - const Discord = require('discord.js');
 - const client = new Discord.Client();
 - const auth = require('./auth.json');
 - client.on('ready', () => {
 - console.log(`Logged in as ${client.user.tag}!`);
 - });
 - client.on('message', msg => {
 - if (msg.content === ‘hello’) {
 - msg.reply(‘hi!’);
 - }
 - });
 - client.login(auth.token);
 - This sample code will write a message to the command line console when the bot is called, confirming a successful login and containing your user tag.
 - Save your updated bot.js file.
 - Return to Command Prompt or Terminal and type the following to run your bot script: node bot.js
 - If you’ve done everything correctly up to this point, the following text should appear in your Command Prompt or Terminal window: Logged in as discord-test-bot#

 
##   Integrate the Bot Code With Your Server  
 

You're almost there...

 

Launch the Command Prompt (Windows) or Terminal (macOS) application.

 

Type the following text at the prompt and press Enter or Return on your keyboard: mkdir discord-test-bot

 
You can replace discord-test-bot with a name of your choosing.
 

Next, type the following command to traverse into your newly-created directory: cd discord-test-bot

 

The command prompt should now be updated, displaying the name of your bot’s folder project folder. Type the following and hit Enter or Return: npm init -y

 

A file named package.json should now be created in your project folder, as shown in the above screenshot. Type the following at your command prompt and hit Enter or Return: npm install --save discord.js

 

A list of WARN messages may now be displayed, which can be ignored as long as there are no errors (ERR) shown and the message toward the bottom of your Command Prompt or Terminal window reads “added 7 packages” or “added 8 packages”. Type the following and hit Enter or Return to create the auth.json file: touch auth.json

 
If you receive an error message when trying to use the touch command, you may first need to install it by entering the following syntax at your command prompt: npm install touch-cli -g
 

There will be a confirmation message noting that this file was created, but you can type ls -al (macOS) or dir (Windows) to see the contents of your project directory and confirm for yourself that auth.json is in fact listed. 

 

Launch your preferred code or text editor such as Atom, Notepad or TextEdit, and navigate to your new project folder.

 

Open the auth.json file and enter the text shown in the accompanying screenshot, replacing AUTH-TOKEN with the authentication token string that you stored earlier in the tutorial. Save the file when done.

 
You must copy and paste the entire authentication string within the quotes shown. If you are missing even one character then your bot will not function as expected. 
 

Return to the editor and create a new file in your project folder named bot.js. 

 

The bot.js file will contain the code that dictates your bot’s behavior, which is completely up to you. For the purposes of this tutorial, however, we recommend using the following code and testing your bot end-to-end to make sure that everything is working as expected. You can then go back and edit the contents of bot.js as you see fit.

 

const Discord = require('discord.js');

 

const client = new Discord.Client();

 

const auth = require('./auth.json');

 

client.on('ready', () => {

 

 console.log(`Logged in as ${client.user.tag}!`);

 

});

 

client.on('message', msg => {

 

 if (msg.content === ‘hello’) {

 

  msg.reply(‘hi!’);

 

 }

 

client.login(auth.token);

 
This sample code will write a message to the command line console when the bot is called, confirming a successful login and containing your user tag.
 

Save your updated bot.js file.

 

Return to Command Prompt or Terminal and type the following to run your bot script: node bot.js

 

If you’ve done everything correctly up to this point, the following text should appear in your Command Prompt or Terminal window: Logged in as discord-test-bot#

 
- Open a browser and navigate to the Discord Developer Portal for your server, logging in if necessary.
 - Select the application we created earlier from the MY APPLICATIONS screen, if prompted.
 - Click OAuth2, located in the left menu pane.
 - Scroll to the bottom of the screen until you locate the SCOPES section. Place a check mark next to the bot option by clicking on it once.
 - Scroll down again to the BOT PERMISSIONS section, placing check marks next to each permission type that your individual bot might need to function as expected. For the purposes of this example bot, we need the following permissions: Send Messages, Read Message History
 - Your particular bot will likely need a significantly different set of permissions. It’s important to understand what each permission entails before enabling it, so that bot users cannot exploit it for nefarious purposes.
 - Click Copy, located in between the SCOPES and BOT PERMISSIONS sections and accompanied by a long URL.
 - Open a new browser tab and paste this URL in the address bar, hitting Enter or Return to load the page.
 - The CONNECT TO DISCORD interface should now be displayed, as shown in the accompanying screenshot. Click Select a server and choose the name of your server from the list provided.
 - Click Authorize.
 - Place a check mark next to I’m not a robot by clicking on its check box once.
 - A confirmation message should now be displayed, noting that your bot is authorized and has been added to your server.

 
##   How to Test Your Bot on the Server  
 

You can test your bot by launching the Discord client and sending it commands or messages that correspond to your particular code. In this example, send the word hello to your bot and it should respond with hi!

 

Select the application we created earlier from the MY APPLICATIONS screen, if prompted.

 

Click OAuth2, located in the left menu pane.

 

Scroll to the bottom of the screen until you locate the SCOPES section. Place a check mark next to the bot option by clicking on it once. 

 

Scroll down again to the BOT PERMISSIONS section, placing check marks next to each permission type that your individual bot might need to function as expected. For the purposes of this example bot, we need the following permissions: Send Messages, Read Message History

 
Your particular bot will likely need a significantly different set of permissions. It’s important to understand what each permission entails before enabling it, so that bot users cannot exploit it for nefarious purposes.
 

Click Copy, located in between the SCOPES and BOT PERMISSIONS sections and accompanied by a long URL.

 

Open a new browser tab and paste this URL in the address bar, hitting Enter or Return to load the page.

 

The CONNECT TO DISCORD interface should now be displayed, as shown in the accompanying screenshot. Click Select a server and choose the name of your server from the list provided.

 

Click Authorize.

 

Place a check mark next to I’m not a robot by clicking on its check box once.

 

A confirmation message should now be displayed, noting that your bot is authorized and has been added to your server. 

 

Get the Latest Tech News Delivered Every Day




