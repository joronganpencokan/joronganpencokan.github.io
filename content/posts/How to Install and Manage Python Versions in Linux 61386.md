---
title: "Unlock the Secrets: The Ultimate Guide to Installing and Mastering Multiple Python Versions in Linux"
ShowToc: true 
date: "2023-06-29"
author: "Estelle Seiber"
---
*****
---
title: "Unlock the Secrets: The Ultimate Guide to Installing and Mastering Multiple Python Versions in Linux"
date: 2022-05-30T10:00:00Z
draft: false
---

## Introduction

Python is a very versatile language with a wide range of applications, from machine learning and data analysis, to web development and game programming. However, different projects require different versions of Python, and sometimes you need to use multiple versions simultaneously. In this guide, you will learn how to install multiple Python versions on Linux, manage them with virtual environments, and master the art of switching between them effortlessly.

## Prerequisites

Before we start, you should have root access to your Linux distribution and a basic understanding of the command line interface. We will use Ubuntu as an example, but the instructions should work on other distributions as well.

## Step 1: Install Python Versions

Ubuntu comes with Python 2 and Python 3 pre-installed, but you might want to use other versions as well. To install them, you can use the `deadsnakes` PPA:

```
sudo apt-get update
sudo apt-get install software-properties-common
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt-get update
```

This PPA contains packages for all Python versions from 2.3 to 3.9, including beta releases and development versions. You can install any version by running:

```
sudo apt-get install python3.8
```

Replace `python3.8` with the desired version number.

## Step 2: Install Virtual Environments

Virtual environments are an essential tool for managing multiple Python versions and dependencies. They allow you to isolate each project's environment, so that you can install different packages and versions without interference.

To install virtual environments, first make sure you have `pip` installed:

```
sudo apt-get install python3-pip
```

Then install the `virtualenv` package:

```
pip3 install virtualenv
```

You can create a new virtual environment by running:

```
virtualenv myenv --python=python3.8
```

This will create a new directory called `myenv` and install Python 3.8 in it. To activate the virtual environment, run:

```
source myenv/bin/activate
```

You should see `(myenv)` in your terminal prompt, indicating that you are now working inside the virtual environment. You can deactivate it by running `deactivate`.

## Step 3: Use `pyenv` for Version Management

While virtual environments are useful for managing dependencies, they do not help you manage multiple Python versions themselves. To solve this problem, we can use a tool called `pyenv`.

`pyenv` allows you to install and switch between multiple Python versions and keep them separate from the system Python. To install `pyenv`, run:

```
curl https://pyenv.run | bash
```

This will download and install `pyenv` in your home directory. Add the following lines to your `~/.bashrc` or `~/.bash_profile`:

```
export PATH="$HOME/.pyenv/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
```

Close and reopen your terminal, and `pyenv` should be ready to use. To install a new Python version, run:

```
pyenv install 3.9.5
```

Replace `3.9.5` with the desired version number. You can list all installed versions by running `pyenv versions`.

To switch the global Python version, run:

```
pyenv global 3.9.5
```

This will set the default Python version for your system. You can also set the version per directory or shell session by using `pyenv local` or `pyenv shell`, respectively.

## Conclusion

Managing multiple Python versions on Linux can seem daunting at first, but with the right tools and practices, it can be a breeze. By installing different versions, using virtual environments, and mastering `pyenv`, you can easily switch between projects and work seamlessly with different versions and dependencies. Happy coding!

{{< youtube sePT9AZauWs >}} 



The Python programming language was introduced in 1991. In all these years, it has gone through many changes, with each version adding and removing various features. Due to these changes, software written in newer versions of Python may or may not work with older versions.
 
This version mismatch costs developer experience and productivity, so it’s important to learn how to manage Python versions installed on your computer to run them all efficiently. This tutorial shows you how to do that.
 
## How to Install a Different Python Version
 
The easiest technique for Python version management is using the native package manager. Python comes installed out of the box on most Linux desktops. It has two major versions: Python2 and Python3. You can confirm if these two versions are available on your computer by using the following commands:
 
To install Python versions other than the preinstalled ones, use the deadsnake PPA (Personal Package Archive) in Ubuntu-based distributions.
 
If you don’t have PPA enabled on your machine, enable it with this command:
 
Use this command to add the deadsnake PPA to your apt source:
 
Now you can install any Python version you want with the following command. Be sure to replace “3.10” with the relevant version number.
 
Use the --version flag to check if your new Python version has been installed properly.
 
Remember, if you check your system’s Python version at this point, it still shows the number of the preinstalled version.
 
