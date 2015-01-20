---
layout: post
title: A few applications of the Unix alias command
publish: true
---

I recently stumbled on the Unix 'alias' command, and began wondering
how i could apply it to my daily tasks. Suddenly, i was hit by a ton
of ideas on how to get things done faster with such a command.


The terminal(command line) provides a fruitful and excitingly
versatile  environment for a wide array of computing tasks. For example, a user
downloads a file titled 'alias.txt' into the 'Downloads' folder, and
wants to copy or move this file to the 'Documents' folder. Most
millenials will use the mouse to click through to the 'Downloads'
folder, copy the 'alias.txt' file, navigate back to the 'Documents'
folder and paste the copied file. A swift analysis on this combo of
clicks and navigation would show that the clicking user will  spend
more time on the task than a counterpart using the terminal. Here is
 the simulated action in the terminal:

*cd ~/Downloads && cp alias ~/Documents*

Note: I'm assuming the users are on a Unix environment

In a flash, that command is executed, and i presume the command line
user will be more productive.

Now back to the alias command. Having seen that the terminal is a
little faster and more flexible, we might even enjoy more of it by
tweaking it to our taste.

Like in everyday life, the alias command simply enables the
replacement of words by another word or string. Interestingly, it can
be used to alias longer commands, enabling users to type less key
strokes and get more done. Below is an alias syntax:

*alias new_name original_name*

In my case, i spend a lot of time in the terminal. I move between
project files, my home directory, my dropbox folder etc. I have
happily used the alias command to simplify these movements. Below are
a few ways i use this command:

*alias home='cd ~'*

With this setting, all i need to do is type 'home' in the terminal to
move to the home directory. I guess this is way shorter and far more
productive than typing 'cd ~' every time.

*alias docs='cd ~/Documents'*

Similarly, i use the newly created 'docs' alias to move to my
documents folder anytime.

Other ways,

*ll ='ls -l'*
*la ='ls -a'*

Definitely, 'man alias', 'help alias' will provide you with more
information on this powerful tool. Now go on and enjoy life in the terminal.
