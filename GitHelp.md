##Rename a local and remote branch in git
If you have named a branch incorrectly AND pushed this to the remote repository follow these steps before any other developers get a chance to jump on you and give you shit for not correctly following naming conventions.

#1. Rename your local branch.
If you are on the branch you want to rename:
c:\> git branch -m new-name

#2. Delete the old-name remote branch and push the new-name local branch.

c:\> git push origin :old-name new-name
#3. Reset the upstream branch for the new-name local branch.
c:\> git push origin -u new-name



## Git Revert
this command will auto comit  after revert
git revert 99759c7a33ad3 

this command will not comit after revert.
git revert -n 99759c7a33ad3

## Git Reset.

git command will reset the curent branch to this commit at local.
git reset --hard 99759c7a33ad35518c1f46cb74f558134278a70a

after reset local, you need to  force to push this changes to remote 
gut push origin -f 