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
    
    $ git log shows the commits of the current branch
    $ git log --oneline shows all commits but only one line commit info
    $ git log --oneline --all shows the history of all files including all branches, but only with one line commit info
    $ git log --oneline --all --graph graph that shows the branches and shows the branch and merge history
    $ git log --oneline --all --graph --decorate shows the branch and merge history, and puts more colors in there and gives the names to the branch
    $ git log --follow -p -- filename shows the history of the file 
    $ git log -S'static void Main' searches for the "static void main" string
    $ git log --pretty=format:"%h - %an, %ar : %s" allows you to specify your own log format (commit hash, author name, author date, subject)

## Managing branches

... put commands and explanation here

## Merging

.. put commands and examples here

    $ git diff shows changes of the file and opens kdiff 
    $ git diff --staged shows difference of staged files
    $ git diff test.txt shows difference in this file and between two commits
    $ git diff --theirs shows theirs version and shows difference
    $ git diff --ours shows what you had in your branch before commit and merge
    