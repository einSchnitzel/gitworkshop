# Git workshop 

## Initialise repository

	git init

## Place identities globally

	git config --global user.name "name"
	git config --global user.email "email@something.com"

### Use local instead of global if it should be with this folder only
	
	git config --local user.name "name"
	git config --local user.email "email@something.com"

## Add file
### All in folder
	git add *
###	One file
	git add <filename>

## Remove added file

	git rm --cached <filename>

## Commit a new version
	git commit -m "added filename"

## Git status and log
### Check what is added and commited
	git stauts

### Check the log and history
	git log
	git log <filename>

### See who made which edits
	git blame <filename>

## Git diff
### Displays the differences between last commit and current version
### Differences may be displayed using  the branches in vscode as well
### You can exit using q
	git diff

## Create a new branch
	git branch main
### List all branches
	git branch

## Switch branch to another branch
### everything is now on main as well
	git checkout main

## Checkout to a previous branch
### sometimes there may be issues when returning due to changes, conflicts need to be sorted then

## Connect remote repositories to github via ssh
### Origin is just a name
	git remote add origin git@github.com:something/path.git
	git branch -M main
	git push -u origin main

## Renaming remote repositories

	git remote rename currentname newname

## List remote directories
	git remote -v

## Change  remote URL to ssh 
git remote set-url origin git@github.com:something/path.git
## Change  remote URL to htmls
git remote set-url origin https://github.com/something/path.git

## It is possible to push to 2 remotes within one repo