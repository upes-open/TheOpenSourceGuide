# Git Basics
[![Pictures-from-ProGit](https://img.shields.io/badge/Pictures%20from-ProGit-yellow.svg)](https://git-scm.com/book/en/v2)

You can do two things here either you can clone an repo from github if you have accoutn or you can 

## Initializing a Repository in an Existing Directory
Open terminal at the place where you have your project or where you will liketo save your project from github, if already exist.
```
git init
```
Adding files 
```
git add
```
## Cloning an Existing Repository
If you have project in GitHub then you need to clone it into your local repo.
```
 git clone https://github.com/upes-open/TheOpenSourceGuide
 ```
 ## Recording Changes to the Repository
 
 <img src="https://github.com/Nehasingh1300/TheOpenSourceGuide/blob/master/Module%202/resources/recodingchanges.PNG" >
Your all changes to your repo are being staged which have been committed. Remember that each file in your working directory can be in one of two states: tracked or untracked. Tracked files are files that were in the last snapshot; they can be unmodified, modified, or staged. Untracked files are everything else – any files in your working directory that were not in your last snapshot and are not in your staging area.

## Checking the Status of Your Files
Checking if your files are staged or not tracked or untracked, you will use
```
git status
```
If in result you get this: this means you have committed everything and there is nothing left to commit.
```
On branch master
Your branch is up-to-date with 'origin/master'.
nothing to commit, working directory clean
 ```
 Else if you get this : this means that  README file has not been added and it will also suggest you to add it
 ```
 On branch master
Your branch is up-to-date with 'origin/master'.
Untracked files:
 (use "git add <file>..." to include in what will be committed)
 README
nothing added to commit but untracked files present (use "git add" to track)
```
### Tracking New Files
Adding new files is same as making them tracked but not staged, staging is done after commit.
```
 git add README
 ```
### Staging Modified Files
If after committing you again add a file then you will get this, which means that you have to add the file and also commit it again
```
 git status
On branch master
Your branch is up-to-date with 'origin/master'.
Changes to be committed:
 (use "git reset HEAD <file>..." to unstage)
 new file: README
Changes not staged for commit:
 (use "git add <file>..." to update what will be committed)
 (use "git checkout -- <file>..." to discard changes in working directory)
 modified: CONTRIBUTING.md
```

### Ignoring Files
There can be some files which you will not like to push to remote repo for that you can add all those files in this file
```
vim .gitignore
```
### Viewing Your Staged and Unstaged Changes
To see what you have staged and what not, you can run
```
 git diff
diff --git a/CONTRIBUTING.md b/CONTRIBUTING.md
index 8ebb991..643e24f 100644
--- a/CONTRIBUTING.md
+++ b/CONTRIBUTING.md
@@ -65,7 +65,8 @@ branch directly, things can get messy.
 Please include a nice description of your changes when you submit your PR;
 if we have to read the whole diff to figure out why you're contributing
 in the first place, you're less likely to get feedback and have your change
-merged in.
+merged in. Also, split your changes into comprehensive chunks if your patch is
+longer than a dozen lines.
 If you are starting to work on a particular area, feel free to submit a PR
 that highlights your work in progress (and note in the PR title that it's
 ```
 
 ## Committing Your Changes
Your changes are in staging area now but not staged for that run this command here you -m signifies messsage for you r commit as no commit can be done without message
```
git commit -m "Initial Commit"
```
### Skipping the Staging Area
If you want to skip staging are and direclty commit, you can use :
```
 git commit -a -m 'added new benchmarks'
[master 83e38c7] added new benchmarks
 1 file changed, 5 insertions(+), 0 deletions(-)
 ```
 ### Removing Files
To remove any file which do not use or is wrongly placed:
```
git rm README.md
```
### Moving Files
To move files from one plce to another
```
git mv file_path_from file_path_to
```
## Viewing the Commit History
Everything you do in git is recorded with help of SHA-1(dicussed in chapter 1). You can check logs to get this.<br>
You can check logs generated or you can also tree based logs generarted.
```
 git log
commit ca82a6dff817ec66f44342007202690a93763949
Author: Scott Chacon <schacon@gee-mail.com>
Date: Mon Mar 17 21:52:11 2008 -0700
 changed the version number
commit 085bb3bcb608e1e8451d4b2432f8ecbe6306e7e7
Author: Scott Chacon <schacon@gee-mail.com>
Date: Sat Mar 15 16:40:33 2008 -0700
 removed unnecessary test
commit a11bef06a3f659402fe7563abf99ad00de2209e6
Author: Scott Chacon <schacon@gee-mail.com>
Date: Sat Mar 15 10:31:28 2008 -0700
 first commit
 ```
 ## Undoing Things
Be careful in this blog, because undoing thing can never be reverted. If you want to go back to commit or undo something.<br>
It undoes the last commit you made and hencec you go one commit back.
```
 git commit --amend
```
 ### Unstaging a Staged File
It unstages the file 
```
git reset HEAD CONTRIBUTING.md
```
### Unmodifying a Modified File
It’s important to understand that git checkout -- <file> is a dangerous command. Any changes you made to that file are gone – Git just copied another file over it. 
```
 git checkout -- CONTRIBUTING.md
 ```
 
 ## Working with Remotes
 To be able to work with everyone you have to have something on remote which is accessible by everyone, so other than one repository/folder in you rlocal computer there is one in remote.
 ## Showing Your Remotes
To check how many remote you have in your repo (Al the remotes)
```
git remote
origin
```
To get all the URLs
```
git remote -v
origin https://github.com/upes-open/TheOpenSourceGuide (fetch)
origin https://github.com/upes-open/TheOpenSourceGuide (push)
```
### Adding Remote Repositories
Addingg remote to your repo so that you can connect local repo and remote repo
```
 git remote
origin
$ git remote add pb https://github.com/paulboone/ticgit
$ git remote -v
origin https://github.com/upes-open/TheOpenSourceGuide  (fetch)
origin https://github.com/upes-open/TheOpenSourceGuide (push)
```
### Fetch 
To get information from remote to your local repo with your remote name
```
 git fetch [remote-name]
```
### Pushing to Your Remotes
When you have your project at a point that you want to share, you have to push it upstream. The command for this is simple: git push [remote-name] [branch-name].
```
$ git push origin master
```
### Removing and Renaming Remotes
Renaming : Itn shows renamed origin
```
 git remote rename origin origin1
$ git remote
origin1
```
Removing : It does not show any remote as we deleted on that exists
```
 git remote rm 
$ git remote

```
