## Remote tracking branches
_At the time you last communicated with this remote repository, here is where x branch was pointing_

<mark style="background: #ADCCFFA6;">git branch -r</mark> to see the remote tracking branch

A RTB is a reference to the state of the master branch on the remote. Like a bookmark <mark style="background: #FFB8EBA6;">pointing to the last known commit on the master branch on origin.</mark> 


## Remote branches
<mark style="background: #ADCCFFA6;">git branch -r</mark> to see them
<mark style="background: #ADCCFFA6;">git switch REMOTE-BRANCH-NAME</mark> 

<mark style="background: #FFB8EBA6;">After git clone URL:</mark> 
GMX+109020781 (main)
$ <mark style="background: #FFF3A3A6;">git branch -r</mark> 
  origin/HEAD -> origin/main
  origin/fantasy
  origin/food
  origin/main
  origin/more-fantasy
  origin/morefood
  origin/movies

GMX+109020781(main)
$ <mark style="background: #FFF3A3A6;">ls</mark> 
cactus.txt  rose.txt

GMX+109020781(main)
$ <mark style="background: #FFF3A3A6;">start rose.txt</mark> 

GMX+109020781(main)
$ <mark style="background: #FFF3A3A6;">git switch food</mark> 
Switched to a new branch 'food'
branch 'food' set up to track 'origin/food'.

GMX+109020781(food)
$ <mark style="background: #FFF3A3A6;">ls</mark> 
apple.txt  banana.txt  coffee.txt  popsicle.txt  tea.txt

GMX+109020781(food)
$ <mark style="background: #FFF3A3A6;">start apple.txt</mark> 

# Fetch
Allows to download changes but you don't have to merge them into what you're working on.

<mark style="background: #ADCCFFA6;">git fetch origin master</mark> 

If you want to see them you can do
<mark style="background: #ADCCFFA6;">git checkout origin/master</mark> , but MY master branch is untouched.

# Pull
We can use it to retrieve changes. It updates our working directory.

<mark style="background: #FFF3A3A6;">git pull = git fetch + git merge</mark> 

<mark style="background: #ADCCFFA6;">git switch movies
git pull origin movies</mark> 

<mark style="background: #FF5582A6;">It can result in merge conflicts!</mark> 

<mark style="background: #FF5582A6;">BEFORE PUSHING YOU SHOULD PULL CHANGES</mark> 

### Shorter syntax for git pull
If I run <mark style="background: #ADCCFFA6;">git pull</mark> in a particular branch it'll retrieve the changes in that remote branch

<label class="ob-comment" title="IMPORTANT" style="background-color:yellow color:black"> Remember to set an upstream first <input type="checkbox"> <span style=""> Comment </span></label>

![[Pasted image 20220725150816.png]]

