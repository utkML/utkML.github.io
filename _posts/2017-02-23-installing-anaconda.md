---
layout: post
section-type: post
title: Installing Anaconda
subtitle: By Tyler Stuessi
category: Tech Tips
tags: [ 'anaconda', 'python', 'r' ]
---


Anaconda is a core part of making life easier as a data scientist. It installs both Python and R, and it comes pre-packaged with the most common scientific computing packages for both languages. It also gives you access to Jupyter notebooks, which are incredibly useful for writing readable and well-documented code. Here is how to install Anaconda:

## Installing on Windows
For Windows, you will want to start by downloading the 64-bit installer found [here](https://www.continuum.io/downloads "Anaconda Download Page"). Run the installer and agree to the licenses. 

Once you have done that, you should get to a screen asking you to install "for me only" or for the system. Normally, installing "for me only" is the better way to go, as if you have multiple users on the system they might want different versions of Anaconda. Go ahead and choose where you want it to install (normally the default location is fine). You should then get to the advanced instructions:

> Add Anaconda to my PATH environment variable

This will change your path so that you can easily access the Anaconda packages, and for most cases you will want to leave this checked. Note that this will change your default distribution of Python when you run it from the command prompt.
> Register Anaconda as my default Python

If you wanted to use an IDE with Python, leave this checked.

After this, it will install Anaconda and all its packages. You can run all of the usual commands from the command prompt!

## Installing on Mac
For the command line method, check out the Linux guide.

Installing with the GUI on a Mac is fairly simple. Just download the GUI installer found [here](https://www.continuum.io/downloads "Anaconda Download Page") and double click on the .pkg file. Once you agree to all of the conditions, you will get to a screen asking you to choose who to install for. You will want to choose "Install for me only" so that the anaconda directory will be put in your home area. The next screen will start the installation.

Once the installation is finished, there is only one thing left to do. If you are using a shell other than bash, you will need to add the anaconda/bin folder to your path in your shell config file. In zsh, this will look like adding this line to your .zshrc file:

```shell
export PATH=/Users/yourusername/anaconda/bin:$PATH
```
Once you have this set, you can run any of the Anaconda commands. Note that running Python from the command line will now give you the Anaconda version of Python.

## Installing on Linux
Just as before, go [here](https://www.continuum.io/downloads "Anaconda Download Page") and download the Anaconda package. To install it, all you have to do is go to the command line and run the following command in the directory where you saved the downloaded file (Note that it will not install to that directory):

```shell
>> bash Anaconda3-4.3.0-Linux-x86_64.sh
```
This will run the installer in your shell. After hitting enter a few times to get through the license and approving it, it will ask you to give a location to install Anaconda. The default location will work fine for most purposes.

Next it will install everything, which could take anywhere from a few minutes to half an hour. After that, the only thing left is to make sure that anaconda/bin is in your path, which can be done the same as in the Mac section above. Note that if you are using bash, you do not need to do this step.

By Tyler Stuessi