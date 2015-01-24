# Linux Commands

#### Class: CS 477
#### Team:  OpenDoor                       
--------------------------------------------------------------------------------
*note: this file is written using markdown.  Please edit it using the markdown syntax, described here:*  
*[Extensive Syntax](http://daringfireball.net/projects/markdown/syntax)  
[Github Cheat sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#tables)*

I am going to keep this document in our repository so we can put all helpful and needed linux terminal commands here.  This way, everyone can benefit from everyone's knowledge.

I just made up a structure for this document.  Everyone, please change this to suit your needs, and push a new version.  We will try to combine everybody's ideas and make it nice.

---------------------------------------------------------------------------------
### 1. BASH - basic terminal commands
---------------------------------------------------------------------------------
**BASH** is the Bourne Again Shell.  Read more about it here: [BASH](http://www.gnu.org/software/bash/.)

Here are some helpful linux commands I know.  Feel free to add (guess at the table syntax).  I knew some already, and found a bunch more helpful files at [tecmint](http://www.techmint.com/useful-linux-commands-for-newbies/):

Command				|Result
:-----------------------	|:------------------------------------------------------
`cd <directory>`		|change current directory to the path supplied 
`cd /`				|change current directory to root
`cd ~`				|change directory to your user directory, ex: `/usr/aaron`
`cd $HOME`			|analogous to `cd ~`
`ls`				|list files & folders in the current directory	
`ls -a`				|list all, including hidden items beginning with '.')
`ls -l`				|list a verbose list that lists permissions, size, and date modified.
`lsblk`				|list all drives and partitions mounted on your system.
`pwd`				|print working directory, ex. `/usr/aaron/Documents`a
`mkdir <directory-name>`	|creates a new directory with the given name.
`more <filename>`		|print the entire contents of a file into the terminal.
`less <filename>`		|print the contents of the file with a browser view (type the keys `esc + : + q + enter` to exit)
`cat <filename>`		|print the contents of the given file to the terminal.
`cat > <filename>`		|type at least one line of text with a newline at the end, then save the output with `ctrl + d` to pipe the text into a new file with the given name.
`cat >> <filename>		|concatenate some input text (in the same input manner as the previous command) to the end of the given file.
`touch <filename>`		|creates a new file, or updates the timestamp of an existing file.
`mv <path1> <path2>`		|move the contents of path1 into path2 (will create a new file or directory if necessary)
`rm <filename>`			|remove the named file
`rm -r <directory-name>`	|recursively remove the named directory and all of its contents *(caution!)*
`sudo <command>`		|run as super-user, or 'root'.  Requires your password.
`apt-get install <package name>`|install the package name, if the package manager `apt-get` can `find it in your repositories.`	|Usually requires use of `sudo`.
`uname -a`			|print detailed inofrmation abotu the machine name, OS and system kernel.
`history`			|dumps your previous commands into the terminal output.
`cal`				|print a calendar
`date`				|print the current date



--------------------------------------------------------------------------------
General GNU/Linux Knowledge
--------------------------------------------------------------------------------
Here is a place to share all general information concerning how to use linux distros like Ubuntu or Mint that we think may benefit other team members.

### terminal keyboard shortcuts
Shortcut                    	|Result
|:-----------------------------	|:----------------------------------------------
`ctrl + alt + t`		|Open a new terminal window
ctrl + c			|escape the currently running command
arrow `up` or `down`		|scroll though your previously entered commands
`ctrl + left`			|jump to the beginning of input text
`ctrl + right`			|jump to the end of the input text
`shift + ctrl + c`		|copy 
`shift + ctrl + v`		|paste


