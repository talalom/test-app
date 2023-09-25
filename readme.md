# Instructions for Git

* git clone url.com // to clone the repo
* cd into the folder you've cloned
* git status // to see the folder's status
* git add readme.md
* git status
* git commit -m "Readme file updated" // because we cloned the repo, we don't need the origin, but it is a needed step if you don't clone
* git push -u origin main
## Extra Comments

* git add can have multiple endings:
	* git add readme.md
		* This will add a single file to the staging area
	* git add readme.md index ts
		* this will add two files to the staging area
	* git add .
		* this will add all changes to the staging area
	* git add *
		* this will add all changes in the current directory but not the sub directory
	* git add -all OR git add -A
		* this will add all hidden files but try not to add hidden files. They are often hidden for a reason. .gitignore is an exception

# VS Demonstrations
* using the git changes window, we can use a gui instead of a command line
* if you don't see the git changes, click view and git changes

# Version Numbers of Applications

* 1.0.0
* The far right 0.0.1 <- Is a minor change to the application
	* 0.0.2 is a minor change from 0.0.1
* The middle number 0.1.0 <- is a bigger change but not a drastic move
* The left number 2.0.0 <- is a major change, like visual changes, overhaul, or a lot of features

## Branching

* We can use branching to allow engineers to try different solutions without causing issues on the main codebase
```
git branch example
git checkout example
```
* to merge with main, we need to do:
```
git checkout main
git pull origin main
git merge example
git push origin main
```