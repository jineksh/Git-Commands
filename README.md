1. 'git init' -> Powers your folder to be managed by git,and intialise a new empty repository .it also create a .git folder that has all the relevent logic to manage versions of your projects.

2. Working area -> there can be a bunch of files that are not currently handled by git .it means that changes done or to br done in these files are not manages by git yet. A file which is in working area is considered to be not in the staging area .when we do 'git status' and we see abunch if 'untracked files 'then these are actually called to be in the working area.

3. staged area ->  what all files are going to br part of next version that we will create.This stage area is the place where git knows what changes will be done from last version to the new version. for this use 'git add <file name>'

4. repository area -> this area actullay contains the details of all you previous registered version. and the files in this area . git already manages then and knows their version history.

'git add <files>' -> moves file workig area to staging area.

'git rm --cached <files>' -> moves file back from staging area to wrokig area.

'commit' -> commit is a particular version of the project .it capatures the sanpshot of the project's staged changes and creates a version out of it.

'git log' -> list down all commits.if you want to exit from git log just press q.

'git restore <file>' -> it removes all files changes from the staging area to commited. This can be useful. if we did some dirty code and how no more want. we can restore last clean version of the file.

whenever your file is commited and you can change in file or write new code on it so writed new code is now in working area and if you don't need of new code then you use it 'git restore'.

once your file in staging area and now you don't need last change so you can use 'git restore --staged <file>' this will help you to move your last change from staging area to working area and now you can remove with 'git restore'.

Quetions-> diff between rm and restore;
ans-> if you move whole file back to untracked stage than you use "git rm --cached".and if not whole file and some part of file than you use restore.

'git diff commit1 commit2' -> give the diff between what changes in commit1 and commit2. 

remote connections -> It helps you to link two git repositories for uploading and downloading changes from each other.

'git remote add <name of remote> <link>' -> it will link your local repository to online github repository.

'git remote rm <name of remote>'-> this command deletes a remote connections.

'git remote rename <oldname> <newname>'  -> this command rename the remote connection .

'git pull <name of remote> <branchname>' -> download latest changes from the branch of the mentioned remote in your local repository.

### recommended practice for working to do 
-make change
-git add
-git commit
-git pull
-git push