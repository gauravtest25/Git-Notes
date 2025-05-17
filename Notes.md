Git is a version control system.
Version control system is the tool that helps you to track changes in the code .
Commands
Git clone & Git status

// Clone a repo git clone YourGitlink

// Getting status code git status

Git status components

Untracked : new files that git doesn't track\
modified : changed file
staged : file is ready to be committed -- After we add the file the status become staged
unmodified : unchanged -- When we commit the file the status become unchanged
Add & Commit

add - adds new or changed files in your working directory to the git staging area.

git add fileName
// Another command to add all the files

git add .
commit - it is the record of the change

git commit -m "some message"
push - To push your changes to your git

git push origin main
// What if don't want to mention the branch name and origin again and again and we want to specify that we will work in same branch only

git push -u origin main
//After using this command you don't to write the command origin main again and again  and things will work with 'git push'
Remote Commands
If we are already having so many files in our local. And we want certain folder to be a repo we will initialize empty git repo init.
Commands

git init used to create the new git repo or we can say to initialize git in that folder we use this command.

git remote add origin repoLink - Connecting our remote repo to our local folder.

git remote -v : to verity remote

Branch Commands
git branch : to check the branch

git branch -M <NameThatYouWant> : to rename the branch

git checkout <branchName> : To navigate

git checkout -b <newBranchName> : to create new branch

git branch -d <branchName> : to delete the branch\

//Note :- If you want to delete certain branch then first you need to move to another branch then only you will be able to delete the branch

git diff <branchName> : to compare commits , branches, files & more

git merge <branchName> : to merge 2 branches

Pull Request
It let's you tell others about changes you've pushed to a branch in a repository on github

Pull command
To brings the changes you have done to your remote now have to show in local then you will use pull commands.

It basically fetch and download content from the remote repo.
git pull origin main

Resolving merge conflicts
An event that takes place when git is unable to automatically resolve differences in code between two commits.

Undoing Changes
case :1 Staged Changes

git reset filename - to reset changes in particular fil

git reset - to reset changes in all the files

case : 2 Committed Changes (for one commit)

// To reset the change that is last commited git reset HEAD~1

// command to check all the commits git log

case : 3 committed Changes (for many commits) // Note : You can take the hash or the commit using git log

//'To reset the particular commit using their hash git reset <-commit hash>

// To reset the particular commit and the commit's that are done after it. git reset --hard <-commit hash->

Fork
A fork is a new repository that shares code and visibility settings with the original "upstream" repository. Fork is a rough copy.