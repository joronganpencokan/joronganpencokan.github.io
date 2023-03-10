---
title: "Unlock the Secret to Uninterrupted Linux Usage with This Simple SSH Hack!"
ShowToc: true 
date: "2022-11-27"
author: "Ryan Crook"
---
*****
# Unlock the Secret to Uninterrupted Linux Usage with This Simple SSH Hack!

Are you tired of being booted off your Linux system every time you lose your internet connection or shut down your computer? Do you wish you could continue working uninterrupted even if you can't physically access your computer?

Then it's time to learn about SSH!

SSH, or Secure Shell, is a powerful tool that allows you to connect to your Linux system remotely, even if you're not physically in front of it. With SSH, you can continue working on your Linux system from anywhere in the world, as long as you have an internet connection.

But SSH is more than just a remote connection tool - it can also be used to keep your Linux system running smoothly, even if you lose your internet connection or shut down your computer.

Here's how to unlock the secret to uninterrupted Linux usage with this simple SSH hack:

## Step 1: Install SSH on your Linux system

To use SSH, you first need to install it on your Linux system. Most Linux distributions come with SSH pre-installed, but if yours doesn't, you can easily install it using your package manager.

In Ubuntu, for example, you can install SSH using the following command:

```
sudo apt-get install ssh
```

## Step 2: Enable SSH on your Linux system

Once SSH is installed, you need to enable it on your Linux system. This is done through the SSH daemon, which listens for incoming SSH connections.

In Ubuntu, you can enable the SSH daemon using the following command:

```
sudo systemctl enable ssh
```

This will start the SSH daemon every time you boot your Linux system, ensuring that it's always available for remote connections.

## Step 3: Connect to your Linux system remotely

With SSH installed and enabled on your Linux system, you can now connect to it remotely from another computer.

To do this, you'll need to know your Linux system's IP address. You can find this by running the following command on your Linux system:

```
ifconfig
```

Look for the line that starts with `inet` - this will give you your IP address.

Once you have your IP address, you can connect to your Linux system remotely using an SSH client. There are many SSH clients available, but one of the most popular is PuTTY.

Download and install PuTTY on your remote computer, then open it and enter your Linux system's IP address in the "Host Name" field. Click "Open" to connect.

You'll be prompted to enter your Linux system's username and password. Once you do, you'll be connected to your Linux system remotely!

## Step 4: Keep your Linux system running smoothly with SSH

Now that you're connected to your Linux system remotely, you can use SSH to keep it running smoothly even if you lose your internet connection or shut down your computer.

One way to do this is by using the "screen" command. This command creates a virtual terminal that can continue running even if your internet connection is lost or your computer shuts down.

To use the screen command, simply type the following into your SSH session:

```
screen
```

This will create a new virtual terminal. You can continue working as normal in this terminal, even if your SSH connection is lost or your computer shuts down.

To detach from the screen terminal and leave it running in the background, press `Ctrl + a` and then `d`.

To reattach to the screen terminal later, simply type the following into your SSH session:

```
screen -r
```

This will reattach you to the screen terminal, allowing you to continue working where you left off.

## Conclusion

SSH is a powerful tool that can unlock the secret to uninterrupted Linux usage. By installing and enabling SSH on your Linux system, you can connect to it remotely from anywhere in the world using an SSH client like PuTTY.

With SSH, you can keep your Linux system running smoothly even if you lose your internet connection or shut down your computer. By using the "screen" command, you can create a virtual terminal that can continue running even if your SSH connection is lost or your computer shuts down.

So why wait? Unlock the power of SSH today and enjoy uninterrupted Linux usage!

{{< youtube ACM36qtHIEg >}} 



For those that need to work constantly on SSH, it can be very frustrating when the system cut you off after a period of time. This article shows you the method to keep SSH connection alive until you disconnect it. 
 
Login to your remote system, or open the terminal in your own computer.
 
Open the /etc/ssh/ssh_config file.
 
and add the following line to the end of the file:
 
What this option does is to send a null packet to the server at every 60 seconds (of inactivity) to keep the SSH connection alive. You can experiment with the value, setting it to either higher or lower, depending on your system configuration. A value of 60 is a good starting point to start the experimentation. 
 
## Per user configuration
 
If you don’t have root access to the system or you just want to configure it for your personal account, you can edit the ~/.ssh/config file instead.
 
If the file does not exist, this will create a new file. 
 
Add the following line:
 
Press “Ctrl + o” to save and “Ctrl + x” to exit.
 
Lastly, restart the SSH server.
 
That’s it. 
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox




