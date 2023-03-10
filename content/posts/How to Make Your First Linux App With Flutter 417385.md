---
title: "Revolutionize Your App Game: Create Your First Linux App with Flutter - Here's How!"
ShowToc: true 
date: "2023-04-10"
author: "Kellee Critchlow"
---
*****
# Revolutionize Your App Game: Create Your First Linux App with Flutter - Here's How!

In recent years, Linux has gained immense popularity as a free, open-source operating system with a wide range of applications. It has become an excellent platform for developers to create innovative software solutions. If you're thinking of building a Linux application that can cater to countless Linux users, then you're in the right place.

Flutter is one of the latest app development kits that have taken the tech world by storm. This framework allows developers to create fast, scalable, and high-performing apps for various platforms, including Linux. In this article, we'll take a look at how you can create your first Linux app with Flutter.

## What is Flutter?

Flutter is a software development kit(DSK) developed by Google to make it easier for developers to build cross-platform apps for iOS, Android, and now Linux. It uses the Dart programming language, which is an object-oriented language that is easy to learn and use.

Flutter works with a reactive programming model, which means that the app's UI automatically updates itself whenever there is a change in the app's state. It uses a declarative API, which makes it easier to create complex animations and interactions with just a few lines of code.

## Why Choose Flutter for Linux App Development?

Flutter is a great choice for Linux app development for several reasons. First, it is open-source and free, which means that you don't have to worry about licensing fees. Second, it is easy to use, and you don't need to have extensive knowledge of Linux to get started.

Third, Flutter is highly customizable, which means that you can create an app that meets your specific needs. Finally, Flutter is fast and efficient, which is essential when developing apps for Linux users who expect their apps to be responsive and user-friendly.

## Getting Started with Flutter for Linux App Development

To get started with Flutter for Linux app development, you'll need to have a few things in place first. Here's what you need:

- A Linux machine with a recent distribution (such as Ubuntu)
- Flutter SDK installed on your machine
- An IDE (Integrated Development Environment) such as Visual Studio Code
- Basic knowledge of Dart programming language

Once you have all of these in place, you can start creating your first Linux app using Flutter.

## Creating Your First Linux App with Flutter

To create your Linux app with Flutter, follow these simple steps:

1. Open Visual Studio Code and create a new Flutter project.

2. Set the project's SDK path to your Flutter SDK.

3. Add the Linux desktop plugin to your project by running the following command:

```sh
$ flutter config --enable-linux-desktop
```

4. Add the linux-cmake plugin to your project by running the following command:

```sh
$ sudo apt-get install cmake
```

5. In the "pubspec.yaml" file, add the following dependencies:

```yaml
dependencies:
  flutter:
    sdk: flutter
  flutter_linux: ^0.1.3
```

6. In the project directory, run the following command:

```sh
$ flutter packages pub get
```

7. Create a new folder in your project directory called "linux" and inside it, create a file called "main.cc".

8. In the "main.cc" file, add the following code:

```c++
#include <flutter_linux/fl_emulator.h>

int main(int argc, char **argv) {
  fl_emulator_main(argc, argv);
  return 0;
}
```

9. After creating your UI, you can build your Linux app by running the following command:

```sh
$ flutter build linux
```

Once the build process is complete, you'll have a Linux-compatible executable file in the "build/linux/release/bundle" directory.

## Conclusion

Flutter is an excellent tool for Linux app development. With its simplicity and flexibility, you can quickly create high-quality applications for Linux users. By following the steps outlined above, you can create your very first Linux app with Flutter in no time. So, are you ready to revolutionize your app game? Try creating your first Linux app with Flutter today!

{{< youtube GLSG_Wh_YWc >}} 



Many popular apps, such as Adobe Photoshop, Microsoft Office, and WhatsApp, don’t have Linux desktop counterparts. However, thanks to cross-platform application development platforms like Electron, Flutter and Tauri, the number of Linux apps is on the rise.
 
If you’re interested in trying your hand at development, this tutorial shows you how to make a very simple app using Flutter and could prove helpful for those who want to figure out how to create apps for Linux and get some programming experience. 
 
## Why Linux Needs More Apps
 
