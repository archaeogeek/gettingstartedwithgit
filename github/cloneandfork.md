# Working with other repositories

The power of GitHub is that you can not only discover lots of fascinating projects, but that you can legitimately download or **clone** them to your local computer, or copy (**fork**) them to your own GitHub repository.

The approach you should take depends on what you intend to do:

* You just want to download it for personal use: clone
* You might want to contribute back changes: fork to your github repository and clone that version

## Cloning a project

When signed in to GitHub click on the **Explore** button on the top menu. Find a project that interests you (hint, click the topics button on the right), and click the green clone button.

*If you're stuck for an idea, then clone [https://github.com/templeman/awesome-ipsum](https://github.com/templeman/awesome-ipsum)*

For now, choose "Clone with HTTPS", and copy the provided URL to your clipboard.

At your command prompt, change to your top level git repositories directory (that we created at the start of [Creating your first local repository](../git/repository.md)). Type the following:

    git clone <the pasted URL>

Hit return, and this will clone your copy of the repository to your local machine, in a folder with the same name as the project. You can now work with your copy of the repository, making changes locally and committing them.

## Forking a project

To create your own copy of a project in your GitHub repository, navigate to one you're interested in and click the "Fork" button in the top right. The number next to the button shows you how many forks there already are.

![Fork](../images/github_fork1.png)

After a few seconds, you will see a new copy of the repository in your GitHub repository. To use this, you should clone it to your local computer, as above.

To work on this, you should follow the instructions in the previous page to add your new repository as a **remote** for your local copy, make changes and **commit** locally, before **pushing** to the remote.