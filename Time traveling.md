## Checkout
We can use it to create branches, switch to branches, restore files and undo history.

<mark style="background: #ADCCFFA6;">git checkout #commit <commit-hash></mark>
Is used to view  previous commit.
Travel back to a commit.

* _We need to use the hash of a commit with ==git log==_ 


_HEAD is a pointer to the current branch reference._
<mark style="background: #FF5582A6;">HEAD USUALLY REFERS TO A BRANCH NOT A SPECIFIC COMMIT</mark> 

==Detached HEAD==
Options:
1. Stay in detached HEAD to examine the contents of the old commit. <mark style="background: #ADCCFFA6;">git checkout master</mark> <mark style="background: #BBFABBA6;">OBSERVER</mark> 
3. Leave and go back, __reattach__ the HEAD. <mark style="background: #ADCCFFA6;">git checkout master</mark> 
4. Create a new branch and switch to it. Make and save changes. HEAD is no longer detached. <mark style="background: #BBFABBA6;">git checkout #commit, git switch -c redo, </mark> 


<mark style="background: #ADCCFFA6;">git checkout HEAD~1</mark> 
HEAD~1 refers to the commit before HEAD
HEAD~2 refers to 2 commits before HEAD


## Discarding Changes
To revert a file back to whatever when you last committed:
<mark style="background: #ADCCFFA6;">git checkout HEAD filename</mark> 

![[Pasted image 20220722125007.png]]

==File is updated to the last commit, changes are deleted.==

## Unmodifying file with restore
<mark style="background: #ADCCFFA6;">git restore file-name</mark> 

## Unstaging files with restore
Used when you have accidentally added a file to your staging area. 
If you don't want to include it in the next commit.
<mark style="background: #ADCCFFA6;">git restore --staged file-name</mark> 

## Undoing commits
<mark style="background: #ADCCFFA6;">git reset commit-hash </mark> will reset the repo back to a specific commit ONLY.

* If you wat to undo both the commits AND the changes in your files you can use:
<mark style="background: #ADCCFFA6;">git reset --hard #commit</mark> 

## Git Revert
Creates a brand new commit which reverses/undos the changes from a commit. It needs a commit message.
