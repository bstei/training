# git cheat sheet

Read your group instruction in the text files 

[group1.md](group1.md)

[group2.md](group2.md)

[group3.md](group3.md)

[group4.md](group4.md)

and place your solution in a fitting category in this file.

## Creating repositories

    git init                    it initiales a local repo

    git clone https://...       copies the whole repo with all branches to local

## Staging and committing

    git add .                   Add all changes but new files and deletions

    git add -u                  Removes as well as modifies index entries to match the working tree, but adds no new files.
    git add -A                  Same like above but also adds new files.

    git add test.txt            Add the test.txt file to the stage

    git reset HEAD test.txt     Resets test.txt to thes state of HEAD, means unstage already staged changes

    git diff --staged           Show diff of already staged changes to HEAD

    git commit                  Starts committing and opens a text editor for putting in the message

    git commit -a               also adds changes from all known files (skips add)

    git commit -m "Add smthg"   Commit with the commit message "Add something"

## Inspecting the repository and history

    $ git cat-file -p a3798b    Command reads content of the file beggining with a3798b with pretty option
    git status
    git log

## Managing branches

    $ git checkout work         Command switches to a branch named work.
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

    git checkout -b feature
create branch feature1

git branch
show all branches

    git branch -a
show all branches, also remotes

## Merging

    $ git merge work	        Command merges work branch into the current branch
    $ git merge --abort         Command canceles the merge if in conflict state 

    git merge feature1
merge branch feature1 into current branch