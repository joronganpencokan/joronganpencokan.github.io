---
title: "Unlock the Ultimate Secret to Effortlessly Convert XLS Files to CSV in Linux Command Line!"
ShowToc: true 
date: "2022-12-15"
author: "Manuel Bateman"
---
*****
Unlock the Ultimate Secret to Effortlessly Convert XLS Files to CSV in Linux Command Line!

Are you tired of manually converting XLS files to CSV format in Linux? Look no further! Here's the ultimate secret to converting XLS files to CSV format with ease, using the Linux command line.

First, you'll need to have the LibreOffice suite installed on your Linux system. LibreOffice is a powerful open-source office suite that includes a spreadsheet program (Calc) that can convert XLS files to CSV format.

Once you have LibreOffice installed, open the terminal and navigate to the directory containing the XLS file you want to convert. Use the following command to convert the XLS file to CSV format:

libreoffice --headless --convert-to csv filename.xls

This command will convert the XLS file to CSV format and save it in the same directory as the original XLS file. If you want to save the CSV file to a different directory, specify the path in the command.

For example, if you want to save the CSV file in the "Documents" folder, use the following command:

libreoffice --headless --convert-to csv --outdir ~/Documents/ filename.xls

This command will convert the XLS file to CSV format and save it in the "Documents" folder.

Now that you know the secret to effortlessly converting XLS files to CSV format in Linux, you can save time and focus on more important tasks. Give it a try and see how easy it is to convert XLS files to CSV format in the Linux command line with LibreOffice!

{{< youtube YqoWJzw7xz0 >}} 



Converting Microsoft Excel sheet (XLS file) to a Comma Separated file (CSV) is relatively very easy while using an Office product, but it could be a tedious task for programmers to do it in command line. The situation may arrive when you have a XLS file and you need to fill the database from it after formatting the data. Converting the XLS to CSV is the ideal way here as the CSV is the format that can easily be manipulated in any language, be it Shell, Perl, Ruby, Python or Java. In this post, we will see the best ways to convert the XLS file to CSV and we will also discuss the pro and cons of using these methods.

 
## catdoc (in C)
 
The first command line tool we are going to talk about is catdoc. The tool is written in C by V.B. Vagner.
 
### 1.1 How to install it:
 
Download the tool from here.  Go to your downloads directory and untar it. You can use the following commands (in case you are facing problem):
 
Now we have a catdoc-0.94.2 directory. Go inside this directory and run the following commands to install it:
 
The installation is an easy process and you should not face any problem here.
 
### 1.2 How to use it:
 
There are several option to run the command. I’ll tell the options that works best for the Microsoft Excel conversion:
 
Note the option “-s” and “-d” (stands for source and destination). These options are used to specify which character encoding is used in the source file and what would be the character encoding for the destination file. Here I have used cpl1252 which is Microsoft character encoding and 8859-1 which is used for Western European character encoding. You can use what other options are available by using the help command.
 
### 1.3 Pros and Cons:
 
Pros: Straight forward installation
 
Cons: No selective conversion in multiple sheet scenario, it coverts all the sheets present in the xls file (one workaround would be to explicitly specify a footer in each sheet and then use option -b in the command), problems with few European characters, problem with date fields (the date fields are messed up big times), messes with quotes.
 
## xls2csv (in Perl)
 
The second tool we are going to talk about is a Perl script xls2csv written by Ken Prows in Perl.
 
### 2.1 How to install it:
 
Download the script here. Gunzip and tar it like we did in previous section and go the extracted directory and use the following commands to install it:
 
Remember this Perl script uses a number of other Perl modules:
 
While installing xls2csv, it will give error that the mentioned perl modules have not been installed. It will ask you to download the modules. Download and install these modules when asked. All these module installation requires root privileges. If you do not have root access, then you should follow the instruction given here to install a Perl module.
 
### 2.2 How to use it:
 
The following command can be used to convert Microsoft excel to csv:
 
Option x and c (means xls and csv) are used to specify the input and output files where as b and a (means before and after) are used to specify the respective character encoding. We have use the same character encoding as in previous tool.
 
### 2.3 Pros and cons:
 
Pros: Good with western European character conversion and date fields, supports selective multiple sheet conversion,
 
Cons: Several Perl modules need to be installed, first cell should not be empty (otherwise it skips the whole row), messes with quotes
 
There are couple of other ways as well. Some scripts in Python and Java are also available to use but they are not as good as these two discussed here. I hope the article solves your problem. Question and suggestions are always welcomed. Cheers :)
 
Abhishek is a Linux lover and Opens Source enthusiast. He takes a keen interest in day-to-day computer life and wishes to share his experience with others to make their computer experience better and easier. He is the owner of increasingly popular tech blog Computer And You and Open Source blog It's FOSS.
 
Our latest tutorials delivered straight to your inbox




