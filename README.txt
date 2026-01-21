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
