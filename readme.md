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

$ git cat-file -p a3798b    Command reads content of the file beggining with a3798b with pretty option

## Managing branches

$ git checkout work         Command switches to a branch named work.
$ git checkout master	    Command switches to a master branch. 

## Merging

$ git merge work	        Command merges work branch into the current branch
$ git merge --abort         Command canceles the merge if in conflict state 