# Creating your first local repository

Folders and files are not version-controlled until we explicitly ask them to be. This process is called **initialising a repository**.

Firstly we need to create a folder to hold our files. We do this at the command prompt using the following syntax (referring back to [here](../intro/introcli.md) if necessary):

## Linux or Mac

	mkdir -p gitrepositories/gettingstartedwithgit

## Windows

    mkdir gitrepositories/gettingstartedwithgit

**Where is this?**

If you don't specify a location for this folder, then it will use a default location as follows:

|OS | Location |
|---|----------|
|Windows using Git Bash | C:\Users\yourname |
|Windows using GitHub Desktop | C:\Users\yourname\Documents\GitHub |
|Linux | /home/yourname |
|Mac using Git from XCode | /Users/yourname |
|Mac using GitHub Desktop | /Users/yourname/Documents |


Now change directory to `gettingstartedwithgit`:

	cd gitrepositories/gettingstartedwithgit

Initialise it as a repository:

	git init

This might not appear to do anything but it creates a hidden folder called `.git` inside `gettingstartedwithgit` that contains the information Git needs to track your repository.

**On windows, change your folder preferences to "always view hidden folders" so you can see this folder**

That's all we can do until we start adding some files and making changes to them, so let's make a file:

## Mac and Linux

	touch blah.txt

## Windows

    type nul > blah.txt

This creates a blank text file called "blah.txt" in the folder.

At this point, we have enough in place to start committing to our repository.


