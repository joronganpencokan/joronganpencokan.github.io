---
title: "You Won't Believe How Easy It Is To Install A Perl Module In Linux Without Root Permission!"
ShowToc: true 
date: "2023-06-30"
author: "William Webb"
---
*****
You Won't Believe How Easy It Is To Install A Perl Module In Linux Without Root Permission!

Perl is a popular programming language among developers who love building web applications, system administration scripts, and network programming. However, installing Perl modules on a Linux system can be a daunting task, especially if you don't have root permission.

Fortunately, there is an easy way to install Perl modules without root permission. In this article, we are going to explore this method, step-by-step.

Step 1: Set up a local Perl library directory

The first step is to set up a local Perl library directory where you can install the modules you need. This directory will be created in your home directory, so you don't need root permission to set it up.

To create the library directory, open your terminal and type the following command:

```
mkdir -p ~/perl5/lib/perl5
```

This will create the directory `~/perl5/lib/perl5` in your home directory.

Step 2: Configure Perl to use the local library directory

Next, you need to configure Perl to use the local library directory you just created. To do this, add the following line to your `~/.bashrc` file:

```
export PERL5LIB=~/perl5/lib/perl5:$PERL5LIB
```

This line will add the `~/perl5/lib/perl5` directory to the `PERL5LIB` environment variable, which Perl uses to find modules.

Step 3: Install the Perl module

Now that you have set up the local library directory and configured Perl to use it, you can install the module you need. To do this, use the `cpanm` command, which is a tool for installing Perl modules.

First, we need to install `cpanm`. To do this, type the following command:

```
curl -L https://cpanmin.us | perl - App::cpanminus
```

This will download and install `cpanm`.

Next, install the Perl module you need. For example, if you want to install the `DateTime` module, type the following command:

```
cpanm DateTime
```

`cpanm` will download and install the `DateTime` module to the local library directory you created earlier.

Step 4: Use the installed module

Now that you have installed the module, you can use it in your Perl code. For example, if you installed the `DateTime` module, you can use it in your code like this:

```perl
use DateTime;
my $dt = DateTime->now;
print $dt->strftime("%Y-%m-%d %H:%M:%S");
```

This will print the current date and time in the format `YYYY-MM-DD HH:MM:SS`.

Conclusion

As you can see, installing a Perl module in Linux without root permission is quite easy. By setting up a local Perl library directory and configuring Perl to use it, you can install any Perl module you need without the need for root permission. This method is especially useful for developers who don't have access to the root account on a Linux system.

{{< youtube _dOCtaBObg4 >}} 



Installing a Perl module is not a genius’ work, but getting it done without root access can be a challenging task (of course not impossible). You may face this situation when you do not have rights to standard directories where a Perl module is installed. In this tutorial we will see how we can install a Perl module without root or super user permission by installing it in separate non-standard directories.

 
## First Step
 
Before we proceed, let’s make a few things clear. First of all, I am assuming that you have Perl installed on your system. Apart from that, I’ll be using the following directories to install the Perl module:
 
You can create these directories (bin, man, man/man3 and lib) anywhere you want. We will use that path in the Perl configuration. You should replace the path used in the tutorial to your own directory path.
 
## Second Step
 
Now we need to define some variables to configure Perl locally. These configuration will be used to tell the Perl module where it should be installed. To do that, I would suggest that we write all those variables in one file and then use it while installing. It will save us time and effort in writing the lengthy commands and will be good for future use.
 
Let’s say we create a file “perl_local_config” in /home directory (the file can be created wherever you want):
 
Now let’s edit this file to set the configuration variables. Write the following variables in it:
 
## Third Step
 
Download the Perl module from the CPAN (or from wherever you want). Unzip it. Go into the module directory. Now, the standard steps of installing a Perl module is:
 
Since you do not have root access, the perl Makefile.PL will give error. And here comes the local configuration file to our rescue. Run these commands one by one:
 
If the Perl module depends upon other Perl module then the above command will generate error. In that case, download and install the modules on which it is dependent. Same procedure, which we are discussing here, would be followed.
 
All tests should pass successfully.
 
## Further troubleshooting
 
When running the Perl module may generate error like this:
 
That means that Perl is looking for your module in standard lib directory and not the one where you have installed it. To solve this error, add the locally created lib directory (/home/perl_modules/lib in the example) to the library path like this:
 
Do change the paths with your own directory path.
 
I hope that the tutorial was easy to understand and simple to follow. I also hope that you are now able to install Perl modules locally, without super user privileges, like a champ now. I would appreciate your feedback. Do subscribe to newsletter if you found the tutorial helpful and want to stay in touch for more updates. Enjoy :)
 
Abhishek is a Linux lover and Opens Source enthusiast. He takes a keen interest in day-to-day computer life and wishes to share his experience with others to make their computer experience better and easier. He is the owner of increasingly popular tech blog Computer And You and Open Source blog It's FOSS.
 
Our latest tutorials delivered straight to your inbox




