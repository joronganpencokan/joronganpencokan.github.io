---
title: "Revolutionize Your Blogging Game: Host Your Blog for FREE with Jekyll and Github Pages Now!"
ShowToc: true 
date: "2023-02-27"
author: "Alexandria Nichols"
---
*****
Revolutionize Your Blogging Game: Host Your Blog for FREE with Jekyll and Github Pages Now!

Blogging has become an essential part of our daily lives. It is a way to share our thoughts, opinions, ideas, and experiences with the world. However, running a blog is not always an easy task, especially when it comes to hosting. Hosting a blog requires technical skills, money, and time. But what if we told you that you could host your blog for free using Jekyll and Github Pages? Yes, you heard it right! In this article, we will explain how to revolutionize your blogging game and host your blog for free using Jekyll and Github Pages.

What is Jekyll?

Jekyll is a static website generator that allows you to create a website or blog using plain text files. It helps you to transform simple text files into a well-structured website. Jekyll is an excellent choice for bloggers who do not want to deal with the complexity of content management systems (CMS) like WordPress but still want a powerful and customizable website.

What is Github Pages?

Github Pages is a web hosting service that allows you to host your website or blog for free. It is based on the version control system Git, and it is connected to your Github account. Github Pages is a great choice for developers or bloggers who want to host their static websites, blogs, or documentation.

How to Host Your Blog for Free with Jekyll and Github Pages?

Step 1: Create a Github Account

The first step to hosting your blog for free with Jekyll and Github Pages is to create a Github account. Go to Github.com and sign up for a free account.

Step 2: Create a New Repository

After creating a Github account, the next step is to create a new repository. Go to the Github dashboard and click on the “New” button. Name your repository as “username.github.io”, where username is your Github username. This naming convention is essential for Github to recognize it as a Github Pages repository.

Step 3: Install Jekyll

The next step is to install Jekyll on your computer. Jekyll requires Ruby version 2.4.0 or higher. If you do not have Ruby installed on your computer, download and install it from Ruby-lang.org. After installing Ruby, open your command prompt or terminal and run the following command to install Jekyll:

```
gem install jekyll bundler
```

Step 4: Create a New Jekyll Site

The next step is to create a new Jekyll site. Open your command prompt or terminal and run the following command:

```
jekyll new my_blog
```

This command will create a new Jekyll site named “my_blog” in your current directory.

Step 5: Edit Configuration File

After creating a new Jekyll site, the next step is to edit the configuration file. Open your Jekyll site directory in a text editor and navigate to the _config.yml file. Edit this file according to your preferences. You can change the site title, description, author name, URL, and other settings.

Step 6: Choose a Jekyll Theme

Jekyll comes with default themes that you can use for your blog, or you can choose to use a third-party Jekyll theme. Navigate to the _config.yml file and change the theme. You can find Jekyll themes on Github or theme-gem-based Jekyll themes.

Step 7: Push Your Jekyll Site to Github

The final step is to push your Jekyll site to Github. Navigate to your Jekyll site directory on your computer, open the command prompt or terminal and run the following commands:

```
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/username/username.github.io.git
git push -u origin master
```

Replace the “username” with your Github username. This command will create a new Git repository, add all the files, commit them, add a remote Github repository, and push the files to Github. Wait for a few seconds, and your site will be live at http://username.github.io.

Conclusion

Hosting a blog has never been easier with Jekyll and Github Pages. In this article, we explained how to host your blog for free using Jekyll and Github Pages. We hope this article has helped you to revolutionize your blogging game and start your blog without worrying about hosting costs. Happy blogging!

{{< youtube -QA6HqZalBQ >}} 



If you’re looking to start a blog, chances are the first name you’ll encounter is WordPress. There’s a reason for that. WordPress is incredibly flexible and powers huge websites as well as small ones. The thing is, not every website needs such a powerful infrastructure, especially a simple blog.
 
Smaller, simpler, and cheaper options are available. GitHub Pages, for example, is free for personal use. Combine that with Jekyll, a static site generator, and you have everything you need for a blog. Even better, it’s free.
 
