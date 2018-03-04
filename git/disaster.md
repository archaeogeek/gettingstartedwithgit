# Recovering from disaster

Git provides a number of ways of recovering from disaster, aka undoing changes to your repository. We won't go into too much detail here as it's all rather more complicated than we have time for!

In all cases, you will need to know the SHA ID for the a commit, found by running the `git log` command. You can get a shorter (7 character) version of the SHA, which is equally valid, by appending `--abbrev-commit` to the command, as follows:

    git log --abbrev-commit

## git checkout

This allows you to **view** the repository at a particular point in time, or commit:

    git checkout <sha>

It does not replace your current working state, you can get back to that with:

    git checkout <branchname>

To continue working on the repository from the position of the commit you have gone back to:

    git checkout <sha>
    git checkout -b newbranchname

**At this point, in this branch, the subsequent work no longer exists**

## git clean

This allows you to "tidy" a repository by deleting untracked files. To see what it will do before it actually does it, add the `-n` option, which performs a dry-run:

    git clean -n

*Note that `-n` can be used after most git commands to give you a dry-run of what the command will actually do*

## git revert

This allows you to undo changes to your commit history by adding a new commit, which is equivalent to the "inverse" of the one referred to in the command:

    git revert <sha>

## git reset

This undoes changes to your commit history but also modifies the file system and staging index, depending on the way git reset is invoked.

| Command | Operation |
|---------|-----------|
| git reset --soft &lt;sha&gt; | The contents of the staging index and file system are unchanged |
| git reset --mixed &lt;sha&gt; | Resets the staging index but leaving the working directory unchanged |
| git reset --hard &lt;sha&gt; | Resets the staging index and the working directory back to the state of the specified commit |

Of these options `git reset --hard <sha>` is the most dangerous and commonly used invokation. It is most commonly used to return everything (commit history, staging index and file system) back to the state it was in before the most recent commit, with:

    git reset --hard HEAD^





