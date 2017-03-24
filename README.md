# Git-Bash-Commands

vi filename - create/edit file
to exit the file and save it - press exit and then write :wq


git init - create a .git folder (create repository)

git hash-object -w filename - save the file to the .git repo in the (.git/objects) as a hashed file

git cat-file -p [hash number] - geting the original file content

git status - what git knows about the changed files

git commit - save the project folder version and the commit massge, 
by hashing the commit - the commit hashing number point to the commit info  (author, time stamp etc..) 
and to the hash tree number (the hash tree number - point to the hashfiles content number and from there we get all the content)
git commit -am "commit description" - shorter way two use git add -A (add all) + git commit -m "commit secription.
-------------------branch--------------------------
https://www.youtube.com/watch?v=oFYyTZwMyAg

branches let you duplicate a specific version of the project, without worry about that it will change by someone else while you 
working on a new feature and after you finished
you can push the changes you did to the original project (master branch)(that might already been changed by other pull requests)

git branch featureName - create a branch named featureName 
git branch - show you the branches that exist
git checkout [branchname] - switching branch to name specified
git checkout -b [branchname] - switching branch , if the branch not exist it create it
git merge [branchname] - will try to merge all the changes in the branch specified into the current branch is in (for example if i in 
feature1 branch and i write git merge master - it will take all the changes from master and try to paste it into the feature1 branch)
-when we create a branch it will create it by refrencing to the branch that we were on -