Linux has a smaller desktop user base compared to Windows and Mac, which is one of the reasons application developers are reluctant to publish their apps on Linux. Unfortunately, the scarcity of popular apps compatible with Linux affects adoption by the general population, thus creating a vicious cycle. It doesn’t help that Linux is often considered an alternative for more tech-savvy individuals. 
 
To change this narrative, the Linux community needs to focus on porting more utility-focused apps to its ecosystem. With and increasing user-base, major developers will finally be encouraged to launch their applications on Linux. If you’d like to be part of this effort, Flutter is a great way to start your Linux app development journey.
 
## What Is Flutter?
 
Flutter is a cross-platform application development framework by Google that uses Dart, an object-oriented programming language. Flutter’s biggest advantage is that it allows developers to build natively compiled applications for mobile, Web, and desktop from a single codebase.
 
Currently, Flutter supports all desktop platforms, including Windows, Mac, and Linux, as well as Android and iOS on mobile. Flutter doesn’t use platform-specific UI elements and instead implements a blank canvas with added widgets. Therefore, Flutter is called a declarative framework.
 
## Why Choose Flutter for Your Linux App Development?
 
Flutter is very fast compared to alternatives like Electron. The latter uses web technologies to build desktop apps and bundles a Chromium engine to get consistent performance on all desktop platforms. Therefore, apps developed on the platform are very heavy and consume more RAM.
 
Flutter takes a different approach, compiling the Dart source code into platform-specific C/C++ bundles. The resulting apps are considerably lighter than Electron apps, which means they’re also more performant and consume fewer resources.
 
Flutter comes with support for the latest Gnome Libadwaita style widgets and allows developers to customize their applications using Ubuntu’s Yaru theme. Moreover, Canonical has published various easy-to-use packages to help users build Linux apps efficiently and without digging too much into the Linux system APIs.
 
## 1. Installing Flutter on Your Machine
 
Described below are three ways to install Flutter on your Linux desktop.
 
### Install Flutter Using Snap
 
Before installing Flutter via Snap, you should have Snap installed on your computer. Snap is part of Ubuntu distributions, but you can easily install it in other desktop environments too.
 
If you are using a Debian-based distribution, first install “snapd” using your package manager.
 
Restart your device to ensure all Snaps paths are correctly set up. To get the latest version of “snapd,” install the core Snap package.
 
For Fedora or Red Hat-based Linux distributions, you can use the DNF package manager to install “snapd.”
 
Flutter is a classic Snap, so it behaves as a traditionally installed system. It has full access to your system as opposed to normal Snaps, which are confined to a sandbox environment. To enable classic Snap in Fedora, run the following command.
 
Once Snap is onboard your computer, install Flutter with Snap.
 
Run the flutter doctor -v command to see if everything is set up on your device. If that’s not the case, the Flutter CLI (Command Line Interface) gives you the proper instructions to set up all of the required components to develop Linux apps on your device.
 
### Install Flutter Manually
 
If you don’t want to use Snap, you can download the latest Flutter stable release from the official website and install it manually from there. Alternatively, run the wget command to download Flutter directly without leaving your Terminal.
 
You’ll need to substitute version 3.3.2 with the latest Flutter stable version using this command:
 
Then extract the files into the current directory.
 
Copy the extracted Flutter directory to your Home folder and set the Flutter binary path in your bash environment.
 
Run the flutter doctor -v command to see whether Flutter is successfully installed. If you want to set the Flutter environment variables permanently and make Flutter commands accessible in your environment, set the Flutter environment variable in your “.rc” file.
 
If you’re using the bash shell, open your “.bashrc” file and paste the following line of code at the end of it. 
 
Note: change the [PATH_OF_FLUTTER_DIRECTORY] to your own Flutter directory path.
 
Hit save and source your “.bashrc” file or use a new Terminal window to refresh your environment variables present in the “.bashrc” file.
 
Finally, run the flutter doctor -v command again to see whether all the Flutter components are properly installed on your device. Alternatively, follow the Terminal outputs to install all required Flutter libraries.
 
### Install Using Git
 
Installing Flutter using Git is similar to the above processes. The primary difference is, instead of downloading a particular Flutter version, you can switch the Flutter version by simply adding a Terminal argument.
 
It’s possible to install Git using your package manager.
 
Clone the GitHub repository to the current working directory. You should use your home directory rather than a random directory.
 
The above command cloned the master branch of the GitHub repository. If you want to switch it to the stable branch, add a -b flag to the git clone command.
 
