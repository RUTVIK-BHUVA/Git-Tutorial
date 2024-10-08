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

git commit -m <your commit message>
`git remote` --> List down all the remote connection names
Remote connection --> It helps you to link two git repositoroes for uploading and downloading changes from each otherwise
`git remote add <name of remote> <link of the remote>` --> This command helps us to add a new link to the remote repo and give a name to it
`git remote rm <name of remote>` --> This command deletes a remote connection
`git remote rename <oldname> <newname>` --> This command renames the remote connection

Note : The name of the remote connection is always used to establish communication between the repos


20. `git add <file1> <file2> <file3>` --> this command will add multiple file changes together in the staging area

21. `git add .` --> This command will add all files from working repo to the staging area.

22. `git pull <remote name> <branch name>` --> Downloads latest changes from the branch of the mentioned remote in your local repo


### Recommanded practice to do 

    - make changes 
    - git add <file>
    - git commit
    - git pull
    - git push
