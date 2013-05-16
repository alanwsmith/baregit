baregit
=======

A simple script for creating git repos in a primary, local storage location. When created a master branch is created with initial `.gitattributes`, `.gitignore` and `readme.md` files. 

Setup for execution
-------------------

Option 1: Drop a copy of baregit in a directory that's on your path (e.g. `/usr/local/bin`) and chmod it for execution (e.g. `sudo chmod u+x /usr/local/bin/baregit`).

Option 2: Clone the repo any location on your machine and create a symbolic link to the script from a location that's on your path. For example, if the repo is cloned to a `~/scripts` direcotry and a `/usr/local/bin` direcotry is on your path, the link command would be:

	sudo ln -s /usr/local/bin/baregit ~/scripts/baregit/baregit
	or
	ln -s /usr/local/bin/baregit ~/scripts/baregit/baregit
	if you don't need sudo

Option 3: Any other way you want to make the script executable and have it on your PATH. 


Usage
-----

Just do:

    baregit repo-name

This will make a new git repository in the current directory. As part of the process, the repo is checked out to a tmp repo where a basic set of files are created, added and committed back. With this setup, the repo can be cloned immediately and the master branch will exist and be ready to go. 


