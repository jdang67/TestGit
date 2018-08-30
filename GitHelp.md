##Rename a local and remote branch in git
If you have named a branch incorrectly AND pushed this to the remote repository follow these steps before any other developers get a chance to jump on you and give you shit for not correctly following naming conventions.

#1. Rename your local branch.
If you are on the branch you want to rename:
c:\> git branch -m new-name

#2. Delete the old-name remote branch and push the new-name local branch.

c:\> git push origin :old-name new-name
#3. Reset the upstream branch for the new-name local branch.
c:\> git push origin -u new-name