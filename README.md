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

12. `Difference between git rm and git restore` -->

ans: if you want to move the whole file back to the untracked state,then we do git rm, otherwise if we just want the

changes to be moved in working area or staging area then we go git restore .

13. `git diff commit1 commit2` --> gives the difference of all file changes between two commits

14. ``->if we want to avoid a text editor vim/nano while `git commit` we can use `git commit -m <commit msg>`

15. `git remote ` -->list down all remote connectin names

`Remote Connection` -->it helps you to link two git repos and downloading changes from 

each otherwise


16.`git remote add <name of remote> <link of the remote>` -->: this command helps us to 

add a new link to the remote repo and gives a name to it

17. `git remote rm <name of repo>` --> this command deletes remote cnnection 

18.`git remote rename <old name><new name>` -->: this command renames the remote Connection

19. `git add <file1>,<file2>,<file3>`-->adding multiple files into the staging area.

20. `git add .`-->adding all files to staging area.

21.`git pull <remote name><branch name>`:-->download latest changes from the branch of 

mentioned remote in your local repo

#Recommended practice to do
    -make changes
    -git add<file>
    -git commit
    -git pull
    -git push

merge conficts can occur if multiple people try to make changes to the same file,and
then collaborate




`merge conflicts` are very common while merging
