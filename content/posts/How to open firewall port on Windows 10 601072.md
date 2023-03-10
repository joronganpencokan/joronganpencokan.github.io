---
title: "Unlock the Hidden Power of Windows 10: Learn How to Open Firewall Ports in a Single Click!"
ShowToc: true 
date: "2023-03-24"
author: "Sandra Harmon"
---
*****
# Unlock the Hidden Power of Windows 10: Learn How to Open Firewall Ports in a Single Click!

If you are a Windows 10 user, you know how important it is to keep your computer secure. And one of the most critical parts of keeping your computer secure is ensuring that only authorized traffic is allowed in and out of your network. That is where the Windows 10 Firewall comes in. The Firewall is a critical part of your computer’s security that monitors and manages incoming and outgoing traffic.

Today, we will be discussing how you can open firewall ports in Windows 10, in a single click, to unlock the hidden power of your Windows 10 operating system.

## What are Firewall Ports?

Before we dive into how to open firewall ports in Windows 10, let's quickly discuss what Firewall Ports are. Firewall Ports are numbers that represent different network services that run on your computer. Each port is associated with a particular protocol, and different protocols use different ports.

When a network service requests access to your computer, the Firewall checks the port that the service is using to see if it is allowed. If the port is not allowed, the request is blocked, and the service is denied access.

## How to Open Firewall Ports in Windows 10

Now that we understand what Firewall Ports are let's take a look at how to open them in Windows 10. 

Traditionally, users had to go through a series of steps to open Firewall Ports. However, Microsoft added a feature in Windows 10 that enables users to open Firewall Ports with a single click. 

Here is how to do it: 

1. Open the “Windows Security” app. You can do this by searching for “Windows Security” in the Windows search bar, or by clicking on the Shield icon at the bottom right of your screen in the taskbar.

2. Click on the “Firewall & Network Protection” tab.

3. Click on the “Advanced settings” option.

4. Click on the “Inbound Rules” option in the left-hand menu.

5. Click on the “New Rule” option at the top of the right-hand pane.

6. In the “New Inbound Rule Wizard,” select "Port" and click "Next."

7. Select the "TCP" or "UDP" option, depending on your needs, and enter the port number that you want to open. Click "Next."

8. Select "Allow the connection" and click "Next."

9. Check all where the rule applies, click "Next."

10. Name the rule and add a description if necessary. Click "Finish."

That's it! You have opened a Firewall Port in Windows 10 with a single click.

## Conclusion

Opening Firewall Ports in Windows 10 is not only essential for your computer's security but also for allowing authorized network traffic through. With the simple steps outlined above, you can now open Firewall Ports in a single click, unlocking the hidden power of your Windows 10 operating system.

Stay secure!

{{< youtube xMGPyZtdP00 >}} 



- To open a Windows firewall port, open the “Windows Defender Firewall with Advanced Security” console.
 - Then click on “Inbound Rules” or “Outbound Rules,” click on “New Rule,” and select the “Port” option.
 - Continue selecting the protocol, and the port number to open on Windows 10, allow the connection, choose the network profile to apply the rules, and save the changes.

 
On Windows 10, the built-in firewall (also known as the “Microsoft Defender Firewall” or “Windows Firewall”) is a powerful feature that protects your computer and data from threats from outside trying to get in and from those inside trying to get out.
 
A firewall works as a gatekeeper and blocks all unnecessary network ports. Every time an app or service tries to communicate outside your device, it checks if there’s a specific rule in the database to allow or deny network access. You’ll see a prompt to identify and grant or deny permission if it can’t find a rule.
 
Sometimes well-known applications (for example, SQL Server and QuickBooks) will not work as expected because they’re getting blocked by the Microsoft Defender Firewall. When this happens, you’ll need to manually create a rule to allow them to access the network.
 
This guide will teach you the steps to open a port to allow an app to communicate outside the network using the built-in firewall on Windows 10.
 
- Open firewall port on Windows 10
 - Close firewall port on Windows 10

 
