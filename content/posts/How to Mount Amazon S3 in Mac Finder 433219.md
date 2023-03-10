---
title: "Revolutionize Your File Storage: Learn How to Mount Amazon S3 in Mac Finder like a Pro!"
ShowToc: true 
date: "2022-11-27"
author: "Roy Lockett"
---
*****
# Revolutionize Your File Storage: Learn How to Mount Amazon S3 in Mac Finder like a Pro!

Are you tired of constantly switching between different file storage systems on your Mac? Do you struggle with finding a reliable and secure way to store your files? Look no further than Amazon S3, a cloud-based file storage system that offers flexible, scalable, and secure options to store and retrieve your files.

Mounting Amazon S3 in Mac Finder can revolutionize the way you handle your file storage, making it easily accessible and organized from your desktop. In this article, we will walk you through the steps to mount Amazon S3 in Mac Finder like a pro!

## Prerequisites

Before we begin, make sure that you have the following prerequisites in place:

- An Amazon Web Services (AWS) account
- Access to an S3 bucket in your AWS account
- MacOS X 10.9 or later
- Fuse for MacOS installed on your Mac

You can download Fuse for MacOS from https://osxfuse.github.io/.

## Installing S3FS

S3FS is a Fuse-based file system that allows you to mount S3 buckets as local file systems. To install S3FS on your Mac, follow the below steps:

1. Open Terminal on your Mac.
2. Enter the command `brew install s3fs`.
3. Once the installation is complete, run the command `s3fs --version` to verify the installation.

## Configuring AWS Credentials

Now that you have installed S3FS, the next step is to configure your AWS credentials. Follow the below steps:

1. Open the AWS Management Console.
2. Navigate to the IAM service.
3. Create a new IAM user and give them S3 access.
4. Generate an access key and secret key for the IAM user.

## Mounting S3 in Mac Finder

Once the preceding steps are complete, it's time to mount your S3 bucket in Mac Finder. Please follow the below steps:

1. Create a folder where you would like to mount your S3 bucket as a file system.
2. Open Terminal on your Mac.
3. Enter the following command: `s3fs -o rw,user,suid,allow_other,uid=501,gid=20 myBucketName /Volumes/myS3BucketName`. 

You will need to replace `myBucketName` and `myS3BucketName` with your S3 bucket name and the folder you created to mount the bucket, respectively.

4. Once your bucket is mounted, go to the folder where you mounted your bucket to confirm that your S3 files are visible and accessible from your Mac Finder.

## Benefits of Mounting Amazon S3 in Mac Finder

1. Easy access to files: With Amazon S3 mounted directly in Mac Finder, it's easier to access, edit, and save files without navigating between different storage systems on your computer.

2. Increased Productivity: By having the S3 bucket located on your desktop, you can quickly drag and drop files between local and cloud storage, saving time and effort.

3. Improved organization: By having all files in one centralized location, it's easier to keep your files organized and easily accessible.

In conclusion, a well-organized and easily accessible storage system is integral to staying productive and efficient in today's digital age. By learning how to mount Amazon S3 in Mac Finder, you can revolutionize the way you handle your file storage, making it simple, secure, and easily accessible for all your storage needs.

{{< youtube tP5edaxBEEI >}} 



To get started, download ExpanDrive and install it to your Mac. After the installation, you should find an icon in the menu bar. Click on it to reveal all the cloud storage services that it supports.
 

 
ExpanDrive costs $49.95, but you can use the free trial for 14 days.
 
Download and install Transmit in your Mac. 
 
Launch Transmit. On the right panel, select “S3” at the top and enter your Access key and secret. 
 
Transmit comes with a 7-day free trial and its license key costs $34. 
 
## Conclusion
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