## Before you get started
 
You’ll be running Jekyll on your own computer, and only macOS and Linux are officially supported. We’ll be covering both operating systems here, and the Linux instructions may work with the Windows Subsystem for Linux running Ubuntu. That said, it hasn’t been tested.
 
You’ll also want access to a good text editor. TextEdit or GEdit will do, but you might want something more robust. We’ve taken a look at several great cross-platform text editors in the past.
 
## Things you should know
 
You should have at least a passing familiarity with the command line. Being familiar with git and GitHub will be necessary as well. If you’re not familiar, we’ve got a guide to git, and GitHub’s own documentation is excellent.
 

 
Finally, Jekyll utilizes Markdown, which lets you write in plain text but present your content in HTML to the user. You should be familiar with Markdown, or at least willing to learn it. This may sound daunting, but Markdown is easy to learn (we even have a cheatsheet for it).
 
## Install Jekyll and its dependencies
 
This has been tested on macOS Mojave and Ubuntu 18.04. If you’re running another version of either operating system, you may need to check the Jekyll website for further information.
 
### macOS
 
Before you can install Jekyll, you need to install the XCode command line tools with the following command:
 
Select Install and wait for the installer to complete. Now you can install Jekyll and Bundler:
 
When you run this command, you’ll see a warning similar to the one below:
 
WARNING:  You don't have /Users/YOURNAME/.gem/ruby/2.3.0/bin in your PATH, gem executables will not run.
 
Note the version number. Assuming the above message, run the following commands, substituting the correct version number if it differs:
 
### Ubuntu
 
Before installing Jekyll, you’ll need to install the build tools with the following command:
 
As with macOS, we want to install and run from the home directory instead of as root. Run the following commands:
 
Now install Jekyll and Bundler:
 
### Test your Jekyll installation
 
To make sure everything is up and running, run the following:
 
If everything has installed correctly, you’ll see a message with the version number. If instead you see a message like command not found, see the Jekyll documentation.
 
## Set up your new blog with Jekyll
 
Now that Jekyll is installed, creating your new blog is simple:
 
You can use any name you want in the above command instead of blog. This is simply the name of the directory Jekyll creates. Now cd to the directory that you just created, and run the following command:
 
This will launch your new blog about running locally on your computer. Open the URL displayed in your browser to take a look at the site. As you can see, there’s some work to do. Press Ctrl + C to stop.
 
## Customize your blog
 
To edit the site title and other information, open your blog directory and edit “_config.yml”. The various options here are fairly obvious. Now if you want, you can edit your home page, which is the “index.md” file, though this is optional.
 
To get started writing your first blog post, open the “_posts” folder and you’ll see a sample post. Open this up and edit it, or duplicate it to create a new post.
 
## Deploy your blog to GitHub
 
Now that your site is set up locally, it’s time to take it online. If you don’t have a GitHub account set up already, sign up and get git installed and configured on your computer. Next, create a new repository with the name username.github.io, replacing “username” with your GitHub username.
 
Now open your terminal and cd to your blog folder. Run the following commands.
 
Now you should be able to visit username.github.io and see your new blog. If it doesn’t show up right away, wait a few minutes and try again.
 
## Next steps
 
The steps above are just the basics to get you up and running. Jekyll has plenty to offer, so be sure to check out the documentation. There are also a number of themes available to spice up the look of your blog.
 
There are further steps to take with GitHub Pages too. Enabling HTTPS support used to be a more complex process, but now can be done in your repository settings. Setting up your own domain name is a simple process as well, and GitHub has a great guide on how to do so.
 
One final thing to keep in mind is that it’s a good idea to check site changes locally before committing them to your repository. Simply run the bundler command we used earlier to look at your site on your computer. This will help you catch everything from typos to Markdown syntax errors.
 
Kris Wouk is a writer, musician, and whatever it's called when someone makes videos for the web.
 
Our latest tutorials delivered straight to your inbox




