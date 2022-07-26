### Branches
Alternative timelines for a project
______________________________________________

<mark style="background: #BBFABBA6;">(HEAD -> master)</mark> 
_(bookmark)_
HEAD is branch a pointer that refers to the current "location"


### Viewing branches
<mark style="background: #ADCCFFA6;">git branch</mark> 
with *  we see the branch we're on. 

### Make a new branch
<mark style="background: #ADCCFFA6;">git branch [branch-name] </mark>  upon the current HEAD
### Change branch
<mark style="background: #ADCCFFA6;">git switch [branch-name]</mark>  OR <mark style="background: #ADCCFFA6;">git checkout [branch-name]</mark> 

### Oneline way to add and commit
<mark style="background: #ADCCFFA6;">git commit -a -m "This is the message"
</mark> 


## Git Checkout vs Git Switch

Same behavior, git switch was made to simplify the switching of branches.

### Creating & Switching
<mark style="background: #ADCCFFA6;">git switch -c [BRANCH-NAME]</mark> 


<mark style="background: #FF5582A6;">ALWAYS ADD AND COMMIT CHANGES BEFORE CHANGING BRANCHES TO AVOID LOSING CHANGES OR TAKING FILES WITH YOU TO OTHER BRANCHES.</mark> 

## Deleting and renaming branches
1. Change to another branch that aint the one you want to delete.
2. <mark style="background: #ADCCFFA6;">git branch -d NAMEOFBRANCH </mark> 

### Renaming
1. Change to the branch you want to rename
2. <mark style="background: #ADCCFFA6;">git branch -m NEWNAMEOFBRANCH</mark> 

