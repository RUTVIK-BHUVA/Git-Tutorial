`git init` --> Powers your folder to be managed by git, and initialises a new empty repository. It also creates a .git folder that has all the relevant logic to manage versions of your project.
`Working area` --> There can be a bunch of files that are not currently  handled by git. It means that changes done or to be done in those files are not managed by git yet. A file which is in working area is considered to be not in the staging area. When we do `git status` and we see a bunch of `untracked files` then these are actually called to be in the working area.
`Staging area` --> What all files are going to be part of the next version that we will create. This staging area is the place where git knows what changes will be done from the last version to the next version.
`Reposetory area` --> This area actually contains the details of all your previous registered version and the files in this area git already manages then and knows their version history.
`git add <file>` --> Moves file from working area to staging area.
`git rm --cached <file>` --> Moves file back from staging area to working area.
`commit` --> Commit is a particular version of the project. It captures a snapshot of the project's staged changes and creates a version out of it.
`git commit` --> Registers staging changes to a commit.
`git log` --> List down all the commits of the repository. If you want to exit out of git log prompt press `q`.
`git restore <file>` --> It removes all files changes from the staging area to be committed. This can be useful, If we did some dirty piece of code and now no more want it. Instead of deleting every change line by line, we can restore it or you can say restore last clean version of the file.

`git restore --staged <file>` --> It removes file changes from staging area to working area.

Difference between git rm and git restore 
ans : if you want to move the whole file back to the untracked state, then we do git rm, otherwise if we just want the changes to be moved in working area and staging area then we do git restore
`git diff commit1 commit2` --> gives the difference of all file changes between two commits
`` --> If we want to avoid opening a text editor like vim/nano to add commit message we can use this following command
