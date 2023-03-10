---
title: "Revolutionize Your Linux Experience: Unleash The Power Of Arch Linux With Our Ultimate Guide To Installing Deb Packages!"
ShowToc: true 
date: "2023-06-20"
author: "Will Witten"
---
*****
# Revolutionize Your Linux Experience: Unleash The Power Of Arch Linux With Our Ultimate Guide To Installing Deb Packages!

If you're a Linux user, chances are that you have heard of Arch Linux. It's a popular distribution among Linux enthusiasts due to its customizable nature and the fact that it offers a rolling release model. However, one of the biggest complaints about Arch Linux is that it does not support Debian packages (deb), which are commonly used in popular Linux distributions like Ubuntu, Mint, and Debian itself.

Fortunately, there is a solution to this problem. By following our ultimate guide to installing deb packages on Arch Linux, you can gain access to a wider range of software packages and have a more user-friendly experience using Arch Linux.

Before we dive into the guide, it's important to note that this method is not officially supported by the Arch Linux community. While there are many users who have successfully installed deb packages on their Arch Linux systems, there is a small risk that something could go wrong during the installation process. With that said, if you follow our guide carefully, the risk should be minimal.

## Step 1: Install the Required Dependencies

The first step to installing deb packages on Arch Linux is to install the required dependencies. Open your terminal and enter the following command:

```
sudo pacman -S dpkg binutils fakeroot
```

This will install the Debian package manager (dpkg), the GNU binutils package, and the fakeroot utility. These tools are necessary to extract deb packages and create a temporary Debian environment to install them.

## Step 2: Download and Extract the Deb Package

The next step is to download the deb package you want to install. You can download it from the software's official website or a trusted third-party repository. Once you've downloaded the package, navigate to the directory where it is saved and extract it using the dpkg-deb command:

```
sudo dpkg-deb -x package_name.deb directory_name
```

Replace "package_name.deb" with the name of the deb package you downloaded and "directory_name" with the name of the directory where you want to extract it.

## Step 3: Build and Install the Deb Package

Once you have extracted the deb package, you can build it and install it using the fakeroot utility. Navigate to the directory where you extracted the package and enter the following commands:

```
sudo fakeroot sh -c 'dpkg-deb -e control.deb; dpkg-deb -x package.deb directory/; dpkg-deb -b directory new-package-name.deb'
sudo pacman -U new-package-name.deb
```

Replace "control.deb" with the name of the control file that was generated when you extracted the deb package, "package.deb" with the name of the package file that was extracted, "directory/" with the name of the directory where the package was extracted, and "new-package-name.deb" with the name you want to give to the new package.

The first command creates a temporary Debian environment, extracts the package contents, and generates a new control file. The second command installs the new package on your Arch Linux system using the pacman package manager.

## Conclusion

By following our ultimate guide to installing deb packages on Arch Linux, you can enjoy a wider range of software packages and an improved user experience. While this method is not officially supported, it has been successfully used by many Arch Linux users. However, always remember to exercise caution and ensure that the packages you download are from trusted sources. With the power of Arch Linux and the versatility of deb packages, you can take your Linux experience to the next level.

{{< youtube DPLnBPM4DhI >}} 



If you’ve used Linux for any amount of time, you’ve noticed that one of the most common methods to install third-party applications is via a .Deb package. Often times this is the only way to get this software, as the developers can’t be bothered to go through the process of packaging in the dozens of different formats the Linux platform offers.
 
Many non-Debian-based Linux distributions have their own ways of getting around this issue. However, out of all Linux distributions, Arch Linux has the most interesting ways of getting a Debian package working. In this article we outline three ways to accomplish this and discuss which one is best.
 
Note: the steps below will work for any Arch-based distro.
 
## Installing via the AUR
 
The AUR is the first place to check when looking for software that isn’t officially supported in Arch Linux. Always check here first. It’s a service that allows anyone to upload a PKGBUILD script, designed to automatically take software from various places, download some or all of the needed dependencies to run them and compile a native Arch Linux package.
 
When using the AUR, there are two ways to go about it:
 
### 1. Use an AUR Helper
 
If you want to get stuff done quickly without having to jump through hoops, use an AUR helper like yay or yaourt. This won’t allow you to install a .deb file, but you may be able to find the package in arch format, created by arch users.
 
For more information about AUR hepers and how to install them, refer to our list of five awesome AUR helpers. Once you have one, just search the AUR, install and go.
 
Chances are if you’re using Manjaro, Endeavour, Garuda or any of the other Arch-based distros, you’ll have an AUR helper installed. Have a look at your distro’s documentation to check out what is included. Both Garuda and Endeavour use yay.
 
If you’d rather have a graphical environment, you can always install the pamac-aur package with your AUR helper – if it’s not installed already. Note that you’ll have to enable AUR support after installation under “Preferences -> Third Party.”
 
### 2. Manual Installing AUR Packages
 
Another way of getting unofficial packages is by going to the AUR website, using the search bar, and downloading the “snapshot.” This is a less automated process, but it’s worth it if you want more granular control over how packages are made or installed. Instead of instantly installing the package, it’ll spit out a native package you can modify for your own purposes.
 
