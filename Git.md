# Git Basics

## Basic Commands

### Initiating a repository

If you have a project directory that is currently not under version control and you want to start controlling it with Git, you first need to go to that project’s directory. If you’ve never done this, it looks a little different depending on which system you’re running:

` git init ` 

For example: 

` mkdir kntu-react-native-class`

` cd kntu-react-native-class `

` git init `

### Clone a repository

You clone a repository with:

` git clone <url> `

For example, if you want to clone the Git linkable library called libgit2, you can do so like this:

` git clone https://github.com/libgit2/libgit2 `

### Tracking new files

In order to begin tracking a new file, you use the command git add.

` git add [file_name] `

For example: 

` git add README.md `

### Checking the status of your files

The main tool you use to determine which files are in which state is the git status command. If you run this command directly after a clone, you should see something like this:

` git status `

To see what you’ve changed but not yet staged, type git diff with no other arguments:

` git diff `

### Commiting your changes

The simplest way to commit is to type:

` git commit `

Doing so launches your editor of choice. 

Alternatively, you can type your commit message inline with the ` commit command ` by specifying it after ` a -m ` flag, like this:

` git commit -m 'Initial Commit' `

### Removing files

To remove a file from Git, you have to remove it from your tracked files (more accurately, remove it from your staging area) and then commit. The git rm command does that, and also removes the file from your working directory so you don’t see it as an untracked file the next time around.

` git rm [filename] ` 

### Moving files

If you want to rename a file in Git, you can run something like:

` git mv file_from file_to `

### Viewing the commit history

After you have created several commits, or if you have cloned a repository with an existing commit history, you’ll probably want to look back to see what has happened. The most basic and powerful tool to do this is the following command.

` git log `

## Copyright

All contents adapted from [Scott Chacon. “Pro Git.” iBooks. ] (https://git-scm.com/book/en/v2)