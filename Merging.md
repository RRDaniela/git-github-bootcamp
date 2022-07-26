## Merging
Incorporate changes form one branch into another.
1. We merge branches, not specific commits.
2. We always merge to current HEAD branch


<mark style="background: #ADCCFFA6;">Follow these steps to merge:</mark> 
1. Switch to the branch you want to merge the changes into. (Receiving branch).
2. Use git merge command to merge changes from a specific branch into the current branch.

<mark style="background: #ADCCFFA6;">git merge bugfix</mark> 

## Fastforward merge
Move a pointer up to catch up.

<mark style="background: #ADCCFFA6;">git branch -v</mark> 
Shows the last commit in branch

## Merge Conflicts
1. Open the file with merge conflicts
2. Edit the file to remove the conflicts
3. Remove the conflict markers
4. Add changer and make a commit

