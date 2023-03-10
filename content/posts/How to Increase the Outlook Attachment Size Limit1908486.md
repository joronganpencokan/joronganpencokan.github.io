---
title: "Boost your productivity by increasing the attachment size limit in Outlook! Click now to learn how!"
ShowToc: true 
date: "2022-11-17"
author: "Dean Gonzales"
---
*****
# Boost Your Productivity by Increasing the Attachment Size Limit in Outlook! Click Now to Learn How! 

Are you tired of sending large files through different sharing platforms and not receiving timely responses from your coworkers? Outlook is the perfect platform to manage your professional communication and stay organized. However, its default attachment size limit can be a productivity killer. 

With Outlook, you can attach files up to 20 MB in size. While it may seem like plenty, when working with high-quality photos, videos, slideshows, or numerous attachments at once, you can quickly reach this limit. Moreover, Outlook also adds its overhead to the attachment, which reduces its total size. 

Thankfully, there is a way to increase the attachment size limit on Outlook, and we are happy to provide you with a step-by-step guide. 

## Step-by-Step Guide 

Before you begin, ensure that you have the latest version of Outlook for your device. This guide is geared towards Windows users, but the steps should be similar on other operating systems. 

1. Launch Outlook on your device 
2. Click on the File tab on the top left corner 
3. Click on Options, which is located below the File tab 
4. A new window with options for Outlook will open; click on ‘Mail’ tab. 
5. Scroll down until you see ‘Send messages’ section and locate the Maximum attachment size box. 
6. Change the value to the desired size, which should not exceed 100 MB. 
7. Click on ‘OK’ to save changes. 

Congratulations! You have successfully increased the attachment size limit in Outlook. You can now send larger files without the need for additional sharing platforms. 

It is essential to remember that larger attachments can also slow down the email sending and receiving process. You may also find that some email providers have their attachment size limits. If you encounter issues, consider compressing files or using sharing platforms instead. 

## Conclusion 

In conclusion, productivity is essential in today’s fast-paced work culture, and being able to send large files quickly and easily is a valuable asset. By following our step-by-step guide, you will be able to increase the attachment size limit in Outlook and save yourself and your colleagues time and frustration when dealing with large files. 

So, what are you waiting for? Click now to learn how to increase your attachment size limit and improve your productivity today!

{{< youtube lEOzI24qYO0 >}} 




This article explains how to increase the maximum Outlook attachment size limit. Instructions apply to Outlook 2019, Outlook 2016, Outlook 2013, Outlook 2010, and Outlook for Microsoft 365.

 
### 
What to Know
 
- Open the Windows Registry Editor, find the entry for Outlook, and change the value of MaximumAttachmentSize.Enter the desired size limit in KB (up to 25600).The attachment file size limit in Outlook cannot exceed your mail server's limit.

 
##   How to Increase the Outlook Attachment Size Limit  
 

When sending an email attachment in Outlook, you may receive an error message warning you that the attachment size exceeds the allowable limit. When your mail server allows messages up to 25 MB and your attachment is slightly over the default 20 MB limit, change Outlook's default to match the mail server's default size.

 
- Press Windows+R.
 - In the Run dialog box, type regedit.
 - Select OK.
 - Navigate the registry tree and go to the entry corresponding to your Outlook version:
 - Outlook 2019 and 2016: HKEY_CURRENT_USER\­Software\­Microsoft\­Office\­16.0\­Outlook\­\PreferencesOutlook 2013: HKEY_CURRENT_USER\­Software\­Microsoft\­Office\­15.0\­Outlook\­\PreferencesOutlook 2010: HKEY_CURRENT_USER\­Software\­Microsoft\­Office\­14.0\­Outlook\­\Preferences
 - Double-click the MaximumAttachmentSize value.
 - If you don't see MaximumAttachmentSize, add a registry key and value. Go to Edit, select New > DWORD Value, enter MaximumAttachmentSize, and press Enter.
 - In the Value data text box, enter the desired attachment size limit in KB. For example, to set a size limit of 25 MB, first tick the box next to Decimal and then enter 25600 (because 25600 decimal = 25.6 MB).
 - The default value (when MaximumAttachmentSize is not present) is 20 MB or 20480.For no attachment file size limit, enter 0. Most mail servers have a size limit, so 0 is not recommended; you may get large messages back as undeliverable.The limit corresponds to your mail server's limit. Reduce the Outlook limit by 500 KB to allow wiggle room.
 - You may be confused that 25600 KB equals 25 MB. That's because regedit uses a different measurement system than you may be familiar with. Because of these differences, regedit uses 1024 KB to equal 1 MB. So, the equation to determine the decimal number depends on the MB of storage you want to use. In this case 25 MB is: 25 x 1024 KB = 25600 KB.
 - Select OK.
 - Close the Registry Editor.

 
