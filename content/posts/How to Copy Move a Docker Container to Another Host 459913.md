---
title: "Unlock The Secret to Seamlessly Copying Docker Containers Across Different Hosts - Learn How Now!"
ShowToc: true 
date: "2022-12-15"
author: "Inez Lynch"
---
*****
# Unlock The Secret to Seamlessly Copying Docker Containers Across Different Hosts - Learn How Now!

Are you struggling with how to move Docker containers from one host to another without running into numerous challenges? Do you find it challenging to replicate container configurations across different deployment environments? If yes, this article is here to help you.

Docker containers are a popular means of deploying applications and managing infrastructure. However, copying Docker containers across different hosts can be a daunting task, especially for beginners. The process involves copying the container image, transferring the container data, and replicating the container configuration – a task that can be quite challenging, especially when dealing with complex container configurations.

But do not worry because there is a little-known secret to seamlessly copying Docker containers across different hosts, and in this article, we will reveal it to you. So, let’s get started.

## The Secret: Export and Import

The secret to seamlessly copying Docker containers across different hosts lies in using the Docker `export` and `import` commands. These commands allow you to export a container and import it into another host, thereby replicating the container configuration and data.

The `export` command creates a tar archive of the container’s root file system, which you can then copy to another host using a file transfer protocol such as SCP. The `import` command then uses the exported tar archive to create a new container on the target host.

The process is simple, and it involves the following steps:

1. Export the Docker container:

To export a container, use the `docker export` command followed by the name or ID of the container and the output file name. For example:

``` 
docker export container-name > container.tar
```

This command will create a tar archive of the container’s root file system and save it to the file `container.tar`.

2. Transfer the exported tar archive to the target host:

You can use any file transfer protocol to transfer the exported tar archive to the target host. For example, you can use SCP to copy the file to the target host. For example:

``` 
scp container.tar user@target-host:/path/to/container.tar
```

This command will transfer the `container.tar` file to the `target-host`.

3. Import the exported tar archive to create a new container:

To create a new container from the exported tar archive, use the `docker import` command followed by the path to the exported tar archive and the name of the new container. For example:

``` 
docker import /path/to/container.tar new-container-name
```

This command will create a new container on the target host using the exported tar archive.

And that’s it! With these simple steps, you can seamlessly copy Docker containers across different hosts.

## Conclusion

Copying Docker containers across different hosts can be a daunting task, but with the Docker `export` and `import` commands, it becomes a simple and seamless process. These commands allow you to export a container, transfer it to another host, and import it to create a new container, replicating the container configuration and data.

So, if you are struggling with copying Docker containers across different hosts, give this method a try, and you will be surprised at how easy and seamless the process can be.

{{< youtube eGz9DS-aIeY >}} 



Since Docker containers are little boxes of software, so to speak, you can copy and move them around from computer to computer. However, this is not often discussed, probably because larger organizations set up their own repositories, where they can customize their own images and distribute across their servers as they see fit. But you shouldn’t have to go through the trouble of setting up your own line of distribution if you occasionally need to move one or more containers around.
 
It may be that you worked on a Docker instance on your local computer and decided to move it to a more powerful server. Or maybe you just want to deploy your customized container on multiple computers, “copy and paste” it around. Other times you may be dissatisfied with a cloud-computing provider and want to switch to a different one. Whatever the situation, there’s a rather simple procedure to do this which will be detail below.
 
## Save Container Image from Source Host
 
It’s not required to stop the container first, but it’s highly recommended that you do so. You will take a snapshot of the data in your Docker instance. If it’s running while you do this, there’s a small chance some files might end up being incomplete in your snapshot. Imagine someone uploading a 500MB file. When 250MB has been uploaded, you issue the docker commit command. The upload then continues, but when you restore this Docker image on another host, only 250MB out of the 500MB might be available.
 
So, if you can, first stop the instance.
 
A Docker container is built out of a generic, initial image. Over time, you add your own changes to this base image. Processes running inside the container might also save their own data or make other changes. To preserve all of this, you can commit this new state to a new image.
 
Note that if the instance is currently running, this action will pause it while its contents are saved. If you added a lot of data to your container, this operation will take a longer time to complete. If this is a problem, you can avoid this pause by entering docker commit -p=false NAME_OF_INSTANCE mycontainerimage instead of the next command. However, don’t do this unless absolutely necessary. The odds of creating an image with inconsistent/incomplete data increase in this case.
 
In this tutorial, a generic name has been chosen for the resulting image, mycontainerimage. You can change this name if you want to. If you do so, remember to replace it in all subsequent commands where you encounter it.
 
Now, save this image to a file and compress it.
 
Next, use your preferred file transfer method and copy mycontainerimage.tar.gz to the host where you want to migrate your container.
 
## Load Container Image on Destination Host
 
After you log in to the host where you transferred the image, import it to Docker.
 
Since you never initialized this container here, you cannot start it with docker start yet. Instead, issue the same command you used in the past, when you first ran this Docker instance. The only difference now is that you will use “mycontainerimage” at the end instead of whatever image you used in the past.
 
The next command is just an example; don’t copy and paste this unless it applies to you. (No special parameters were required when you ran the image for the first time)
 
As contrast, the following is an example of a command where parameter --publish was required to forward port 80 on the host machine to port 80 on the container:
 
Afterwards, you can stop and start this container normally, with docker stop and docker start commands.
 
## Transfer Image without Creating a File
 
Sometimes you may want to skip creating a mycontainerimage.tar.gz file. Maybe you don’t have enough disk space since the container has a lot of data in it. You can save, compress, transfer, uncompress and load the image on the destination host in one command. After running the docker commit command discussed in the first section, you can use this:
 
It should work from Windows, too, since it now has a built-in SSH client (PuTTY not necessary anymore).
 
Afterwards, continue with the docker run command that applies to your situation.
 
## Conclusion
 
docker save and docker load are great as an ad hoc solution for moving containers around occasionally. But remember, if you do this often, you might want to set up your own private repository instead.
 
Image Credit: Air Force Medical Service
 
Fell in love with computers when he was four years old. 27 years later, the passion is still burning, fueling constant learning. Spends most of his time in terminal windows and SSH sessions, managing Linux desktops and servers.
 
Our latest tutorials delivered straight to your inbox




