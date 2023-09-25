# Instructions for Git

* git clone url.com // to clone the repo
* cd into the folder you've cloned
* git status // to see the folder's status
* git add readme.md
* git status
* git commit -m "Readme file updated" // because we cloned the repo, we don't need the origin, but it is a needed step if you don't clone
* git push -u origin main
* 
## Extra Comments

* git add cna have multiple endings:
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