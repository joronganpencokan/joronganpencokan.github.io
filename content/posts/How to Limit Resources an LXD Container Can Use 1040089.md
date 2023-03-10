---
title: "Discover the Secret to Maximizing Your LXD Container Efficiency with These Simple Resource Limiting Techniques!"
ShowToc: true 
date: "2023-05-26"
author: "Denise Thurgood"
---
*****
Title: Discover the Secret to Maximizing Your LXD Container Efficiency with These Simple Resource Limiting Techniques!

Introduction:
LXD (Linux container technology) is a rising star when it comes to deploying containers. It is open-source and provides a comprehensive container management experience. When it came to Virtual Machine (VM) deployment, one of the main challenges has been the creation of an isolated environment for processes. Containers, on the other hand, come with their own environment and share the host kernel. This makes them agile, efficient, and easy to manage. In this article, we will walk you through some simple yet effective resource limiting techniques that can help you maximize the efficiency of LXD containers.

Section 1: Understanding Resource Limiting
Resource Limiting is the process of restricting resource usage for containers. This can be in the form of CPU usage, memory usage, disk usage, and network throughput. By setting resource limits, you can prevent containers from overusing resources, which may lead to system instability.

Section 2: Basic Techniques for Resource Limiting
There are several ways to limit resources in LXD containers. Some of the basic techniques are:

CPU Limits: You can set CPU usage limits using the lxc config command. For example, to limit a container to use a maximum of two CPU cores, use the following command: `lxc config set <container-name> limits.cpu 2`

Memory Limits: To limit the memory usage of a container, use the following command: `lxc config set <container-name> limits.memory 2GB`

Disk I/O Limits: You can limit I/O throughput for containers by setting the read and write iops using the following command: `lxc config set <container-name> limits.disk.priority.read_iops 10`

Network Limits: You can also limit network throughput for containers using the following command: `lxc config set <container-name> limits.network.egress.rate 10MB`

Section 3: Advanced Techniques for Resource Limiting
Apart from basic resource limiting techniques, there are advanced techniques that can help you maximize the efficiency of LXD containers. Some of these techniques are:

Using Cgroups: Control Groups (Cgroups) is a feature in Linux that allows you to limit resources for processes. By enabling Cgroups for LXD containers, you can set limits for CPU, memory, and network usage. To enable Cgroups, use the following command: `lxc config set <container-name> raw.lxc cgroup.enabled true`

Using LXD Compression: LXD Compression is a feature that compresses the container’s file system, reducing its size and making it faster to backup, copy and move between LXD hosts. To enable LXD Compression, use the following command: `lxc config set <container-name> raw.lxc lxd.compress true`

Using Storage Quotas: You can also set storage quotas for LXD containers to limit the amount of storage space they can use. To set storage quotas, use the following command: `lxc storage volume set <storage-pool>/<container-name> quota 2GB`

Conclusion:
Resource Limiting is an essential aspect of container management, and LXD offers several ways to limit resources for containers. By using these simple yet effective techniques, you can maximize the efficiency of LXD containers, improve system stability, and ensure smooth operation.

{{< youtube KxkUWD9F-Ek >}} 



In a previous article, you can explore what LXD is and how to get started with it, in case you’re unfamiliar with the platform.
 
In most cases, you will use multiple containers on the same system to split a larger whole into smaller components. It makes sense to limit the amount of resources each component can use. But why? Obviously, the number of reasons is as unlimited as the scenarios for which you can use containers.
 
## When Limits on LXD Containers Can Be Useful
 
- Providing a service and giving each customer an LXD instance. For example, this might be a large server, and you host each customer website into a separate container. If a website gets a sudden burst of traffic, this might slow down the other instances. With limits, only one container will slow down, and the rest will operate normally.In a similar scenario, you can easily sell different service plans. One customer can pay for X amount of resources, and the other can pay for Y amount. And you can easily adjust this with a few simple commands.You can protect yourself against simpler forms of Denial of Service attacks. When one container gets bombarded, it will reach its resource usage limits. The other containers won’t be affected.You have two containers that will each use 100% of the CPU time available. However, you want one to finish the job faster than the other. For example, one might render a video for a project that you need tomorrow. You can assign 90% of the CPU time to the first and 10% to the second.

 
Of course, you may have your own reasons. And if you’re only using one container on the whole system, you might not even need this. But if you’re using multiple containers, you almost always need to set some kinds of limits. Because, an attack, a bug, or some other form of misbehavior in one LXD instance can affect the whole system and slow it down. The more containers you have, the more the likelihood of such a scenario increases.
 
## How to Set Resource Limits On LXD Containers
 
Resource control relating to disk operations will need ZFS to be installed. If you followed the tutorial here, it is already installed. Otherwise, install ZFS utilities as instructed in the tutorial and then rerun the command below. Pick ZFS when asked which storage backend to use.
 
### Limit Memory Usage
 
In the commands below, replace “container_name” with the actual name of your container. Setting a memory limit is as simple as entering:
 
Type “GB” instead of “MB” if you want to use gigabytes instead of megabytes.
 
### Limit CPU Usage
 
When you want to limit how many CPU cores a container can use, type:
 
To “pin” to specific CPU cores, use:
 
This would make the container only use the first CPU. To use the second, you would type 1-1. To use all CPU cores from first to third, you would type 0-3.
 
Another type of limit is how much CPU time a container can use.
 
This would only let the container use ten miliseconds of CPU time out of every 100 miliseconds, so around 10% of one CPU core.
 
### Limit Disk Usage
 
To limit disk-related resources, you must first add a root disk device to your container. It already exists by default, inherited from the default LXD profile. But you can’t change its settings on a per container basis until you do this.
 
If you named your pool differently, replace “default” with the name of your storage pool. If you forgot its name, you can display it with:
 
To limit the disk space an LXD instance can use:
 
Unfortunately, I/O limits (read/write “speeds” and IOPS) don’t work at the moment.
 
### Limit Network Usage
 
As with disks, you first have to add a virtual ethernet device that you can configure. Find the name of your network bridge that connects your LXD instances to the outside world.
 
Replace “lxdbr0” if necessary (if the bridge is named differently in your case). If you didn’t choose the network type as bridged (default answer), in the “lxd init” configuration steps you might have to adapt the command below to reflect your choice. For example, you might have to replace “nictype,” too, with whatever you used for your LXD network.
 
Finally, set limits on network ingress (download) and/or egress (upload).
 
1Mbit is one megabit (not megabyte). One byte contains 8 bits, which means this will limit downloads to around 1/8=0.125Mbits per second, roughly 120 kilobytes. So, if you want it to download with 1MB/s (megabyte), multiply by 8, and set the ingress limit to 8Mbit.
 
For egress, use:
 
## Conclusion
 
This covers the most commonly used properties relating to resource limits. But there are a lot more variables you can set with lxc config device set and lxc config set. You can read more about these adjustable container properties on LXD’s GitHub page.
 
Fell in love with computers when he was four years old. 27 years later, the passion is still burning, fueling constant learning. Spends most of his time in terminal windows and SSH sessions, managing Linux desktops and servers.
 
Our latest tutorials delivered straight to your inbox




