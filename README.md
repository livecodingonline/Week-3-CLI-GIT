# Week-3-CLI-GIT
##Command line
The command line (cli, shell) is the interface between you (the user) and the operating system which interprets your commands and allows the computer to respond to your command.
# Commands

## General syntax
`command_name param1 param2 [OPTIONS]`
In the above, square brackets denote the optional part of the command.
The square brackets are not supposed to be typed.
`param1` and `param2` are COMPULSORY parameters.
## Some commonly used commands

`ls` - show the contents of the directory. `ls -a` will show all hidden files. `ls -l` will show more files in long format (more details)

`pwd` - print the Present Working Directory. What directory am I in? 

`cd` - change directory to the one specified. If no directory is specified this will take you to your home directory. Remember that `.` is the current directory and `..` is the parent directory. So `cd .` changes the directory to the current directory (does nothing!). 

`echo` - prints the string on screen (on desktop/bash terminal). `echo -e "hello\n"` will interpret `\n` as newline.

`cat` - print the contents of the file - this will print the WHOLE file. If you want to pause printing after a full screen use the below command.

`less` - show one screen full of the file (spacebar/Enter moves forward and q stops printing)

`head` - show the beginning of a file e.g. `head -3` shows the first 3 lines of the file

`tail` - show the end of a file `tail -4` shows the last 4 lines of the file

`tail -f -100` - shows last 100 lines of a log file, while it's being updated. The output of the command will be automatically updated as well. This is the best way to watch logs.

`wc` - show the word count of a file (prints number of lines, words and characters in the file)

`CTRL-c` - stop what is happening on the command line 

`CTRL-z` - hard stop what is happening on the command line 

`mkdir` - create a new directory

`touch` - create an empty file
