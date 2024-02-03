1. `git init` -->powers your folder to managed by git ,and initialized a new empty

repo.it also creats a .git folder that has all the relevant logic to manage versions

of your project.

2.  `Working Area` --> There can be a bunch of files that are not currently handled 

by git.It means changes done or to be done in those files are not managed by git yet.

A file which is in working area is considered to be not in the staging area.

When we do `git status` and we see a bunch of `untracked files` then these are actually 

called to be in the working area.

3. `Staging Area` --> what all files are going to be part of next version .

This staging area is the place where git knows what changes will be done from last version 

to the next version.

4.  `Repository Area` -->This area actually contains the detail of all your previous registered versions.

and the files in this area ,git already manages them and knows their version history.

5. `git add <file>`--> Moves file from working area to staging area 

6. `git rm --cached <file>` --> Moves file back from staging area to working area 

7. `commit` --> commit is a particular version of the project . it captures a snapshot of the project's

staged changes and creates a version out of it.

8. `git commit` --> registers staging changes to a commit

9. `git log` --> list down all commits of the repository .if you want to exit out of git log prompt press 'q'

10. `git restore <file>` --> it removes all files changes from staging area to be commited .This can be useful 

if we did some dirty piece of code and now no more want it .Instead of deleting every change line by line 

we can restore it or you can say restore last clean version of the file.

11. `git restore --staged <file>`  --> it remove file changes from staging area to working area.this only 
works if changes are in your staging area.

12. `