Add the Flutter path to your “.bashrc” file to finish the Flutter installation.
 
## 2. Generating a Flutter Project
 
If you just started working on the project and haven’t written much code yet, creating a project with a new package name (unique identifier) is the cleanest solution. Each Flutter app has a package name that uniquely identifies your app, and you can set it using the flutter create command.
 
If you have a domain name called “example.com,” then your package name should be “com.example projectname“. You can set this package name using a --org flag in the flutter create command.
 
This will create a new Flutter project in the current directory where the project name is “counter” and the package name is “com.example.counter.”
 
When you create a Flutter app, the “main.dart” file found in your project’s “counter/lib” folder will be populated with a demo application (its code can be modified, as shown below), which you can run immediately!
 
## 3. Running Your First Flutter Application
 
After generating your Flutter project, open the project directory in your favorite code editor. For instance, if you’re using Visual Studio Code, run code counter in the Terminal to open your project directory (“counter” in our case) in VSCode.
 
Use the CTRL + ` command to open a Terminal inside the editor, which you’ll use to run your first Flutter application by typing:
 
If you’ve done everything correctly, you should be running your Linux application on your desktop. It’s a simple app that lets you press a “+” (Add) to increase the centrally-placed counter.
 
## Basic Concepts of Flutter Apps
 
Before starting to edit parts of this demo code, you will need to understand a few concepts that are unique to Flutter. Open the “counter/lib/main.dart” file in your code editor to observe a couple of aspects:
 
- main() – this is a function that represents the starting point of the application.MyApp() – this is a Flutter widget. Think of widgets as basic building blocks of Flutter. They come in two flavors: Stateless and Stateful.

 
### 1. Stateless Widgets in Flutter
 
Stateless widgets are basic widgets, which contain other widgets and can’t be altered once they are built. As the name suggests, Stateless widgets don’t have any state on their own. MyApp() is an example of a Stateless widget. It contains the MaterialApp() widget but doesn’t have any reactivity, as it’s visible in the code itself:
 
### 2. Stateful Widgets in Flutter
 
In contrast, Stateful widgets can be altered once they are built. In the demo app, you’ve seen a “counter” value change as we pressed the button. This is achieved through the use of Stateful widgets, as seen in the code where:
 
- MyHomePage is a Stateful widget. Inside _MyHomePageState class, notice the variable named _counter, which is initialy set to 0.Clicking the button in the demo will cause the _incrementCounter() function to run and increase the value by 1. The setState() function inside _incrementCounter() re-renders the MyHomePage widget, and an updated _counter value gets displayed on the screen.

 
## Customizing Your App
 
Inside the MyApp widget, you can, for example, change the title string from “Flutter Demo Home Page” to “Make Tech Easier”:
 
You can also change the application theme using the primarySwatch property of the MaterialApp widget. By default, you get a blue color theme. To change this color to green, just replace “Colors.blue” to “Colors.green”:
 
To see the changes, go to your Terminal and hit r on your keyboard to hot reload the application. You can instantly see that the application color and title are changed.
 
This is a very basic tutorial to give you an idea of how Flutter works and how you can get started with Linux app development by using it. If you are interested and want to learn more, follow this getting started guide from the Flutter website.
 
## Frequently Asked Questions
 
Image credit: Carl Heyerdahl via Unsplash. All screenshots by Hrishikesh Pathak
 
### Can you create websites with Flutter?
 
Yes. Flutter also supports web development. You can write the code and deploy your application on mobile, desktop, and web platforms. After building your web application, you can submit your web application to Cloudflare pages or other static site-hosting platforms.
 
### Can you run shell commands in Flutter?
 
Running shell commands is crucial if you’re developing for Linux. Flutter offers this functionality out of the box using dartIO. If you are a Linux beginner, get up to speed with the basics of shell scripting in Linux by checking out our dedicated article on the matter.
 
### How can I deploy my Flutter Linux applications?
 
The official way to deploy the Flutter Linux application is by using Snap packages. Alternatively, you can release them to the Snap Store. But as Flutter builds statically linked binaries, you can package these by using Appimage, Flatpak, or native packaging formats like “.deb” or “.rpm.” 
 
Developer and writer. Write about linux and web.
 
Our latest tutorials delivered straight to your inbox




