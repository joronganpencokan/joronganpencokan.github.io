---
title: "Unveiling the Ultimate Hack: Watch YouTube Videos on VLC Player with Clipman in Linux Like a Pro!"
ShowToc: true 
date: "2023-04-29"
author: "Shane Waithe"
---
*****
Introduction:

Are you fond of watching YouTube videos on your Linux system but tired of buffering and slow loading time? Do you want to know about a simple yet effective way to watch YouTube videos without any hassle? If yes, then stick to this article till the end because today, we will unveil the ultimate hack of watching YouTube videos on VLC Player with Clipman in Linux like a pro!

What is VLC Player & Clipman?

VLC Player is a highly versatile media player that supports almost every audio and video format. The player is available for Windows, macOS, and Linux systems. It comes with a simple user interface and supports advanced features like video and audio streaming, DVD playback, and much more.

On the other hand, Clipman is a clipboard manager for Linux that helps you manage cut, copy, and paste operations. It allows users to easily copy and paste text, URLs, and files between applications. This tool works seamlessly with the native clipboard of the operating system, making it an essential productivity tool for many Linux users.

Why Watch YouTube Videos on VLC Player with Clipman in Linux?

Despite numerous benefits of watching YouTube videos directly on YouTube, there are various reasons why some users prefer to watch videos on VLC Player with Clipman in Linux. Firstly, it enables users to watch videos without any online distractions. Secondly, transferring YouTube videos to VLC Player can enable users to choose their desired playback speed, audio outputs, aspect ratio, and much more. Thirdly, VLC offers various unique features like frame-by-frame playback, zooming, and much more, that YouTube cannot provide on its app.

How to Watch YouTube Videos on VLC Player with Clipman in Linux?

The process of watching YouTube videos on VLC Player with Clipman in Linux is straightforward and does not require any complicated coding skills. You need to follow these simple steps:

Step 1: Install VLC Player and Clipman on your Linux system.

Step 2: Open your web browser and go to YouTube to select the video you want to watch.

Step 3: Copy the YouTube video URL from the address bar.

Step 4: Open Clipman and paste the copied URL into the clipboard manager.

Step 5: Right-click on the video URL in Clipman, and select the Open with VLC Player option.

Step 6: Once the video loads in VLC, you can control the playback settings according to your preference, and watch the video without any buffering or obstruction.

Conclusion:

In conclusion, watching YouTube videos on VLC Player with Clipman in Linux is a simple yet effective way to improve your video streaming experience. By using this hack, you can manage your video playback settings, avoid online distractions, and enjoy seamless playback. So, follow the mentioned steps and watch your favorite videos like a pro!

{{< youtube 7KhRg14_Jug >}} 



YouTube remains, for better or for worse, the most popular Internet destination for online videos. Through the years, it has evolved, amassing a massive collection of content and, strangely, mostly remained the same as far as its appearance and the way it works.
 
Although it has gained new features and received tweaks here and there, watching videos on YouTube remains a sub-par experience when compared to standalone media players.
 
Thankfully, VLC supports playing (almost) any online video stream, offering the best of both worlds. Unfortunately, though, playing a stream in it is a five-click process and then some. It doesn’t seem significant, but as the videos pile up, it gets tiresome. Soon you find yourself directly clicking on links in your browser because it’s simply easier.
 
What if there was a better way? Enter Clipman!
 
## What Is Clipman?
 
Clipman is a clipboard manager for XFCE that can be extended with custom actions, by using Regular Expressions – or RegEx for short.
 
Custom actions allow you to set it up in such a way that when “something” you define is copied to the clipboard, Clipman will spring into action. Your custom action, that is, as it “does” what “you told it to do” by setting up your custom action.
 
If that sounds too general, it’s because it is. You can set up Clipman to do almost anything, running any terminal command when it detects a specific string of text.
 
