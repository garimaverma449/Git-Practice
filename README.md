# ***Git Commands*** <img src="Git.png" alt="GIT" width="100"/ 


## **Git config** 

This command sets the author name and email address respectively to be used with your commits. 
_Usage_  
- git config --global user.email "[email address]" 
- git config --global user.name "[name]" 


## **Git Add** 

This command will add modified files to the staged area. 
_Usage_  
- git add <file.name 

_Flags:_  
- git add .  -  Move the file from the working area to the staging area
- git add -all,-A  -  move all the files from the working directory.
- git add <filename   -  move the file named in the staging area.


## **Git Commit**

This command will commit the added file and records the file permanently.  
_Usage_  
- git commit -m "Message"

_Flags:_  
- git commit -m " Initial Commit"  -> This command will record files permanently. 
- git commit -a -  This will commit all the File changed since then.


## **Git Status**

This command list all the files that have to be committed or will show the working tree status.  
_Usage_  
- git Status

_Flags:_  
- git status 
- git status -s
- git status <branch-name> 


##  **Git log**

_Usage_  
- git log -  This command is use to see the version histoy for the current branch.


## **Git Init** 

This commands is used to create a local repository.

_Usage_  
- git log -  This command is use to see the version histoy for the current branch.


## **Git Branch** 

This commands list all the branches in the working directory.
_Usage_  
- git branch

_flags:_ 
- git branch ->  This will show all the branches.
- git branch --list -> This will show the list of branches.
- git branch -a,-all-> This will show the list of branches.
- git branch [New-Branch-name] ->  It will make new branch name.
- git branch -d [Branch-name] ->  We can Delete the branch we want too.
- git branch -D -> Delete Branch
- git checkout -b [branch-name] -> This command will make the new branch and switched to the new branch.


## **Git Checkout** 

This command is used to switch one branch to another. 
_Usage_  
-git checkout

_flags:_ 
- git branch -  Show all the branches.
- git checkout [New-Branch-name] -  will make new branch name.
- git switch [branch-name]  - can switch to the another existing branch.
- git branch -b [Branch-name] -  -b makes the new branch also move to the new branch.


## **Git Merge** 

This command is used to merge with the another branch. 
_Usage_  
- git merge [branch-name]
- git merge [source-branch] [target-branch] -  Merge a branch into a target branch. 


##  **Git Remove** 

This command is used to delete the file. 
_Usage_  
- git rm [file-name] -  This command is used to delete the file from your working directory and stages the deletion.

_flags:_  
- git rm -r [file-name.txt] -  Remove a file.

## **Git Remote** 

_Usage_  
- git remote -  This commands let you to view , create and delete the connections to other repositories.

_Flags:_
- git remote -v -  It show the name of all remote repo including URL.
- git remote add [Name][URl] - This command will help to make a remote repo and can use anywhere with the help of name convinient to URL.
- git remote rm [name] -  This command will remove the connection to the remote repo[name]. 
- git remote [old-name] [new-name] -  THis will rename the old name of remote repo with the new name.