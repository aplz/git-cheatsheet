git-cheatsheet
==============

#### branch
+ rename branch: git branch -m <oldname> <newname>
+ set local branch to track remote branch: git branch --set-upstream develop origin/develop

#### remotes
+ see remote origin: git remote -v
+ change remote origin url: git remote set-url origin \<url\>
+ remove remote: git remote rm \<name_of_remote_to_remove\>

 
#### stash
git stash<br /> 
git branch \<branch_name\><br /> 
git checkout \<branch_name\><br /> 
git stash apply<br /> 

#### stash naming
git stash save "abc"<br /> 
git stash apply stash^{/abc}<br /> 

#### commit in wrong branch
git reset --soft HEAD^<br /> 
git stash<br /> 
git co <rightbranch><br /> 
git stash apply<br /> 

#### aliases
+ undo commit: git config --global alias.undo-commit 'reset --soft HEAD^' 