This means that if you have a custom personal repository set up, you can easily place these newly-built packages right in the repo for easy installation.
 
Note: if you just plan to use Arch’s base repositories and the AUR, installing packages with an AUR helper is a much better option than manual builds.
 
Most (if not all) programs that only come in DEB format will be found in the AUR. Here’s how to compile one as an Arch package from scratch.
 
- Make sure you have git and the base dev packages for Arch installed by typing

 
in your terminal.
 
- Pay attention to the “Git Clone URL” on the AUR page of the package you want to download and install and copy it. Use that URL in the terminal opened in the home directory like so:

 
This will download the package’s git repository with a PKGBUILD configuration file for Arch’s powerful makepkg tool.
 
- Type

 
to navigate to the package’s build directory you just downloaded.
 
to create the package and install it automatically. 
 
If you’re curious, the -s (--syncdeps) flag automatically grabs all the dependencies related to the available package in the official Arch Linux repositories, while the -i (--install) flag tells your system to not just compile the package but also integrate it into your system (e.g., create menu items, perform necessary integration into kernel arguments if there are any, etc.).
 
## Install via Debtap
 
If, for some reason, a Deb you need isn’t in the AUR, install Debtap. It’s a program that dismantles a Debian package and makes it into an Arch package that your package manager can “understand.”
 
Warning: Use this method at your own discretion. The .deb package you install may break if the upstream package maintainers for the packages it depends on get updates that remove features or functionality. It doesn’t happen all the time, but you should be aware that this method may not always work fantastically.
 
- Start by installing Debtap via the AUR by following the instructions in the previous section.Once installed, run sudo debtap -u once to update debtap’s own repositories. Otherwise, the application will not work.Download the .deb file you wish to convert, cd into the directory you downloaded it into, and use the following command:

 
- At any point that Debtap asks you to input data, you can simply ignore this and press Enter on your keyboard.When finished, Debtap will have created a “pkg.*.zst” file that your package manager can interpret and install using offline installation procedures.cd into the directory you just converted the .deb package into and type:

 
## Installing Manually
 
Warning: This method is highly unsafe and should only be used when there is no other option and you already have an advanced understanding of how certain packages work and certain behaviors that Arch expects. For example, some applications (like Plymouth, Virtualbox, etc.) may require hooks into the kernel that can only be done by editing configuration files and re-building the kernel with those hooks. Even more, using this method does not also install the dependencies of your package.
 
Though not the most elegant solution, when there’s no way to convert a .deb file with Debtap or compile with an AUR pkgbuild, the best method is to extract the Debian package itself and put the files where they should go.
 
Though this may involve a lot more tedium than previous methods, it’s more platform-independent, meaning you can use this method in many other distributions like Void Linux, Fedora, and openSUSE. I have not tested this in Gentoo and Slackware, so your mileage may vary with them due to how both distros like to handle installing packages.
 
Debian packages are archives with binaries inside, so no compiling is necessary. To install the files in any Deb package to Arch, first extract it to a folder. Keep in mind that you’ll also need to extract the archive known as “data” inside that folder as well.
 
For example, to install Google Chrome, you’d first cd into the extracted Deb folder with the extracted contents of “data.tar.xz” inside it.
 
Then, run the ls command to reveal all of the folders that reside in the data archive inside the Deb package. Keep in mind the names of these folders. cd into each directory and move the contents of these directories to where they belong on the system.
 
For example:
 
## Frequently Asked Questions
 
### 1. Why Is Debtap Taking So Long?
 
Debtap grabs the metadata available in the .deb file to construct the most faithful Arch package possible to minimize issues and provide relevant information on which dependencies pacman should install in addition to the package itself. This involves a significant amount of tedium beyond simply decompressing a tarball.
 
In addition to this, the script Debtap converts files with uses only one CPU core, making single-core performance the determining factor that affects how long your system will take to complete the operation. Expect large packages to take up to a few minutes.
 
### 2. Can I Use a Graphical Installer After Running Debtap?
 
Yes! If you have any version of pamac installed, you can run the tar-zst file Debtap generates through your file manager. By choosing pamac as the program to run the file, you can just double-click it just like you would any .deb package in Debian to install it and all of its dependencies automatically.
 
### 3. How does Debtap Compare with the AUR?
 
You should see Debtap as a last-ditch “dirty” method for installing something you really need and somehow can’t find in the AUR. If you can find something in the AUR, it will always be a better option to install that package than using a .deb file.
 
## Wrapping Up
 
One of the best things about Arch Linux is how many ways users can install packages – from the AUR, to custom repositories, to decompiling other distributions’ packages so they’ll run. Though this information isn’t new, it’s certainly a good resource for those new to Arch and looking for ways to install their favorite programs.
 
Read on to learn how to use AUR in Arch Linux.
 
Image credit: St. Louis, Missouri, USA city skyline and park in the morning by 123RF 
 
Miguel has been a business growth and technology expert for more than a decade and has written software for even longer. From his little castle in Romania, he presents cold and analytical perspectives to things that affect the tech world.
 
Our latest tutorials delivered straight to your inbox




