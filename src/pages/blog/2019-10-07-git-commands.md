---
templateKey: blog-post
title: GIT commands
date: '2019-10-07 19:08'
featuredpost: true
featuredimage: /img/blog-index.jpg
tags:
  - git
---
**git status** -  which will tell you what branch you're on, whether your Local Repository is different from the Remote and the state of tracked and untracked files

**git add Bob.txt** - You've added the file to the Staging Area, in which you collect all the changes you wish to put into Repository

**git add -all** - add all the files to the staging area

**git reset** - This will unstage all files you might have staged with git add

**git checkout .** - This will revert all local uncommitted changes (be it staged or not staged) (should be executed in repo root)

**git commit** - your commit is added to the Local Repository.

**git commit -m ""** - commit with message

**git push**  -  the changes will be sent to the Remote Repository

**git diff** - If you want to see what has changed in your Working Directory and staging area

**git diff --staged** - to show what changes are staged already 

**git log** - list of all the commits with their hash as well as Author and Date

**git diff {commit}^!** - to compare to the commit one before

**git diff {fileName}** - to see the changes in a file

**git remote show origin** - to see the details of which remote repository the local repository is tracking.
- - -

### BRANCHES

**git branch <branch name>** - adds the new branch to the Local Repository.
While your Working Directory and Staging Area don't really care about branches, you always commit to the branch you are currently on

The remote branch is the upstream branch of your local one.

**git branch** - list of local branches

**git branch -a** - also see the remote branches your Local Repository knows

**git push --set-upstream origin change_alice** : This will create a change_alice branch on the Remote Repository and set our local change_alice to track that new branch.

**git push -u origin {feature_branch_name}** : if you are publishing a local branch for the first time on a remote, the "-u" option is helpful. It makes sure that a tracking connection between the local and the newly created remote branch is established

**git merge change_alice** : Merge the change_alice branch to the master branch (master branch first needs to be checkedout)

- - -

### UPDATING the dev environment

**git fetch** : This gets any changes on the remote as well as branches - into your Local Repository.
Note that at this point, changes aren't integrated into the local branches and thus the Working Directory and Staging Area yet.

**git pull**


**git pull --rebase**


#### Rebase

* When a branch is diverging from the one it's based on and you want to integrate the latest changes back into your current branch, rebase offers a cleaner way of doing that than a merge would.
* Using rebase you can make sure that you frequently integrate the changes other people make and push to master, while keeping a clean linear history that allows you to do a fast-forward merge when it's time to get your work into the shared branch.
  	

**git rebase <branch_name>**
