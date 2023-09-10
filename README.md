git init->initializes git repo i.e., making local repo a git repo
<br>
git remote add origin (link)-> adding github main repo
<br>
git remote -v-> to verify remote
<br>
git branch-> to check branch
<br>
git branch -M main-> to rename master branch(local)
<br>
git push -u origin main-> set this into short form for remote branch i.e., no need to write origin main repeatedly
<br>
git push-> push to the github main repo

<!---------- branch commands --------------->
git checkout -b (new branch name)-> to create new branch
<br>
git checkout (branch name)-> moving from one branch to another
<br>
git branch -d (branch name)-> to delete branch

<!---------- merging code  --------------->
git diff (branch name)->to compare commits, branches & files
<br>
git merge (branch name)-> to merge 2 branches
<br>
q-> to exit from git diff command when we stuck in loop
<br>
git pull origin main-> pull the changes from github repo main branch & update to local repo main branch

<!---------- undoing changes  --------------->
Case 1:staged changes<br>
git reset