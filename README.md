git init
git status

Working directory 

git add <filename> 

Staging

git commit -m "comments"

Local Repository

git push

Remote Repository

git init  -- to initialize project
git staus
git add <filename>   --- to add files from working dir to staging location 
git commit -m "comments"  --- to commit files from staging locatgion to local repository
git branch -M main
git remote add origin https://github.com/Raja-GitRep/Ansible.git      -- to setup the remote repository 
git push -u origin main    --- to push the project from local reposoitory to remote repository 


git branch  -- show the branch details which we are in now

git clone <git project URL>   -- to get the project from remote repo to our local 

git checkout  "branch name" / git checkout -b "branch name"   -- to switch to branch   -b will create if that branch not exist
-----------------------------------------------------------
raju@DESKTOP-VAPO6U8:~/Ansible_work$ git checkout raja_test
error: pathspec 'raja_test' did not match any file(s) known to git
raju@DESKTOP-VAPO6U8:~/Ansible_work$ git checkout -b raja_test
Switched to a new branch 'raja_test'
raju@DESKTOP-VAPO6U8:~/Ansible_work$ git branch
  main
* raja_test
raju@DESKTOP-VAPO6U8:~/Ansible_work$ git checkout main
Switched to branch 'main'
raju@DESKTOP-VAPO6U8:~/Ansible_work$



git pull  -- this will pull the code from master and update our local
git fetch   -- this will pull the code from master and not update our local

--------------merge conflicts--------------------
master branch -- hi
dev1 pull -- hi
dev2 pull -- hi
dev1 pushed -- hii  and its merged to marster
now Master and Dev1 have -- hii
now when Dev2 pushed -- hi-dev
there will be merge conflicts as Master is having 'hii' and Dev2 trying to push 'hi-dev'
then to resolve this we need to 'git pull' in **master branch** then run 'git merge origin/main' in **Dev2 branch**

