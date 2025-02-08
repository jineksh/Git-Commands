1. 'git init' -> Powers your folder to be managed by git,and intialise a new empty repository .it also create a .git folder that has all the relevent logic to manage versions of your projects.

2. Working area -> there can be a bunch of files that are not currently handled by git .it means that changes done or to br done in these files are not manages by git yet. A file which is in working area is considered to be not in the staging area .when we do 'git status' and we see abunch if 'untracked files 'then these are actually called to be in the working area.

3. staged area ->  what all files are going to br part of next version that we will create.This stage area is the place where git knows what changes will be done from last version to the new version. for this use 'git add <file name>'

4. repository area -> this area actullay contains the details of all you previous registered version. and the files in this area . git already manages then and knows their version history.

'git add <files>' -> moves file workig area to staging area.

'git rm --cached <files>' -> moves file back from staging area to wrokig area.

'commit' -> commit is a particular version of the project .it capatures the sanpshot of the project's staged changes and creates a version out of it.