## What is a Git Repo?
Workspace which tracks and manages files within a folder. 

==git status== 
Gives information on the current status of a git repository and its contents.

==git init== 
Create a new git repository

==git status==
_ON BRANCH MASTER_

<mark style="background: #FF5582A6;">WARNING</mark> 
DO NOT INIT A REPO INSIDE OF A REPO
==before running git init use git status==

In case you do:
==ls -a==
==rm -rf .git==

## Committing
Checkpoint = commit
Changes that you want to include.

1. ==git add _filename_== OR ==git add .==
2. ==git commit -m "my message"

<mark style="background: #BBFABBA6;">WORKING TREE CLEAN</mark> = Up to date.
_______________________________________________________________

## ==git log==
Retrieves a log of the commits.
1. See author
2. See email
3. See date
4. See commit message

_________________________________________________

## COMMITS IN DETAIL

### Git Docs
https://git-scm.com/docs

### Atomic Commits
A commit should encompass a single feature, change or fix.
This makes it much easier to undo or rollback.

### Writing Commit Messages
What matters is consistency.

______________________

==We need the hashes shown in _git log_ to go back==

1. git log --abbrev-commit
2. git log --oneline 
	1. _One line of each commit message._


## Amending Commits
==--amend== 
Fix mistakes just 1 commit ago.

Example:
```
git commit -m "My commit"
git add forgotten_file.txt
git commit --amend
```

### Ignoring Files
Using<mark style="background: #BBFABBA6;"> .gitignore</mark> file you can tell Git which files and directories to ignore in a given repository.
1. Secrets, API keys.
2. Operating System files.
3. Log files
4. Dependencies & Packages.

