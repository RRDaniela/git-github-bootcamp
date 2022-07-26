## Diff
<mark style="background: #ADCCFFA6;">git diff </mark> 
shows changes between commits, branches, files, working directory. 
*Also helps to see unstaged changes.

### Output
<mark style="background: #BBFABBA6;">1. Compared files</mark> 
_diff --git a/rainbow.txt b/rainbow.txt_
<mark style="background: #BBFABBA6;">2. File Metadata (Not important)</mark> 
_index 72d1d5a..f2c8117 100644_ 
<mark style="background: #BBFABBA6;">3. Markers</mark> 
--- a/rainbow.txt
+++b/rainbow.txt
<mark style="background: #BBFABBA6;">4. Chunks</mark> 
Context before and after.
 before
 after
<mark style="background: #BBFABBA6;">5. Chunk header</mark> 
@@ -3,4 +3,5 @@
How many lines have been extracted. 

<mark style="background: #FF5582A6;">Stating = index
</mark> 

<mark style="background: #ADCCFFA6;">git diff HEAD</mark> lists all changes in the working tree since the last commit.

## Viewing staged changes
<mark style="background: #ADCCFFA6;">git diff --staged
</mark> 
All changes that have been staged. 

## Show changes of one file
<mark style="background: #ADCCFFA6;">git diff --staged colors.txt</mark> 

## Comparing branches
<mark style="background: #ADCCFFA6;">git diff branch1 branch2</mark> 

## Comparing commits
provide git diff with the commit hashes
<mark style="background: #ADCCFFA6;">git diff commit1 commit2</mark> 


## The difference between the commit where HEAD is and 1 before
<mark style="background: #ADCCFFA6;">$ git diff HEAD HEAD<mark style="background: #ADCCFFA6;"></mark> ~1</mark> 

