1. git init -> powers your folder to be managed by git, and initialises a new empty repository. It also create a .git folder that has all the relvant logic to manage versions of your project.

2. Working Area -> there can a bunch of files that are not handled by git.
It means that changes done or to be done in those files are not managed by git yet. A file which is in working area is consider to be not in the staging area. When we do 'git status' and we see a bunch if 'untracked files' then these are actually called to eb in the working area.

3.'Staging area' -> what all files are going to be part of the next version that we will create.
This staging area is the place where git knows what changes will be done from last version to current(next) version.


4.'Repository Area' -> This area actually contains the details of all you pervious registered version .
And the files in this area , git already manages then and knows their version history.


5. 'git add <file>' -> this move the file from working area to staging area

6. 'git rm --cached <file>' --> moves file back from staging area to working area.


7. 'commit' -> Commit is a particular version of your project.
It captures a snapshot of the project's staged changes and create a version out of it.

8.'git commit' -> registers staging changes to a commit


9. 'git log'-> list down the all the possible commit. If want exit from git log press q

10. 'git restore <file>' -> it removes all files chnages from the staging area to be committed .This can be useful, if we did some dirty piece of code and now no more wanted ,instead of deleting every change line by line , we can restore it
or restore last version

11.'git restore --staged <file>'-> it remove file from staging area to the working area.this only works if changes are in your staging area

12. Diff between git rm and git restore
ans: if you want to move the whole file back to the untracked state,then we do git rm,otherwise if we just want the changes to be moved in working area

8b51fb62352612d965674c97c05254f429e6426f
71b5230323262808b68bd124628a7b86d54c97b2

13. 'git diff commit1 commit2' -> gives the difference of all files changes between two commits

14. 'git commit -m"your message"'-> if you dont want to open vim editor follow this command

15. 'git remote' -> list down all the remote connection names

16. Remote connection ->It help you to link two git repository for uploading and downloading changes from each otherwise

17. 'git remote add <name of remote connection> <link of remote connection>' -> this command helps us to add a new link to the remote repo and give a name to it


18.'git remote rm <name of remote>' -> this command deletes remote connection


19.'git remote rename <oldname> <newname>' -> this command rename the remote connection

note: the name of the remote connection is always used to establish communication between the repo

20.`git add <file1> <file2> ..` -> this command will add multiple file changes together in the staging area

21.`git add .` -> this command add all file in the staging area



22.`git pull <remote name > <branch name>`-> downloads latest changes from the branch of the mentioned remote in your local repo