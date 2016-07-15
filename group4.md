Exercise:

Explain the following commands with one sentence:

    $ git checkout work
    $ git checkout master
    $ git merge work
    $ git merge --abort
    $ git cat-file -p a3798b

Example:

    $ git status         Shows the current state of the repository


Here are some standard situations, and a git command. Draw the result, and add some explanation:

Example 1:

    A - B (master)
         \
          C (work)
    
    $ git checkout master
    $ git merge work

Result and explanation here:
    A - B - C (HEAD -> master, work)


Example 2:

    A - B - C - D (master)
         \
          X - Y (work)
    
    $ git checkout master
    $ git merge work

Result and explanation here:
    A - B - C - D - E (HEAD -> master)
         \        /
          X - Y (work)


Example 3:

    A - B - C - D (master)
         \
          X - Y (work)
    
    $ git checkout work
    $ git merge master
    $ git checkout master
    $ git merge work

Result and explanation here:
    A - B - C - D
         \       \
          X - Y - E (HEAD -> master, work)

Add you answers to the file readme.md!