##   Outlook File Size Limit  
 

By default, Outlook does not send email messages with attachments that exceed 20 MB, but many mail servers allow 25 MB or larger attachments. If your email server allows larger attachments, instruct Outlook to send messages larger than 20 MB. You can also avoid getting undeliverable messages if Outlook's default is larger than what you can send through your mail server.

 
Before making changes to the Windows Registry, back up the Registry so that if you make changes, you can restore your system to its original state.
 

Press Windows+R.

 

In the Run dialog box, type regedit.

 

Select OK.

 

Navigate the registry tree and go to the entry corresponding to your Outlook version:

 
- Outlook 2019 and 2016: HKEY_CURRENT_USER\­Software\­Microsoft\­Office\­16.0\­Outlook\­\PreferencesOutlook 2013: HKEY_CURRENT_USER\­Software\­Microsoft\­Office\­15.0\­Outlook\­\PreferencesOutlook 2010: HKEY_CURRENT_USER\­Software\­Microsoft\­Office\­14.0\­Outlook\­\Preferences

 

Double-click the MaximumAttachmentSize value.

 
If you don't see MaximumAttachmentSize, add a registry key and value. Go to Edit, select New > DWORD Value, enter MaximumAttachmentSize, and press Enter.
 

In the Value data text box, enter the desired attachment size limit in KB. For example, to set a size limit of 25 MB, first tick the box next to Decimal and then enter 25600 (because 25600 decimal = 25.6 MB).

 
- The default value (when MaximumAttachmentSize is not present) is 20 MB or 20480.For no attachment file size limit, enter 0. Most mail servers have a size limit, so 0 is not recommended; you may get large messages back as undeliverable.The limit corresponds to your mail server's limit. Reduce the Outlook limit by 500 KB to allow wiggle room.

 
You may be confused that 25600 KB equals 25 MB. That's because regedit uses a different measurement system than you may be familiar with. Because of these differences, regedit uses 1024 KB to equal 1 MB. So, the equation to determine the decimal number depends on the MB of storage you want to use. In this case 25 MB is: 25 x 1024 KB = 25600 KB.
 

Close the Registry Editor.

 
- How do I send a file attachment with Outlook.com?
 - To send attachments in Outlook.com, compose your email message and select Attach, then choose Browse this computer or Browse cloud locations. If you use Google Drive or Dropbox, select Add an account to connect the service to your Outlook.com account.
 - What is the maximum number of email recipients in Outlook?
 - Outlook has a limit of 500 recipients per message. This limit applies to the totality of To, Cc, and Bcc recipients.
 - What is the maximum number of entries for a distribution group in Outlook?
 - The maximum number of people you can add to an Outlook distribution is 60-120. Because the limit is based on the number of available kilobytes (8KB), it depends on the character length of the email addresses.

 
To send attachments in Outlook.com, compose your email message and select Attach, then choose Browse this computer or Browse cloud locations. If you use Google Drive or Dropbox, select Add an account to connect the service to your Outlook.com account.
 
Outlook has a limit of 500 recipients per message. This limit applies to the totality of To, Cc, and Bcc recipients.
 
The maximum number of people you can add to an Outlook distribution is 60-120. Because the limit is based on the number of available kilobytes (8KB), it depends on the character length of the email addresses.
 

Get the Latest Tech News Delivered Every Day