If you want to use your newly installed version of Python as the default, you can use the update-alternatives command, which helps set the priority for different versions of the same software. Run the following commands to set python3.10 as the Python version with the highest priority.
 
The second command marks python3.8 to your preinstalled Python version.
 
You can use the following command to switch between different Python versions.
 
## Manage Python Projects With Virtual Environments
 
Python is not good at managing dependencies. If you use the default package installer, pip, or pip3 to install Python libraries and packages, it will install the packages globally. As Linux comes with a preinstalled version of Python and uses different packages to run the operating system, manually installed packages in the global scope can disrupt its functioning. This is where a virtual environment comes in handy. It’s an isolated Python environment that has its own tools and libraries independent of the main setup. Think of a virtual environment as an isolated room that has minimal dependencies.
 
If you don’t use virtual environments, you don’t have any control on the versions of the packages you have used in your project, which is problematic when you try to run your software on a different machine. Therefore, it is advisable to use a virtual environment for your Python projects.
 
## Creating a Virtual Environment With Venv
 
venv is the recommended way to create a virtual environment in Python and it comes preinstalled. If you have never used venv, you should first install its dependencies on your computer with the following command. Change python3.10 to your installed Python version in the command.
 
Now create a new virtual environment using the venv package. We named our virtual environment “venv.” You can name it whatever you want.
 
After creating the virtual environment, activate it by sourcing venv environment variables and commands.
 
Now you can see a (vnev) prefix in your terminal prompt, which means that your virtual environment is now active and ready for installing dependencies. Let’s install a new dependency called “requests” inside our newly created virtual environment.
 
To deactivate the virtual environment, run deactivate within it.
 
## Creating a Virtual Environment With Virtualenv
 
virtualenv is the most popular tool to create Python virtual environments. It is a superset of venv, which means that virtualenv can do all the things venv can and more. 
 
You can create different virtual environments with different versions of Python using virtualenv. It also allows you to use different and specific versions of the same package in projects – a feature not available in the venv package.
 
 virtualenv has a command similar to venv for creating a virtual environment.
 
A new virtual environment named “venv” is created from the command above. To activate the virtual environment, source the activate file.
 
Now you can see a (venv) prefix in your terminal prompt to indicate that the virtual environment has been activated.
 
To create a virtual environment with different Python versions, you should use the --python or -p flag and give the location of the Python executable. For example, if you want to create a virtual environment with Python 2.6, a very old Python version, the command should look like this:
 
## Creating a Virtual Environment With Miniconda/Anaconda
 
Conda is a package manager like pip. But unlike pip, Conda supports many other programming languages and takes a different approach to creating virtual environments. Conda is developed independently from pip.
 
You can use Conda by installing the Miniconda package. If you are into data science and machine learning, you can also install the Anaconda package which includes all the data-science-related packages.
 
To install Miniconda on your Linux machine, download Miniconda for the relevant Python version and run this shell script in your terminal to set up Miniconda automatically.
 
After installation, a default Miniconda environment called “base” is created. If you run the conda install command, the newest versions of the packages you request are installed within the environment. If your Conda environment is not activated, activate it using this command.
 
Conda makes it easy to create environments for different Python versions. All you have to do is specify the correct Python version in the command. Conda will then automatically download, install, and set up all the dependencies for you.
 
For example, if you want Python version 3.7 in a Conda environment, the command should look like this.
 
After creating and activating this environment, you can use it to install your favorite software, such as NumPy:
 
## Run a Python3 Script With “Python”
 
It is more intuitive to type python instead of python3 to run a Python script. You can make this switch automatically if you use the “python-is-python3” package in Linux. After installing this package, the python command automatically uses python3 binaries.
 
The “python-is-python3” package is available in Ubuntu repositories and you can install it using the apt package manager.
 
## Frequently Asked Questions
 
Image credit: Hitesh Choudhary via Unsplash.  All screenshots by Hrishikesh Pathak.
 
### Can installing different Python versions break my system?
 
It’s possible. If your operating system needs some specific features of Python to work properly and they’re deprecated in the Python version installed on your machine, you may experience instability on your machine. In the worst case, your operating system may break and you may have to install it afresh.
 
### Where do virtual environments store Python packages?
 
Virtual environments store packages in specific hidden directories inside the home folder. Different virtual environments have different storage locations to ensure that they don’t pollute the system-level packages and the scopes and don’t interfere with the working of the operating system.
 
### How to remove a virtual environment?
 
You can delete your virtual environments very easily. Go to your project directory and find the directory named after your virtual environment. It stores all the configurations of your virtual environments. Delete this directory and you are good to go.
 
Developer and writer. Write about linux and web.
 
Our latest tutorials delivered straight to your inbox