## Open firewall port on Windows 10
 
To open one or more ports in the Windows firewall, use these steps:
 
- Open Windows Security.
 - Click on Firewall & network protection.
 - Click the Advanced settings option.
 - Select Inbound Rules from the left navigation pane.
 - Under the “Actions” section, click the New Rule option in the right pane.
 - Select the Port option.
 - Click the Next button.
 - Select the appropriate protocol (TCP or UDP) depending on the application. (Usually, the option is TCP.)
 - Type the port number in the “Specific local ports” setting.
 - Quick note: If the app requires multiple ports open, you can type as many as you need as long as you separate each one with a comma (4500,4600,5000). If you need to specify a port range, you can use a hyphen (-). For example, 3000-3100.
 - Click the Next button.
 - Select the Allow the connection option. (Using the same step, note that you can block the connection.)
 - Click the Next button.
 - Select the network type to apply the rule. (Usually, you want to leave this option with the default selections.)
 - Click the Next button.
 - Type a descriptive name for the rule—for example, My Inbound Rule for QuickBooks.
 - Click the Finish button.

 
After you complete the steps, inbound connections will be allowed for the app through the port you open in the firewall.
 
Open Windows Security.
 
Click on Firewall & network protection.
 
Click the Advanced settings option.
 

 
Select Inbound Rules from the left navigation pane.
 
Under the “Actions” section, click the New Rule option in the right pane.
 
Select the Port option.
 
Click the Next button.
 
Select the appropriate protocol (TCP or UDP) depending on the application. (Usually, the option is TCP.)
 
Type the port number in the “Specific local ports” setting.
 
Select the Allow the connection option. (Using the same step, note that you can block the connection.)
 
Select the network type to apply the rule. (Usually, you want to leave this option with the default selections.)
 
Type a descriptive name for the rule—for example, My Inbound Rule for QuickBooks.
 
Click the Finish button.
 
### Open outgoing port in Microsoft Defender Firewall
 
If the app needs a specific outbound port, you can use the same instructions, but instead of selecting Inbound Rules on step 4, you would choose the Outbound Rules options.
 
To open an outbound firewall port on Windows 10, use these steps:
 
- Open Windows Security.
 - Click on Firewall & network protection.
 - Click the Advanced settings option.
 - Click on Outbound Rules in the left navigation pane.
 - Under the “Actions” section, click the New Rule option in the right pane.
 - Select the Port option.
 - Click the Next button.
 - Select the appropriate protocol (TCP or UDP) depending on the application.
 - Type the port number in the “Specific local ports” setting.
 - Click the Next button.
 - Select the “Allow the connection” option.
 - Click the Next button.
 - Select the network type to apply the new rule.
 - Click the Next button.
 - Type a descriptive name for the rule.
 - Click the Finish button.

 
Once you complete the steps, outbound connections will be allowed for your application through the port you open in the Windows firewall.
 
Click on Outbound Rules in the left navigation pane.
 
Select the appropriate protocol (TCP or UDP) depending on the application.
 
Select the “Allow the connection” option.
 
Select the network type to apply the new rule.
 
Type a descriptive name for the rule.
 
## Close firewall port on Windows 10
 
To close the port in the Microsoft Defender Firewall, use these steps:
 
- Open Windows Security.
 - Click on Firewall & network protection.
 - Click the Advanced settings option.
 - Click on Inbound Rules or Outbound Rules from the left navigation pane, depending on where you open the firewall port.
 - Select the rule you want.
 - Under the “Actions” section, click the Disable Rule to close the port while keeping the rule. Or click the Delete Rule option to close the port and remove the rule from the firewall.

 
After you complete the steps, the app or service will no longer have access to the network or internet because the Windows firewall will block it.
 
Click on Inbound Rules or Outbound Rules from the left navigation pane, depending on where you open the firewall port.
 
Select the rule you want.
 
Under the “Actions” section, click the Disable Rule to close the port while keeping the rule. Or click the Delete Rule option to close the port and remove the rule from the firewall.




