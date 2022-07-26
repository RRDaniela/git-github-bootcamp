ccd ## What is Github?
Is a hosting platform for git repositories.
You can put your Git repos on Github and access them from anywhere and share them.

It also helps people share and collaborate on repos.

## Cloning
==git clone== goes and gets a repository that is not on your machine and it brings it to your machine.
<mark style="background: #FF5582A6;">make sure you're not inside a git repo</mark> 

<mark style="background: #BBFABBA6;">It's a GIT command
</mark> 


## SSH
Secure shell
protocol that allows to be authenticated without putting email and password at each interaction

https://docs.github.com/en/authentication/connecting-to-github-with-ssh

## Remote
Setup a destination

## Creating a Github Repo
### Option 1.
#### Existing Repo on laptop
1. First create repo on Github.com
2. <mark style="background: #ADCCFFA6;">git remote -v</mark> 
3. <mark style="background: #ADCCFFA6;">git remote add origin URL</mark> 
4. ![[Pasted image 20220725100104.png]]
5. git push REMOTE BRANCH
	1. Example:
	2. <mark style="background: #ADCCFFA6;">git push origin master:</mark> tells git to push up the master branch to our origin remote
	3. ![[Pasted image 20220725101406.png]]

<mark style="background: #FF5582A6;">RENAME A REMOTE</mark> 
git remote rename <old> <new>
<mark style="background: #FF5582A6;">REMOVE A REMOTE</mark> 
git remote remove <name>


## How to push from a local branch to a remote branch with a different name
Example:
<mark style="background: #ADCCFFA6;">git push origin pancake:waffle</mark> 
This is to push from our local pancake branch up to a remote branch called waffle. 


## What does git push -u mean?
Upstream: A connection from the local branch to a branch on Github.
Example:
1. If we had a local dogs branch and a remote dogs branch we would have to do:
2. <mark style="background: #ADCCFFA6;">git push origin dogs.</mark> 
3. We could set an upstream so we only do <mark style="background: #ADCCFFA6;">git push</mark> 
4. To set an upstream we have to run the following command:
5. <mark style="background: #ADCCFFA6;">git push -u origin dogs</mark> 
6. Now we have an upstream set! Just do <mark style="background: #ADCCFFA6;">git push</mark> 

## Option 2:
### Start from scratch

1. Create a brand new repo on github
2. Clone it on your machine

## Rename Master to Main
<mark style="background: #ADCCFFA6;">git branch -M main</mark> 

## Option 3:

