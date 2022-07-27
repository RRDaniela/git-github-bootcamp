## Reflog
### Limitations
Git only keeps reflogs locally. They are not shared with collaborators.
They also expire, after 90 days.

### Git reflog command
Accepts subcommands: show, expire, delete and exists.

<mark style="background: #ADCCFFA6;">git reflog show HEAD</mark> 
We see a log. Show track of every change to HEAD.

## How to go back in time in a branch
<mark style="background: #ADCCFFA6;">git checkout master(branch)@{1.week.ago}</mark> 

### Rescue lost commits
1. Pick a point you want to go back to. <mark style="background: #ADCCFFA6;">git log --oneline</mark> 
2. <mark style="background: #ADCCFFA6;"> git reset --hard HASH</mark>
3. <mark style="background: #ADCCFFA6;">git reflog show master</mark> to see your deleted commits
4. <mark style="background: #ADCCFFA6;">git reset --hard</mark> <mark style="background: #FFB8EBA6;">master@{1}</mark> or the <mark style="background: #FFB8EBA6;">HASH</mark> 

### Undoing a rebase
1. After <mark style="background: #ADCCFFA6;">git rebase -i HEAD~4</mark> 
2. <mark style="background: #ADCCFFA6;">git reflog show</mark> <mark style="background: #FFB8EBA6;">BRANCH</mark> 
3. Copy <mark style="background: #FFB8EBA6;">HASH</mark> 
4. <mark style="background: #ADCCFFA6;">git reset --hard</mark> <mark style="background: #FFB8EBA6;">HASH</mark> 
5. <mark style="background: #ADCCFFA6;">git log</mark> 

