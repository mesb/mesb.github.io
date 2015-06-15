---
layout: post
title: On data Persistence!
publish: true
---
# On Data Persistence and Configuration Files<a id="sec-1" name="sec-1"></a>

Persistence can be defined as the continued or prolonged existence of
something. Persistence plays an important role in computing. Random
Access Memory (RAM) is fast and volatile, meaning its contents get
erased when the system is powered off. However, we still recognize
our computers when ever we login. This is the power of persistence in
computing.

Persistence makes computing systems to have personality. You
configure a system and it remembers these configurations till you
decide to explicity change them. The major abstraction for
persistence is the 'file system'. Unlike the RAM, files stored on
devices on are there to stay.

This ability to store files can be used to do real good, especially
on Unix environments. Unix was originally known as the Programmer's
Work Bench (PWB), because of its ease of configuration and clean
design. Programmer's would customize their Unix environments in every
possible way to derive a comfortable working environment.

Take the shell, also known as the terminal, for example. It can be
used to perform file and directory manipulations among other
versatile tasks. Navigating to the notes directory in the Documents
folder can be done by the command:

*cd ~/Documents/notes*

Since laziness is a virtue, i won't want to type 'cd
~/Documents/notes' every time. Unix being flexible and
customizable provides a command just for people like me(and maybe
you), the *alias* command. 

/alias notes='cd ~/Documents/notes'/

This would register **notes** to be a shortcut for the long **cd ~/Documents/notes/** command. 
However, making alias entries in the terminal is not persistent. The
registered aliases won't work when the shell is restarted. A solution
to this, as it is for many configurable systems, is to save the
aliases in a configuration file. I have come to realize that providing
configuration files is a popular and clean way of making programs and
systems customizable by users, which is
common to Unix applications such as emacs, vim, and the terminal.

Interestingly, to avoid the RAM effects on our settings, aliases in
this case, we need to manipulate any of the 2 files listed
below. Feel free to create these files in your home Unix home
directory if they don't exist:

1.  ~/.bash<sub>profile</sub>
2.  ~/.bashrc

What do these files do?
Initialization is an important step in computational processes. When the
terminal is started by a user, the system first looks for personal
configurations in a series of files. 

~/.bash<sub>profile</sub> : has higher precedence. 

Common settings to put in these files are environmental variable configurations, custom messages to print when the terminal starts,
aliases etc

Moreover, to make our aliases persistent, we should save them in the
**~/.bash<sub>profile</sub>** or **~/.bashrc** files. I personally prefer **~/.bashrc**
because it easier to type. In this file, we can store our custom
settings:

/alias notes='cd ~/Documents/notes'/

Fun experiments with this file are:

1.  Display current directory when terminal starts by adding **pwd** to
    the top of your config file
2.  list contents of current directory by adding **ls -l** to config file

As is the goal of data persistence, your settings will remain in the
system till you need them no more. A variety of Unix applications use
this config/settings file model to enable users to customize their
enviroments:

-   Emacs : Uses *~*.emacs, ~/.emacs.d/init.el/
-   Vim : Uses *~*.vimrc/
-   Git : Uses *~*.gitconfig/

In a nutshell, persistence is essential in data storage, personality,
and customization.

