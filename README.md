# ***Git Commands*** <img src=Git.png alt="Git" width=70> <img src=gitlogo.png alt="GitHub" width=70>


## GIT URL's
1. Git:  

## **Some another Git Commands**
1. *pwd*   It is used to print the present working directory.
2. *cd [folder-name]*   It stands for Change Directory. It is used to move into the folder named.
3. *cd ..*   It is used to move one folder back.
4. *cd*   It is used to move to the initial path or at the start of the terminal.
5. *ls*   It is used list all the files and folders in the working directory.
6. *ls -a*   It is used list all the files and folders in the working directory including the hidden folder too.
7. *ls --list*   It is used list all the files and folders in the working directory.


## **Git Log**
The git log command shows all the commits made in a repository. You can see the hash ofe each commits, the message associated with and more metadata. OR we can say this command is used for displaying the history of a repository.

_Usage:_

* To see the history of all the commits done.
```bash 
git log
```   
* To see the info of all the commits in oneline. 
```bash 
git log --oneline
```   
* We can restore the data after the date mentioned.
```bash 
git log --after
```
*  we can restore the data before the date mentioned and can put the relative value that is yesterday.
```bash 
git log --before
```  
* This command is used to see a specific number of commit and the where _a_ is specific number of commits you want to see.
```bash 
git log -n _a_
```     

## **Git config** 

* This command sets the author name and email address respectively to be used with your commits.
* We can store the name locally or globally or we can configure the name for a file.Your Git username does not need to be the same as your version control username, such as the one you use on GitHub. The git config command configures your Git installation.
_Usage:_  
* List all The commits.
```bash 
git config --list
```   
* It is used to set the email of the user.
```bash 
git config --global user.email "[email-address]"
```   
* This command is used to set the name of the user.
```bash   
git config --global user.name "[name]"
``` 

## **Git Add** 

This command will add modified files to the staged area. 
_Usage:_  
* git add <file.name>

_Flags:_  
* Move the file from the working area to the staging area
```bash 
git add .
```    
* move all the files from the working directory.
```bash 
git add -all,-A 
```   
* move the file named in the staging area.
```bash 
git add <filename>
```    

## **Git Commit** 

This command will commit the added file and records the file permanently.  
_Usage_  
* git commit -m "Message"

_Flags:_  
* This command will record files permanently.
```bash
git commit -m " Initial Commit"
```
* It commits all the File changed Since then. 
```bash
git commit -a
```   


## **Git Status** 

This command list all the files that have to be committed or will show the working tree status.  
_Usage_  
* git Status

_Flags:_  
```bash
git status 
```
```bash
git status -s
```
```bash
git status <branchname>
```

## **Git Push**

When you save a file in a Git Repository,the changes will be stored in your computer, we can push the local repository to remote repository BY the help of this command.

_Usage:_
* It Also push the local repo into remote and -u -> Where u means upstream/ -set-upstream.
```bash
git push -u origin master
``` 
* This command help us to push the [branch-name] to the [remote-repository]
```bash
git push [remote-name] [branch-name]
```


## **Git Init** 



## **Git Branch** 

This commands list all the branches in the working directory.<vr>
_Usage_  
* git branch

_flags:_ 
* git branch --list,-l   This command list all the branches.
* git branch   Show all the branches.
* git branch[NewBranchname]   will make new branch name.
* git branch -d[Branchname]   We can Delete the branch we want too.
* git branch -a,--all   This command help us to see all the branches in the local  repository and in the remote repository.
* git branch -D  It is used to Delete the  branches.
* git branch -r   It is used to show all the remote branches.


## **Git Checkout** 

This command is used to switch one branch to another. 
_Usage_  
* git checkout

_flags:_ 
* git branch   Show all the branches.
* git checkout [New-Branch-name]   will make new branch name.
* git switch [branch-name]   can switch to the another existing branch.
* git branch -b [Branch-name]   -b makes the new branch also move to the new branch.


## **Git Merge** 

This command is used to merge with the another branch. 
_Usage_  
* git merge [branch-name]
* git merge [source-branch] [target-branch]   Merge a branch into a target branch. 


##  **Git Remove** 

This command is used to delete the file. 
_Usage_  
* git rm [file-name]   This command is used to delete the file from your working directory and stages the deletion.

_flags:_  
* git rm -r [file-name.txt]   Remove a file.

## **Git Remote** 

_Usage_  
* git remote   This commands let you to view , create and delete the connections to other repositories 

_Flags:_
* This command is used to add or link the remote repo to the localrepo after then we can push,pukk and fetch the file from remote repository.
```bash 
git remote add [remote-name] [URL]   
```
* This command let us see all the remote branches and associated metadata.
```bash 
git remote show 
```
* It show the name of all remote repo including URL.
```bash 
git remote -v 
```
* This command will help to make a remote repo and can use anywhere with the help of name convinient to URL.
```bash 
git remote add [Name][URl] 
``` 
* This command will remove the connection to the remote repo[name].
```bash 
git remote rm [name]
```    
* This will rename the old name of remote repo with the new name.
```bash 
git remote [old-name] [new-name] 
```


## **Git Fetch**
The Git Fetch command is used when the branch exists on a remote repository not on the local repository, so if you want to fetch the file in a local repository,we usse this fetch command.

_usage:_
*  Fetch the files from the remoite repository.
```bash 
git fetch [remote-name] [file-name]  
```
* After fetching the file from the remote repository, Use this command to see the files we fetched:
```bash 
git checkout [remote-name]/[branch-name]
```
## **Git Clone**
The Git clone is used to make a copy or clone of a repository along with its history of commits on the local repository on your computer. Cloning allows you to make a independent version of the main repository.

_Usage_
*  To clone the remote repository in the local repository on your computer.
```bash 
git clone [URL][remote-repo-name.git] 
```

* To clone the repository in a folder named.
```bash
git clone [remote-repo] [folder-name] 
```
### Git-Swallow 
* If In the project, we have hundred of commits it take longer to clone. To skip clonning the entire repository,you can create a swallow clone.
In swallow clone the history of commit specified in depth.
```bash
git clone -depth=1 [repo]
```
* For clonning the latest last 10 clone from the remote repo.
```bash 
git clone -depth=10 https://github.com/username/project-name.git  
```
* We may two or more branch and younn want to clone a Specific branch
```bash
git clone --single-branch --branch master https://github.com/[user-name]/[repository-name].