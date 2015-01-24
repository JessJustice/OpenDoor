# OpenDoor - Github 
#### Class: CS 477
#### Team:  OpenDoor
--------------------------------------------------------------------------------
*note: this file is written using markdown.  Please edit it using the markdown syntax, described here:  
[Extensive Syntax](http://daringfireball.net/projects/markdown/syntax)  
[Github Cheat sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#tables)*

Hi team!  I set up this git repository so we can all contribute helpful stuff
to one area.  Place whatever files we want to share with each other here.

### Connect to this git repository
 
```git clone https://github.com/aaroncarsonart/OpenDoor.git```


---------------------------------------------------------------------------------
### 1. GITHUB - basic terminal commands
---------------------------------------------------------------------------------
Like the `linuxCommands.md` file, read and contribute to this file to help everyone get on the same page with using git and github. 

Here are some helpful linux commands I know.  [This tutorial](http://git-scm.com/docs/gittutorial) is very helpful for understanding basic commands.  Feel free to add and clarify any of my descriptions of commands here (guess at the table syntax for adding rows):

#### 1. Basic Functionality
Command                       |Result
:-----------------------      |:------------------------------------------------------
`git init MyProject`          |initialize a new git repository in the current directory named *MyProject*
`git add file1 file2 etc`	    |add the specified file(s) to the index, to prepare for a commit
`git add .`			                |adds all new or updated files to indexc to prepare for a commit
`git commit -a -m "Comments"` |commit files into version control, and pass a comment string (convenience form) 
`git commit`                  |commit added files into version control, prompt the user for typing commments in vim (escape vim with key sequence `esc` + `:` + `w` + `q`)
`git commit -m "Comments"`    |commit added files, specifying comments in the string.
`git commit -a`               |commit all *updated* files (don't have to use `git add` with this option, unless you make a new file)
`git diff`                    |view changes that have not been added to the index.
`git diff --cached`           |view what will be commited, including changes and/or conflicts
`git status`                  |view summary of your repository, including which branch you are on and if you are up-to-date.
`git log`                     |view a log of the history of the repository (press `q` to escape the view)
`git log -p`                  |view even more information about the history (log + the diff info)
`git log --stat --summary`    |view the log another different way.

#### 2. Branching
Command                     |Result
:-----------------------	   |:------------------------------------------------------
`git branch NewBranch`    		|create a new branch for your project
`git branch`			             |view all branches in your repository
`git checkout NewBranch`	   |switch into the *NewBranch* branch of your repository.  Now any time you access your repository file, from the terminal, a file manager, or any other program, it will see files stored in this branch instead.  
`git checkout master`	     	|switch into your main, "master" branch.  Any files you didn't commit to NewBranch still exist in their modified state in NewBranch; but they aren't placed into version control, so if you modify that file you can't go back to previous edits.  Generally, after you edit a file, you should run `git commit -a -m "what you changed"`.  And, if you made a new file, you must either explicitly add it with `git add <filename>` or add all new/changed files with `git add .`, and then run `git commit -m "what you changed."`.
`git checkout -- <filename>`|grab the version of the repository before the last commit of the specified file.
`git branch -d NewBranch`	  |deletes the specified branch (will not work if not all merges are complete)
`git branch -D NewBranch`  	|forces a deletion of the specified branch (careful not to delete your work)
`gitk`		                  		|launches a gui describing the changes of your project.

#### 3. Pulling changes from a server
Command	               			     |Result
:-----------------------	      |:------------------------------------------------------
`git clone <url or path>`     	|grab the repository and put it in the current directory
`git pull`	                  		|update the repository with the current version (may need certain options to get it to work at first)
`git pull origin`		|pulls from origin, which points to the remote server you are pulling from.
`git pull origin <branch name>`|pulls the specified branch from origin: for instance, `git pull origin master` pulls the master branch.
`git remote add origin <url>`	 |set the url that origin points to.  For instance: your github project url. (needs to be used sometimes when first setting up a project)
`git remote -v`		              |view the details of your remote settings.

#### 4. Pushing changes to a server
Command	                           			|Result
:----------------------------------- 	|:------------------------------------------------------
`git push`                         			|push your committed changes to the server (may require more options to work properly)
`git push origin <branch name>`	      |push your committed changes residing in the specified branch to the remote repository.
`git push <remote-name> <branch-name>`|From [here](http://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes#Pushing-to-Your-Remotes), the first argument of `git-push` is the remote name, followed by the branch name.
`git fetch origin`                  		|fetch information on the remote url that is not synced with your repo


for more help with `git push`, check out [This Link](http://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes)

