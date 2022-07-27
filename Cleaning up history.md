## Interactive Git Rebase
Combine commits down before sharing your work.

<mark style="background: #ADCCFFA6;">git rebase -i HEAD~4</mark> 

4 is how many commits we want to go back.

Opens text editor, the following will appear:

```
pick cbee26b I added project files
pick 519aab6 add basic HTML boilerplate
pick 240827f add bootstrap
pick 6e39a76 whoops forgot to add bootstrap js script
pick 4ff2290 add top navbar
pick 2a45e71 fix navbar typos
pick 655204d fix another navbar typo
pick 2029e20 my cat made this commit
pick 3b23c17 Create README.md
```

<mark style="background: #BBFABBA6;">pick</mark> : use the commit, don't change it.
<mark style="background: #BBFABBA6;">reword</mark> : change the commit message. (Choose a commit and change <mark style="background: #FFB8EBA6;">pick</mark> to <mark style="background: #FFB8EBA6;">reword</mark> to change message).
<mark style="background: #BBFABBA6;">fixup</mark> : use contents but mush it together with the previous commit.
![[Pasted image 20220726212247.png]]
fixup was mushed with _add bootstrap_

<mark style="background: #BBFABBA6;">drop</mark> : remove a commit and its changes.

To fix the last commit:
<mark style="background: #ADCCFFA6;">git commit --amend</mark> 

