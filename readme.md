# git cheat sheet

Read your group instruction in the text files 

[group1.md](group1.md)

[group2.md](group2.md)

[group3.md](group3.md)

[group4.md](group4.md)

and place your solution in a fitting category in this file.

## Creating repositories

... put commands and explanation here

## Staging and committing

... put commands and explanation here

## Inspecting the repository and history

... put commands and explanation here

## Managing branches

    $ git checkout master       Switch to commit that master points to
    $ git branch feature1       Create a branch named "feature1"
    $ git checkout -b work      Switch to newly created branch "work"
    $ git checkout work         Switch to existing branch "work"
    $ git branch                List of existing branches, highlights current branch
    $ git branch -v             List of existing branches with reference to latest commit
    $ git branch -a             List of all existing branches, both local and remote
    $ git branch --merged       List branches, that where merged into the current named branch
    $ git branch --no-merged    List branches, that were not merged into the current named branch
    $ git branch -d work        Delete branch "work", stop when something is open/pending/not merged
    $ git branch -D work        Delete branch "work", hard delete also when something is still open

## Merging

.. put commands and examples here