## Merging in Feature Branches
How to merge your own branches in. (After team approval):
1. Switch to main
2. git pull origin main
3. git merge ==BRANCH YOU'RE MERGING FROM==
4. git push origin main

## Pull Requests
They allow to alert team-members that new work that needs to be reviewed.

## Fork
Allows to create personal copies of other people's repositories.
_"Make my own copy of this repo"_

1. We click on the repo we want to fork
2. We do <mark style="background: #ADCCFFA6;">git clone (URL OF OUR REPO)</mark>
3. git add .
4. git commit -m "commit message"
5. git push origin master <mark style="background: #ADCCFFA6;">(ON MY FORK)</mark> 


## The fork & clone workflow
==Attempt to share to the original repository==
1. Fork the project
2. Clone the fork
3. Add upstream remote
4. Do some work
5. Push to origin
6. Open pull request

<mark style="background: #FFF3A3A6;">git remote -v if you have any doubts</mark> 

After creating a fork:
1. <mark style="background: #BBFABBA6;">ORIGINAL </mark> git remote add upstream [URL ORIGINAL]
2. <mark style="background: #FFB8EBA6;">FORK</mark> git clone [URL FORK MINE]



