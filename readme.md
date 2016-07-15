# git cheat sheet

Read your group instruction in the text files 

[group1.md](group1.md)

[group2.md](group2.md)

[group3.md](group3.md)

[group4.md](group4.md)

and place your solution in a fitting category in this file.

## Creating repositories

git init
it initiales a local repo

## Staging and committing

    git add .
add all files (but new ones?)

    git commit -m "Add something"
commit with the commit message "Add something"

## Inspecting the repository and history

$ git cat-file -p a3798b    Command reads content of the file beggining with a3798b with pretty option
    git status
    git log

## Managing branches

$ git checkout work         Command switches to a branch named work.
$ git checkout master	    Command switches to a master branch. 
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