# Chromebooks and Web Development

This is a guide primarily built for Makers Academy students after their 12 weeks
of using OS X for development and how they can make the change over to Linux on
Chromebooks.

This guide assumes a few things:-

- Little to no prior Linux/chromeOS experience and/or knowledge.
- You plan on using this guide for setting up a dev machine that can be used
  during and after Makers Academy, primarily for web development.
- You will want to run Linux alongside ChromeOS, rather than replacing the OS
  entirely.

# Contents

1. Chromebooks and Linux
    - 1.1 [Why Chromebooks?](#id-whychromebooks)
    - 1.2 [Why Linux?](#id-whyLinux)
        - 1.2.1 [Package Managers and Homebrew](#id-packagemanagers)
        - 1.2.1 [ChromeOS and Distributions](#id-chromeosdistributions)
    - 1.3 [What Chromebooks](#id-whatchromebooks)

2. Installing Linux on your Chromebook Tutorial
    - 2.1 [Intro](#id-tutorialintro)
    - 2.2 [Enabling Developer Mode](#id-tutorialdevelopermode)
       

# Chromebooks and Linux

## Why Chromebooks?
<div id='id-whychromebooks' />

Chromebooks are (mostly) fairly cheap laptops that run and operating system called
ChromeOS. This is built on top of Linux and it is possible through a set of
scripts called [crouton](https://github.com/dnschneid/crouton) to access the
Linux shell and run another linux distribution (e.g. Ubuntu, Debian) alongside
ChromeOS. 

This allows one to setup a Linux environment fairly easily, without having to
worry about compatible hardware or certain drivers being incompatible or not
working entirely. 

## Why Linux?
<div id='id-whyLinux' />

If you've used OS X for web development, you'll likely be familiar with the
command line and programs for it such as git, Homebrew, rvm, Heroku etc. These
all mostly work the same on Linux (aside from Homebrew, I'll get into that in a
second) and only require slightly different configuration for some which I'll
give a tutorial for here.

A lot of Linux software and programs, including some of the distributions
themselves, are also open source, allowing a lot of control and customisation
within your OS.

### Package Managers and Homebrew
<div id='id-packagemanagers' />

When using Mac OS X, you probably used a package manager called
[Homebrew](http://brew.sh/) to install things such as Node, and maybe even 
[Homebrew Cask](https://caskroom.github.io/) to install programs like Google
Chrome and Atom.

Depending on what Linux distribtuion you go for (in this tutorial we'll mostly on
cover Ubuntu), will decide on the type of 
[package manager](https://en.wikipedia.org/wiki/Package_manager) you have. In Ubuntu's
case you'll have the package manager 'apt-get'. 

There are certain differences
between package managers such as them either being a CLI or having their own
seperate GUI (homebrew for example being mostly CLI-based), as well as having
different commands.

### ChromeOS and Distributions
<div id='id-chromeosdistributions' />

Following the tutorial below will result in your chromebook having [ChromeOS]()
and Ubuntu running alongside eachother (that is, once you run Ubuntu from the
ChromeOS shell). 

Ubuntu is just one of the 
[many Linux distributions](https://en.wikipedia.org/wiki/List_of_Linux_distributions)
and depending on what sort of features you look for in an operating
system will likely decide what distribution you choose.

In this guide however, we'll be using
[Ubuntu](https://en.wikipedia.org/wiki/Ubuntu_(operating_system)) a Debian-based Linux OS,
that focuses on the use of free and open-source software.

I chose this OS for the guide as it's one of the most popular distributions
currently, making finding support, guides, and other tutorials fairly painless.
It's default user interface/desktop environment,
[Unity](https://en.wikipedia.org/wiki/Unity_(user_interface)) is also
user-friendly, with  most settings/options having a GUI.
The version we'll be installing in the tutorial also runs very stable on most
Chromebooks.

If you'd like to know more about what different distributions you can install on
your chromebook, refer to [this section]() of the guide.

## What Chromebooks?
<div id="id-whatchromebooks" />

There a lots of resources of choosing a Chromebook depending on your specific
needs, such as
[whichchromebookshouldibuy](http://whichchromebookshouldibuy.com/). When looking
for a chromebook to run Linux, want to make sure it has an Intel Processor, and
ideally 2-4GB of RAM. 

Also another thing to note is that most chromebooks only come with either
16/32/64GB of internal storage, and often come with a SD card slot. This is
sufficient as long as you're not storing anything like games or lots of 
photos/videos you should be fine storage-wise.

My personal recommendations would be as follows:

- For the baseline all-rounder I'd recommend: [Toshiba Chromebook
2](https://www.amazon.co.uk/Toshiba-PLM02E-00D003EN-CB30-B-104-Chromebook-Celeron/dp/B00RK7LFEG/ref=sr_1_3?ie=UTF8&qid=1463570959&sr=8-3&keywords=toshiba+chromebook+2):
    - Intel Celeron 2.16 GHz
    - 4GB RAM
    - 16GB SSD
    - 13.3 inch 16:9 1920x1080 display
    - Price: ~250.00

    This is a decent chromebook if you're planning on using this until you get a job,
    and the using whatever laptop is provided by them as a daily driver,
    alongside this chromebook.

- If you're planning on using this laptop very long-term and possibly even at
  your workplace, the [Chromebook Pixel 2015](https://pixel.google.com/chromebook-pixel/) 
  by Google themselves is the best, but also most expensive option: 
    - Intel i5/i7 2.6 Ghz Processor
    - 8/16GB RAM
    - 32/64GB SSD
    - 12.85 inch 3:2 2560x1700 display
    - Price: 800.00/1000.00

    I actually am using the i5/8GB RAM model daily so if you have any questions
    about the pixel specifically, shoot me a message and I'll give you a look.
    

# Installing Linux on Your Chromebook Tutorial

## Intro
<div id="id-tutorialintro" />

In this guide we'll go through the steps required to setup the Ubuntu
distribution of Linux on your chromebook using [crouton](https://github.com/dnschneid/crouton), 
as well as discuss how to go about installing different distributions and
desktop environments/window managers.

## 1. Enabling Developer Mode
<div id="id-tutorialdevelopermode">

# **INCOMPLETE**