You need to look no further for a more specific example: it’s the very topic of this article. We’ll exploit Clipman’s functionality to detect all YouTube’s URLs that get copied to the clipboard and forward them to VLC. This will turn “watching online video streams in VLC” into a simple two-click process.
 
## Install VLC and Clipman
 
If they aren’t already installed in your system, add both VLC and Clipman to your local software collection. On Debian-based distros, you can do it with:
 
While Clipman is for XFCE, it should work in most other desktop environments. Run Clipman. If you are using a relatively new version of XFCE as your desktop environment, it should already be running and be accessible from your taskbar. Right-click on its icon and select Properties from the pop-up menu to enter its options screen.
 

 
Make sure all options but “Show QR-Code” are enabled.
 
## Taking Action – Or, Rather, Creating One
 
Move to the Actions tab – the list of all the re-actions Clipman already has set for specific strings of text. From here you can create new actions with the “plus” button. You can edit the existing actions by double-clicking on them or selecting them and clicking the “Edit” button (the second one). And, finally, you can delete any action you no longer need (last button with a recycle bin).
 
Click on the plus button to create your first action.
 
## Name and “Sync” Your Action
 
The first thing to do when creating an action in Clipman is giving it a name. Since you’ll probably keep adding similar actions of your own later, choose something easily recognizable and direct – we entered “VLC YouTube.”
 
Also, make sure to enable “Activate only on manual copy.” It might sound like something that restricts you, but it’s the other way around: this option allows Clipman to “see” the actual clipboard contents and act when it detects a string there. If this option was disabled, you’d have to explicitly call for Clipman to act on a text string instead of relying on it to pop up automatically.
 
## Detecting YouTube with RegEx
 
You can think of Regular Expressions as a logical way to define strings of text, and some relations between them, so that they can easily be detected.
 
Download Regular Expresions Cheatsheet here.
 
RegEx can be useful when, for example, renaming large groups of files with similar but not identical names. You could craft a RegEx “recipe” that selects all JPG files that start with “MakeTechEasier” in a folder,but not PNGs. Or in this case, any string that contains the YouTube URL:
 
Please note that you should copy it exactly as it is, including all parentheses. It might look a bit like alien hieroglyphics, but it’s one of the most straightforward RegEx recipes:
 
- The “\/” you see is not some ASCII form of the letter “v” but a backward slash – “\” – that “escapes” the forward slash used in URLs. Since the forward-slash is a special character in RegEx, when you want to treat it as an actual character, and part of the string you want to detect, you have to “escape it,” so you have to place a backward slash in front of it. Backward slashes are, as you might have guessed, “the way you escape things” in the world of RegEx.
 - The RegEx recipe is split into two parentheses: the first contains the beginning of any YouTube video URL: “http://www.youtube.com/watch.” The second one – “(.*)” – is the RegEx way to say “… everything that follows after.”

 
## Open in VLC: The Actual Action
 
The rest is more straightforward and direct: enter the name for the command you want to run whenever the RegEx string we defined is detected. We just entered “VLC URL” here.
 
Enter the actual command in the field that follows. This will be:
 
The first part is just running VLC itself. The \0 actually “maps to everything that matched our RegEx recipe.” In our case, YouTube URLs. Thankfully, VLC can directly open any YouTube URL, so we don’t have to do anything else but point it toward the URL we copied.
 
Remember to click on the “plus” button to add your command to the list, and then click OK and exit the Properties window to activate it.
 
## Send to VLC
 
While browsing YouTube, to directly open any video in VLC, right-click on its URL and choose “Copy Link Location.” A new pop-up will appear, this time from Clipman, that will have detected “it was a YouTube URL” and will allow you to choose the related action we set up. Click on it, and VLC will start streaming your video.
 
OK's real life started at around 10, when he got his first computer - a Commodore 128. Since then, he's been melting keycaps by typing 24/7, trying to spread The Word Of Tech to anyone interested enough to listen. Or, rather, read.
 
Our latest tutorials delivered straight to your inbox




