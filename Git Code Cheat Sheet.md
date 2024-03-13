# **Git Code Cheat Sheet**

## **1. From GitHub to Local**

#### Clone or download repository
- `git clone GITHUB_SSH_LINK`

#### Check status of files
- `git status`

#### Add all files
- `git add .`

#### Add a specific file
- `git add FILE_NAME`

#### Commit the changes
- `git commit -m "commit message" -m "optional extended description"`

#### Push to GitHub
- `git push origin main`

#### Push to GitHub to overwrite
- `git push -f origin main`

#### Pull from GitHub
- `git pull`

## **2. From Local to GitHub**

#### Initialize Git repository
- `git init`

#### Then add and commit
- `git add FILE_NAME`
- `git commit -m "commit message" -m "optional extended description"`

#### Create new repo on GitHub for this local file
(Create new repo on GitHub, then use the below code to connect)
- `git remote add origin GITHUB_SSH_LINK`

#### Check the connection
- `git remote -v`

#### Push it to GitHub
- `git push -u origin main`

## **3. Git Branch**

#### Check all branches
- `git branch`  
(Note: * marks the branch you are on)

#### Create new branch
- `git checkout -b BRANCH_NAME`

#### Change to a new branch
- `git checkout BRANCH_NAME`

#### Check file changes comparing to another branch
- `git diff BRANCH_NAME`

#### Push to GitHub
- `git push -u origin BRANCH_NAME`

#### Pull request from the master branch to merge feature branch
- `git pull origin master`

#### Delete merged branch
- `git branch -d BRANCH_NAME`
