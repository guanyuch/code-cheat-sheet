# Git Code Cheat Sheet

## From Github to local

### Clone or download repository
git clone GITHUB SSH LINK

### Check status of files
git status

### Add all files
git add .

### Add a specific file
git add FILE NAME

### Commit the changes
git commit -m "first small text field" -m "optional extended description"

### Push to Github
git push ORIGIN MASTER

## From local to Github

### Initialize Git repository
git init

### Then add and commit
git add FILE NAME
git status
git commit -m "first small text field" -m "optional extended description"

### Create new repo on Github for this local file
(Create new repo on Github)
git remote add origin GITHUB SSH LINK

### Check the connection
git remote -v

### Push it to GitHub
git push -U ORIGIN MASTER
