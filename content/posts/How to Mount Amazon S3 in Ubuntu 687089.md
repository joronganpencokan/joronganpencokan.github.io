---
title: "You Won't Believe How Easy It Is to Mount Amazon S3 in Ubuntu - Master the Process Now!"
ShowToc: true 
date: "2023-04-27"
author: "Kenneth Boutte"
---
*****
Title: You Won't Believe How Easy It Is to Mount Amazon S3 in Ubuntu - Master the Process Now!

Are you struggling to mount Amazon S3 on your Ubuntu system? Do you find the process too complicated and confusing? If yes, then this article is for you! In this article, we will show you how you can easily mount Amazon S3 in Ubuntu and access your files and folders from the command line. 

Amazon S3 is a cloud storage service provided by Amazon Web Services (AWS). It offers scalable, secure, and reliable data storage for businesses and individuals alike. To access your files and folders stored in Amazon S3, you need to mount the S3 bucket on your Ubuntu system.

Mounting Amazon S3 in Ubuntu is easier than you think. With just a few commands, you can mount the S3 bucket and access your files and folders. Here's how you can do it:

Step 1: Install S3FS

To mount Amazon S3 on Ubuntu, you need to install S3FS, a FUSE-based file system for Amazon S3. You can install it by running the following command:

```
sudo apt-get install s3fs
```

Step 2: Configure AWS Credentials

To access your Amazon S3 account, you need to configure your AWS credentials. Open the AWS Management Console, go to the IAM service, and create an IAM user with S3 permissions. Then, generate an access key and secret access key for the user.

Next, create a file named '.passwd-s3fs' in your home directory and add your AWS Access Key ID and Secret Access Key in the following format:

```
accesskey:secretkey
```

Save the file and make it secure by running the following command:

```
chmod 640 ~/.passwd-s3fs
```

Step 3: Create a mount point

Create a mount point for your S3 bucket by running the following command:

```
sudo mkdir /mnt/s3
```

Step 4: Mount the S3 bucket

Now it's time to mount the S3 bucket. Run the following command:

```
s3fs bucketname /mnt/s3 -o passwd_file=~/.passwd-s3fs -o umask=022 -o url=https://s3.amazonaws.com
```

Replace the 'bucketname' with your S3 bucket name. If your bucket name contains uppercase letters or special characters, replace them with '-' or '_' respectively. For example, if your bucket name is 'MyS3Bucket', use 'mys3bucket' as the 'bucketname' in the above command.

Step 5: Access your S3 files

That's it! Your S3 bucket is now mounted on your Ubuntu system. You can access your files and folders by navigating to the '/mnt/s3' directory. You can also use the command line to copy, move, or delete files in the S3 bucket.

Conclusion:

Mounting Amazon S3 in Ubuntu is not as complicated as it seems. With S3FS, you can easily mount your S3 bucket and access your files and folders. By following the above steps, you can master the process of mounting Amazon S3 in Ubuntu and make the most out of your cloud storage.

{{< youtube oyKaQfwrJxc >}} 



Note: This whole tutorial will be done in the terminal
 
## Installation
 
1. To get started, first install the dependencies.
 
Alternatively, if you are using GIT, you can checkout its Github page for more detail. 
 
3. Extract the file:
 
You should now find a “riofs-master” folder.
 
4. Enter the “riofs-folder” folder and compile it.
 
1. Before we can mount our bucket, we have to configure the configuration file for riofs. In your terminal:
 
This will copy the default configuration file to your local folder. You can change the destination folder if you want to.
 
Next, we need to add the security credential to the configuration file:
 
Scroll down the page till you see the AWS_ACCESS_KEY section. 
 

 
Uncomment that section and replace “###AWS_ACCESS_KEY###” with your access key and “###AWS_SECRET_ACCESS_KEY” with the secret key.
 
Save (Ctrl + o) and exit (Ctrl + x).
 
2. Change the permission for the riofs.conf.xml file.
 
To check if your bucket is successfully mounted, just list all the files in the mounted directory:
 
## More Configuration
 
There are a few things that you can set in riofs.
 
- --cache-dir: set a cache directory to minimize downloads
 - -o "allow_other": allow other users to access your bucket. You will need to enable the “user_allow_other” option in the fuse config file (/etc/fuse.conf)

 
## Conclusion
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




