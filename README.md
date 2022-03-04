# ***Git Commands*** ![Git](/git.png){ width=40%; }


> # **Git config**<br>

This command sets the author name and email address respectively to be used with your commits.<br>
_Usage_<br> 
- git config --global user.email "[email address]"<br>
- git config --global user.name "[name]"<br>


> # **Git Add**<br>

This command will add modified files to the staged area.<br>
_Usage_<br> 
-git add <file.name>

_Flags:_<br> 
- git add .  -> Move the file from the working area to the staging area
- git add -all,-A  -> move all the files from the working directory.
- git add <filename>  -> move the file named in the staging area.


> # **Git Commit**<br>

This command will commit the added file and records the file permanently. <br>
_Usage_<br> 
-git commit -m "Message"

_Flags:_<br> 
- git commit -m " Initial Commit"  -> this command will record files permanently.
-git commit -a -> commit all the File changed Since then.

> # **Git Commit**<br>

This command will commit the added file and records the file permanently. <br>
_Usage_<br> 
-git commit -m "Message"

_Flags:_<br> 
- git commit -m " Initial Commit"  -> this command will record files permanently.
-git commit -a -> commit all the File changed Since then.

> # **Git Status**<br>

This command list all the files that have to be committed or will show the working tree status. <br>
_Usage_<br> 
-git Status

_Flags:_<br> 
- git status 
-git status -s
-git status <branchname>


> #  **Git log**<br>

_Usage_<br> 
-git log -> This command is use to see the version histoy for the current branch.


>  # **Git Init**<br>

Thid commands is used to create a locak repository.

_Usage_<br> 
-git log -> This command is use to see the version histoy for the current branch.


>  # **Git Branch**<br>

This commands list all the branches in the working directory.<vr>
_Usage_<br> 
-git branch

_flags:_<br>
- git branch -> Show all the branches.
- git branch[NewBranchname] -> will make new branch name.
- git branch -d[Branchname] -> We can Delete the branch we want too.


>  # **Git Checkout**<br>

This command is used to switch one branch to another.<br>
_Usage_<br> 
-git checkout

_flags:_<br>
- git branch -> Show all the branches.
- git checkout [New-Branch-name] -> will make new branch name.
- git switch [branch-name]  ->can switch to the another existing branch.
- git branch -b [Branch-name] -> -b makes the new branch also move to the new branch.


> # **Git Merge**<br>

This command is used to merge with the another branch.<br>
_Usage_<br> 
- git merge [branch-name]
- git merge [source-branch] [target-branch] -> Merge a branch into a target branch.<br>


>  #  **Git Remove**<br>

This command is used to delete the file.<br>
_Usage_<br> 
- git rm [file-name] -> This command is used to delete the file from your working directory and stages the deletion.

_flags:_ <br>
- git rm -r [file-name.txt] -> Remove a file.

# **Git Remote**<br>

_Usage_ <br>
- git remote -> This commands let you to view , create and delete the connections to other repositories.

_Flags:_
- git remote -v -> It show the name of all remote repo including URL.
- git remote add [Name][URl] ->This command will help to make a remote repo and can use anywhere with the help of name convinient to URL.
- git remote rm [name] -> This command will remove the connection to the remote repo[name]. 
- git remote [old-name] [new-name] -> THis will rename the old name of remote repo with the new name.