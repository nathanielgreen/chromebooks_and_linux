# Chromebooks and Web Development

This is a guide primarily built for Makers Academy students after their 12 weeks
of using OS X for development and how they can make the change over to Linux on
Chromebooks.

This guide assumes a few things:-

- Little to no prior linux/chromeOS experience and/or knowledge.
- You plan on using this guide for setting up a dev machine that can be used
  during and after Makers Academy, primarily for web development.
- You will want to run Linux alongside ChromeOS, rather than replacing the OS
  entirely.

# Contents

1. Chromebooks and Linux
    - 1.1 [Why Chromebooks?](#id-whychromebooks)
    - 1.2 [Why Linux?](#id-whylinux)
        - 1.2.1 [Package Managers and Homebrew](#id-packagemanagers)
        - 1.2.1 [ChromeOS and Distributions](#id-chromeosdistributions)
    - 1.3 [What Chromebooks](#id-whatchromebooks)
       

# Chromebooks and Linux

## Why Chromebooks?
<div id='id-whychromebooks' />

Chromebooks are (mostly) fairly cheap laptops that run and operating system called
ChromeOS. This is built on top of Linux and it is possible through a set of
scripts called [crouton](https://github.com/dnschneid/crouton) to access the
linux shell and run another linux distribution (e.g. Ubuntu, Debian) alongside
ChromeOS. 

This allows one to setup a Linux environment fairly easily, without having to
worry about compatible hardware or certain drivers being incompatible or not
working entirely. 

## Why Linux?
<div id='id-whylinux' />

If you've used OS X for web development, you'll likely be familiar with the
command line and programs for it such as git, homebrew, rvm, heroku etc. These
all mostly work the same on Linux (aside from homebrew, I'll get into that in a
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

Depending on what linux distribtuion you go for (in this tutorial we'll mostly on
cover Ubuntu), will decide on the type of package manager you have. In Ubuntu's
case you'll have the package manager 'apt-get'. 

There are certain differences
between package managers such as them either being a CLI or having their own
seperate GUI.

### ChromeOS and Distributions
<div id='id-chromeosdistributions' />

## What Chromebooks?
<div id="id-whatchromebooks" />

There a lots of resources of choosing a Chromebook depending on your specific
needs, such as
[whichchromebookshouldibuy](http://whichchromebookshouldibuy.com/). When looking
for a chromebook to run linux, want to make sure it has an Intel Processor, and
ideally 2-4GB of RAM. 

Also another thing to note is that most chromebooks only come with either
16/32/64GB of internal storage, and often come with a SD card slot. This is
sufficient as long as you're not storing anything like games or lots of 
photos/videos you should be fine storage-wise.

My personal recommendations would be as follows:

For the baseline all-rounder I'd recommend: [Toshiba Chromebook
2](https://www.amazon.co.uk/Toshiba-PLM02E-00D003EN-CB30-B-104-Chromebook-Celeron/dp/B00RK7LFEG/ref=sr_1_3?ie=UTF8&qid=1463570959&sr=8-3&keywords=toshiba+chromebook+2):
- Intel Celeron 2.16 GHz
- 4GB RAM
- 16GB SSD
- 13.3 inch screen
- Price: ~250.00
This is a good chromebook if you're planning on using this until you get a job,
and the using whatever laptop is provided by them as a daily driver.




