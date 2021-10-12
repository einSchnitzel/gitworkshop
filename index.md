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

## Git diff
### Displays the differences between last commit and current version
### Differences may be displayed using  the branches in vscode as well
### You can exit using q
	git diff

