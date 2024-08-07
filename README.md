# git important commands
git init->initializes git repo i.e., making local repo a git repo
<br>
git remote add origin (link)-> adding github main repo
<br>
git remote -v-> to verify remote
<br>
git add (file name/.)-> add files to staging area
<br>
git commit -m 'comment any update message'-> saves the staged changes to repo
<br>
git push -u origin main-> set this into short form for remote branch i.e., no need to write origin main repeatedly
<br>
git push-> push changes to the github main remote repo

# allow large files and push
a. git lfs install
<br>
b. git lfs track "*.jar"
<br>
c. git lfs migrate import --include="*.jar"

# branch commands
git checkout -b (new branch name)-> to create new branch
<br>
git checkout (branch name)-> moving from one branch to another
<br>
git branch-> to check branch
<br>
git branch -M main-> to rename master branch(local)
<br>
git branch -d (branch name)-> to delete branch

# merging code
git diff (branch name)->to compare commits, branches & files
<br>
git merge (branch name)-> to merge 2 branches
<br>
q-> to exit from git diff command when we stuck in loop
<br>
git pull origin main-> pull the changes from github repo main branch & update to local repo main branch

# undoing changes
Case 1: staged changes<br>
git reset (file name)->return to unstaged changes for single file after git add
<br>
git reset-> same applies but for all files

Case 2: commited changes(one commit)<br>
git reset HEAD~1->return to unstaged changes after 1 commit(i.e. return to previous commit state by 1 step)

Case 3: commited changes(multiple commits)<br>
git reset (commit sha hash)-> return to specific unstaged changes after multiple commits(i.e. return to any previous specific commit state by multiple steps)
<br>
git reset --hard (commit sha hash)->returns to specific unstaged changes & removes those unstaged changes

<b>NOTE:-</b>reset means revert back to just before the add state i.e. doesn't remove the unstaged changes
<br><br>
Fork--> A fork is copying other github account repo to our account repo. Its just a rough copy.