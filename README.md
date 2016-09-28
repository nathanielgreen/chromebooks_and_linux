# Chromebooks and Web Development

This is a guide primarily built for Makers Academy students after their 12 weeks
of using macOS for development and how they can make the change over to Linux on
Chromebooks for their future web development needs.

This guide assumes a few things:-

- Little to no prior Linux/ChromeOS experience and/or knowledge.
- You plan on using this guide for setting up a dev machine/environment that 
  can be used during and after Makers Academy, primarily for web development.
- You will want to run Linux alongside ChromeOS, rather than replacing the OS
  entirely.

# Contents

- 1. Chromebooks and Linux
    - 1.1 [Why Chromebooks?](#id-whychromebooks)
    - 1.2 [Why Linux?](#id-whyLinux)
        - 1.2.1 [Package Managers and Homebrew](#id-packagemanagers)
        - 1.2.2 [ChromeOS and Distributions](#id-chromeosdistributions)
    - 1.3 [What Chromebooks](#id-whatchromebooks)

- 2. Installing Linux on your Chromebook Tutorial
    - 2.1 [Intro](#id-tutorialintro)
    - 2.2 [Enabling Developer Mode](#id-tutorialdevelopermode)
    - 2.3 [Install Crouton](#id-tutorialcrouton)
    - 2.4 [Install Ubuntu](#id-tutorialubuntu)

- 3. Further Linux
    - 3.1 [Distributions and Desktop Environments](#id-distrosanddes)
        - 3.1.1 [Desktop Environments](#id-des)
        - 3.1.2 [Window Managers](#id-wms)
        - 3.1.3 [Distributions](#id-distros)
               


# Chromebooks and Linux

## 1.1 Why Chromebooks?
<div id='id-whychromebooks' />

Chromebooks are (mostly) fairly cheap laptops that run an operating system called
[ChromeOS](https://en.wikipedia.org/wiki/Chrome_OS). This is built on top of 
Linux, and it is possible through a set of scripts called 
[crouton](https://github.com/dnschneid/crouton) to access the Linux shell and 
run another linux distribution (e.g. Ubuntu, Debian) alongside ChromeOS. 

This allows one to setup a Linux environment fairly easily, without having to
worry about compatible hardware or certain drivers being incompatible, or not
working entirely, as well as being able to reinstall Linux or distro hop fairly
easily if your first install becomes corrupted or no longer wanted, 

## 1.2 Why Linux?
<div id='id-whyLinux' />

If you've used macOS for web development, you'll likely be familiar with the
command line and programs for it such as git, Homebrew, rvm, Heroku etc. These
all mostly work the same on Linux (aside from Homebrew, I'll get into that in a
second) and only require slightly different configuration, in which I'll go over
in the tutorial.

A lot of Linux software and programs, including some of the distributions
themselves, are also open source, allowing a lot of control and customization
within your OS.

### 1.2.1 Package Managers and Homebrew
<div id='id-packagemanagers' />

When using macOS, you probably used a package manager called
[Homebrew](http://brew.sh/) to install things such as Node, and maybe even 
[Homebrew Cask](https://caskroom.github.io/) to install programs like Google
Chrome and Atom.

Depending on what Linux distribution you go for (in this tutorial we'll mostly on
cover Ubuntu), will decide on the type of 
[package manager](https://en.wikipedia.org/wiki/Package_manager) you have. In Ubuntu's
case you'll have the package manager 'apt-get'. 

There are certain differences
between package managers such as them either being a CLI or having their own
separate GUI (homebrew for example being mostly CLI-based), as well as having
different commands.

### 1.2.2 ChromeOS and Distributions
<div id='id-chromeosdistributions' />

Following the tutorial below will result in your chromebook having
[ChromeOS](https://en.wikipedia.org/wiki/Chrome_OS) and Ubuntu 
running alongside each other (that is, once you run Ubuntu from the
ChromeOS shell). 

Ubuntu is just one of the 
[many Linux distributions](https://en.wikipedia.org/wiki/List_of_Linux_distributions),
and depending on what sort of features you look for in an operating
system will likely decide what distribution you choose.

In this guide however, we'll be using
[Ubuntu](https://en.wikipedia.org/wiki/Ubuntu_(operating_system)) a Debian-based Linux OS,
that focuses on the use of free and open-source software.

I chose this OS for the guide as it's one of the most popular distributions
currently, making finding support, guides, and other tutorials fairly painless.
It's default user interface/desktop environment,
[Unity](https://en.wikipedia.org/wiki/Unity_(user_interface)) is also
user-friendly, with  most settings/options having a GUI. **However**, in this
tutorial we'll be installing Ubuntu with the [XFCE](https://www.xfce.org/) 
desktop environment, as it use less system resources than Unity and will 
run smoother on more low-end chromebooks. For more information on Desktop
Environments and their differences, refer to [this section](#id-des) of the guide.

If you'd like to know more about what different distributions you can install on
your chromebook, refer to [this section](#id-distros) of the guide.

## 1.3 What Chromebooks?
<div id="id-whatchromebooks" />

There a lots of resources of choosing a Chromebook depending on your specific
needs, such as
[whichchromebookshouldibuy](http://whichchromebookshouldibuy.com/). When looking
for a chromebook to run Linux, you want to make sure it has an Intel Processor, 
at least 32GB of SSD storage, and ideally 4GB of RAM.

Also another thing to note is that most chromebooks only come with either
16/32/64GB of internal storage, and often come with a SD card slot. This is
sufficient as long as you're not storing anything like games or lots of 
photos/videos you should be fine storage-wise.

My personal recommendations would be as follows:


- A good baseline all-rounder is the [Acer Chromebook
  R11](http://www.acer.com/ac/en/US/content/series/acerchromebookr11):

    - Intel Celeron Quad-core 1.6Hz
    - 2GB/4GB RAM
    - 32GB SSD
    - 11.6 inch 16:9 1366x768 touchscreen display
    - Convertible to tablet mode
    - ~8 hour battery life
    - Price: ~£199/~£229

    This is a decent chromebook if you're planning on using this until you get a job,
    and the using whatever laptop is provided by them as a daily driver,
    alongside this chromebook.

- The [Dell Chromebook 13](http://www.dell.com/uk/business/p/chromebook-13-7310/pd) 
  is another offering that has different configurations depending on your budget:
    - Intel Celeron 3205U Dual-core 1.5GHz/Intel Celeron i3-5005U Dual-core
      2.0/2.3GHz
    - 4GB/8GB RAM
    - 16GB/32GB SSD
    - 13.3 inch 16:9 1920x1080 matte display
    - Touchscreen option.
    - ~12 hour battery life
    - Price: ~£450 up to ~£850
 
- If you're planning on using this laptop very long-term and possibly even at
  your workplace, the [Chromebook Pixel 2015](https://pixel.google.com/chromebook-pixel/) 
  by Google themselves is the best, but also most expensive option: 
    - Intel i5/i7 2.6 Ghz Processor
    - 8/16GB RAM
    - 32/64GB SSD
    - 12.85 inch 3:2 2560x1700 touchscreen display
    - ~12 hour battery life
    - Price ~£800/~£1000

    I actually am using the i5/8GB RAM Pixel model daily so if you have any questions
    about the Pixel specifically, shoot me a message and I'll give you a look.


# Installing Linux on Your Chromebook Tutorial

## 2.1 Intro
<div id="id-tutorialintro" />

In this guide we'll go through the steps required to setup the Ubuntu
distribution of Linux on your chromebook using [crouton](https://github.com/dnschneid/crouton), 
as well as discuss how to go about installing different distributions and
desktop environments/window managers.

## 1. Enabling Developer Mode
<div id="id-tutorialdevelopermode">

**This step will wipe your local data,** so make sure you have any local files
you want to keep backed up onto an external drive or into the cloud.

To put your chromebook into developer mode:

1. Press and hold the Esc and Refresh keys together, then (whilst still holding
   these two keys) press the Power button. This will reboot your Chromebook into
   recovery mode.
2. Once you see the screen for Recovery Mode pop up, (it's a screen with a
   yellow/orange exclamation point) press Ctrl+D. This will then bring up a
   prompt for enabling developer mode. Press Enter to continue.
3. Allow a few seconds after the last step, it should pop up with a different
   screen for a few moment and then begin to reboot, and go through the process
   of enabling developer mode. This may take a while (15ish minutes), and will also
   wipe you local data.
4. Once it's done, the screen with the exclamation point will reappear. Leave it
   alone until it boots into ChromeOS.

## 2. Install Crouton
<div id="id=tutorialcrouton" />

In this step we'll be downloading the set of scripts that allows one to easily
put Linux on ChromeOS called [crouton](https://github.com/dnschneid/crouton).

1. Download by clicking the link at the top of [the crouton github
   repo](https://github.com/dnschneid/crouton), or use the direct download link
   [here](https://goo.gl/fd3zc). It should be saved into your Downloads folder.
2. Press Ctrl+Alt+t to open up a terminal.
3. Type `shell` in the terminal to enter the shell in which we'll run the
   installation commands.

At this stage, crouton provides some different commands depending on what sort
of distribution and desktop environment you prefer. To learn more about the
different distributions and desktop managers [here](#id-distrosanddes).

To see a list of recognized releases and the distros they belong to run: `sudo sh
~/Downloads/crouton -r list`. 

For the sake of this tutorial however we'll be installing the distribution
Ubuntu version 14.04 with the XFCE desktop environment.

## 3. Install Ubuntu
<div id="id-tutorialubuntu" />

1. In the same terminal in which you type `shell`, run the command `sudo sh -e
   ~/Downloads/crouton -t xfce`.
2. Let your computer download and install Ubuntu and XFCE. It may take a while
   (up to 15 minutes, depending on your connection). When the download is
   nearing completion, it will ask you for a username and password you want to use
   for Ubuntu, these can be what you wish.
3. After the installation is finish you can run the following command to enter
   Ubuntu with XFCE: `sudo startxfce4`.

To switch between ChromeOS and Ubuntu while they're both running, 
press Ctrl+Alt+Shift+Back or Ctrl+Alt+Shift+Forward 
(with the back and forward keys being the ones on the function row next to Esc).



# Further Linux

## 3.1 Distributions and Desktop Environments
<div id="id-distrosanddes" />

If you're interested in trying out different flavours of Linux and the tools it
offers, crouton does provide the tools to install different distributions 
and desktop environments, or they can be installed on what you have installed 
from the tutorial, after the fact.

### 3.1.1 Desktop Environments (DEs)
<div id="id-des" />

Desktop environments determine the sort of GUI you interact and what it looks
like. For example, the default desktop environment Ubuntu comes with is called
[Unity](https://en.wikipedia.org/wiki/Unity_(user_interface)), which is built on
top of the [GNOME](https://en.wikipedia.org/wiki/GNOME) desktop environment.

Different desktop environments will offer different features, such as the GNOME
shell having a huge amount of [official and community made
extensions](https://extensions.gnome.org/) that you can choose to download to
suit your workflow. The type of DE you choose may also affect
the way your system works such as some DE's not having HiDPI scaling yet, or
having your workspaces be dynamic as opposed to a fixed number.

### 3.1.2 Window Managers (WMs)
<div id="id-wms" />
A window manager is different to a desktop environment, in that its main
function is just to manager your windows. Window managers are what add all the
window decorations such as buttons to minimize and close. Desktop environments
will usually come bundle with some form WM. 

However, a lot of enthusiasts have chosen to instead run only a lightweight 
window manager in place of a whole desktop environment. One of the more popular
lightweight WMs is [i3 by Airblader](https://github.com/Airblader/i3), and is
actually the one I use (the i3-gaps fork).

i3 itself is a tiling window manager, and comes with Vi style key bindings for
the moving and resizing of windows. Tiling window managers have become
increasingly popular due to the speed and efficiency at which users can resize
and tile their windows with keyboard shortcuts as opposed to dragging the
sides/corners with the mouse in more traditional window managers.

### 3.1.3 Distributions
<div id="id-distros" />

[Ubunutu](http://www.ubuntu.com/) is the distribution we used in this tutorial,
and is one of the most popular linux distributions available, however there are
a [LOT](https://en.wikipedia.org/wiki/List_of_Linux_distributions) of options
for distributions.

The difference between distributions can vary, with some of the difference only
being their desktop environment. For example, Ubuntu being based on
[Unity](https://en.wikipedia.org/wiki/Unity_(user_interface)), Xubuntu using
[XFCE](https://www.xfce.org/) and so on.

Other differences can be the actual goals of the company or community working
on and building the distribution, such as [Fedora](https://getfedora.org/)
aiming to be the first distribution to implement the latest and newest software
and be on the bleeding edge, whereas [Debian](https://www.debian.org/) is more
focused on providing an extremely stable distribution, which means its software
may be more out of date than Fedora's.

