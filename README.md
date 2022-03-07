# ***Git Commands*** <img src=Git.png alt="Git" width=70> <img src=gitlogo.png alt="GitHub" width=70>


## **Some another Git Commands**
1. *pwd* -> It is used to print the present working directory.
2. *cd [folder-name]* -> It stands for Change Directory. It is used to move into the folder named.
3. *cd ..* -> It is used to move one folder back.
4. *cd* -> It is used to move to the initial path or at the start of the terminal.
5. *ls* -> It is used list all the files and folders in the working directory.
6. *ls -a* -> It is used list all the files and folders in the working directory including the hidden folder too.
7. *ls --list* -> It is used list all the files and folders in the working directory.


## **Git Log**
The git log command shows all the commits made in a repository. You can see the hash ofe each commits, the message associated with and more metadata. OR we can say this command is used for displaying the history of a repository.

_Usage:_
* git log -> To see the history of all the commits done.
* git log --oneline -> To see the info of all the commits in oneline.
* git log --after -> We can restore the data after the date mentioned.
* git log --before -> we can restore the data before the date mentioned and can put the relative value that is yesterday.
* git log -n _a_ -> This command is used to see a specific number of commit and the where _a_ is specific number of commits you want to see.  

## **Git config** 

* This command sets the author name and email address respectively to be used with your commits.
* We can store the name locally or globally or we can configure the name for a file.Your Git username does not need to be the same as your version control username, such as the one you use on GitHub. The git config command configures your Git installation.
_Usage:_  
* git config --list -> List all The commits.
* git config --global user.email "[email-address]" -> It is used to set the email of the user.
* git config --global user.name "[name]" -> This command is used to set the name of the user.


## **Git Add** 

This command will add modified files to the staged area. 
_Usage:_  
* git add <file.name>

_Flags:_  
* git add .  -> Move the file from the working area to the staging area
* git add -all,-A  -> move all the files from the working directory.
* git add <filename>  -> move the file named in the staging area.

## **Git Commit** 

This command will commit the added file and records the file permanently.  
_Usage_  
* git commit -m "Message"

_Flags:_  
* git commit -m " Initial Commit"  -> this command will record files permanently.
* git commit -a -> commit all the File changed Since then.

## **Git Status** 

This command list all the files that have to be committed or will show the working tree status.  
_Usage_  
* git Status

_Flags:_  
* git status 
* git status -s
* git status <branchname>

## **Git Push**

When you save a file in a Git Repository,the changes will be stored in your computer, we can push the local repository to remote repository BY the help of this command.

_Usage:_
* git push -u origin master -> It Also push the local repo into remote 
```bash
-u , -set-upstream - Where u means upstream
```
* git push [remote-name] [branch-name] -> This command help us to push the [branch-name] to the [remote-repository].


## **Git Init** 



## **Git Branch** 

This commands list all the branches in the working directory.<vr>
_Usage_  
* git branch

_flags:_ 
* git branch --list,-l -> This command list all the branches.
* git branch -> Show all the branches.
* git branch[NewBranchname] -> will make new branch name.
* git branch -d[Branchname] -> We can Delete the branch we want too.
* git branch -a,--all -> This command help us to see all the branches in the local  repository and in the remote repository.
* git branch -D ->It is used to Delete the  branches.
* git branch -r -> It is used to show all the remote branches.


## **Git Checkout** 

This command is used to switch one branch to another. 
_Usage_  
* git checkout

_flags:_ 
* git branch -> Show all the branches.
* git checkout [New-Branch-name] -> will make new branch name.
* git switch [branch-name]  ->can switch to the another existing branch.
* git branch -b [Branch-name] -> -b makes the new branch also move to the new branch.


## **Git Merge** 

This command is used to merge with the another branch. 
_Usage_  
* git merge [branch-name]
* git merge [source-branch] [target-branch] -> Merge a branch into a target branch. 


##  **Git Remove** 

This command is used to delete the file. 
_Usage_  
* git rm [file-name] -> This command is used to delete the file from your working directory and stages the deletion.

_flags:_  
* git rm -r [file-name.txt] -> Remove a file.

## **Git Remote** 

_Usage_  
* git remote -> This commands let you to view , create and delete the connections to other repositories 

_Flags:_
* git remote add [remote-name] [URL] : This command is used to add or link the remote repo to the local repo after then we can push,pukk and fetch the file from remote repository.
* git remote show -> This command let us see all the remote branches and associated metadata.
* git remote -v -> It show the name of all remote repo including URL.
* git remote add [Name][URl] ->This command will help to make a remote repo and can use anywhere with the help of name convinient to URL.
* git remote rm [name] -> This command will remove the connection to the remote repo[name]. 
* git remote [old-name] [new-name] -> THis will rename the old name of remote repo with the new name.

## **Git Fetch**
The Git Fetch command is used when the branch exists on a remote repository not on the local repository, so if you want to fetch the file in a local repository,we usse this fetch command.

_usage:_
* git fetch [remote-name] [file-name] -> Fetch the files from the remoite repository.
```bash
After fetching the file from the remote repository, Use this command to see the files we fetched:
git checkout [remote-name]/[branch-name]
```
