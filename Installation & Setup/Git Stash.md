## Stash
Save changes without actually committing them.


<mark style="background: #ADCCFFA6;">git stash </mark> 
_saves your changes_ and allows to change branches without taking the changes w/ you or having conflicts.

<mark style="background: #ADCCFFA6;">git stash pop</mark> 
removes the most recently stashed changes and re-applies them 

<mark style="background: #ADCCFFA6;">git stash apply</mark> 
apply whateves is stashed away without removing it from the stash
useful when trying to apply changes to different branches because it <mark style="background: #BBFABBA6;">stays</mark> in stash.

<mark style="background: #BBFABBA6;">YOU CAN STASH DIFFERENT CHANGES</mark> 
1. git stash
2. git stash list
3. choose which one you want to apply
4. git stash apply stash@{2}

## Dropping and clearing the stash
To delete a particular stash
==git stash drop <stash-id>




