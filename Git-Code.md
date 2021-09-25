# **Git Code Cheat Sheet**

## **1. From Github to local**

#### Clone or download repository
- `git clone GITHUB SSH LINK`

#### Check status of files
- `git status`

#### Add all files
- `git add .`

#### Add a specific file
- `git add FILE NAME`

#### Commit the changes
- `git commit -m "first small text field" -m "optional extended description"`

#### Push to Github
- `git push ORIGIN MASTER`

#### Pull from Github
- `git pull`

## **2. From local to Github**

### Initialize Git repository
- `git init`

### Then add and commit
- `git add FILE NAME`
- `git status`
- `git commit -m "first small text field" -m "optional extended description"`

### Create new repo on Github for this local file
(Create new repo on Github, then use below code to connect)
- `git remote add origin GITHUB SSH LINK`

### Check the connection
- `git remote -v`

### Push it to GitHub
- `git push -U ORIGIN MASTER`

## **3. Git branch**

### Check all branches
- `git branch` <br />
(* marks the branch you are on)

### Create new branch
- `git checkout -b BRANCH NAME`

### Change to a new branch
- `git checkout BRANCH NAME`

### Check file changes comparing to another branch
- `git diff BRANCH NAME 2`

### Push to GitHub
- `git push -u origin BRANCH NAME`

### Pull request from master branch to merge feature branch
- `git pull origin BRANCH NAME`

### Delete merged branch
- `git branch -d BRANCH NAME`
