git init -> Create empty Git repo in specified directory. Run with no 
           arguments to initialize the current directory as a git repository.


working area = There are bunch of files that are not currently handeled by git.
It means changes done or not to be done in those files are not managed by git.A file which is
not in working area is consider to be in staging area.when we do `git status` and we see bunch 
of `untracked files` then these are actually called to be in working area.

Staging area - What all files are going to be part of next version that we will create.the 
staging area inthe place where git kows what changes will be done from the last version 
to the next version. 

Repository area - This area actually contain the details of all your previous register version.
And the file in this area , git already manages them and manages therir version history.

`git add <file>` move file from working area to staging area

`git rm --cached <file>` -> move files back from staging area to working area.

`commit' - Commit is the particualr version of the project.It captures a snapshot of the project's staged
changes and creat a version out of it.

`git commit` - registering staging changes to commit

`git log` - list down all the commits of the repository.

`git restore <file>` - it remove all the file changes from stating area to be commited.this can be useful
,if we did some dirty piece of code and now no more want it.Instead of deleting every changes line by
line ,we can restore it or you can say restore last clean version of file.

`git restore --stagged <file>` - it removes files from changes from staging area to the working area.
This only work when changes in your staging area.

Diff between git rm and git restore.
-if you want to move the whole file back to the untracked state then we do git rm,otherwise 
if we just want to changes to be moved in woorking area and staging area tehn we do git restore.


`git diff commit1 commit2` - give the difference of all file changes between two commits.


`git commit -m "<your commit message>"` - if you don't want to open any vim/nano operator to
type the commit meggage.

`git remote` -> list down all the remote connection names.

Remote Connection -> It helps you to link two git repository for uploading and 
downloading changes from each other.


`git remote add <name of remote> <link of the remote>` : this command helps us to add a new link to the 
remote repo and name to it.

`git remote rm <name of remote>` :  this command delete the remote connection.

`git add .` : add all the file to working area to staging area.


`git remote rename <olname> <newname>` : this command rename the new connection


`git pull <remote name> <branch name>` :downlaod latest changes from the branch of the mentioned remote
to your local repo 

