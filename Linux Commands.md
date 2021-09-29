# **Command Line Cheat Sheet**

## **1. Basic Linux Commands**

### cd
 - `$ cd ~ ` Navigate to HOME directory
 - `$ cd /` Navigate to the root directory
 - `$ cd .. ` Move one level up 
 - `$ cd DIRECTORY NAME` Change to a particular directory

### ls
 - `$ ls ` Lists all files and directories
 - `$ ls-R` Lists files in sub-directories as well
 - `$ ls-a ` Lists hidden files as well 
 - `$ ls-al` Lists files and directories with detailed information like permissions, size, etc.

### cat
 - `$ cat FILE NAME ` Displays the file content
 - `$ cat > FILE NAME` Creates a new file
 - `$ cat FILE1 FILE2 > FILE3 ` Joins two files and stores the output in a new file

### mv
 - `$ mv FILENAME NEW_FILENAME` Renames the file to the new name
 - `$ mv FILE 'NEW PATH' ` Moves the file to the new location

### rm
 - `$ rm FILENAME ` Deletes the file
 - `$ rm -r DIRECTORY ` Deletes the directory and its content recursively
 - `$ rm -f FILENAME ` Forces to remove the file without confirmation
 - `$ rm -rf DIRECTORY ` Forcefully deletes the directory and its content recursively

$ pwd  
# Displays the name/path of the current working directory  
$ mkdir directory_name 
# Creates a new directory   
$ cp file1 file2 
# Creates a copy of file1 as file2  
$ cat file_name 
# Displays the contents of the file  
$ less file_name 
# Displays the contents of the file (similar to above but paginates the output -use this to display  your text files!)  
$ head file_name 
# Displays the first 10 lines of the file  
$ tail file_name 
# Displays the last 10 lines of the file  
$ cd ..  
# Goes up one level in the directory tree  

$ cd  
(also, another case of this is “$ cd ~” )

# Goes to the $HOME directory  
$ cd /etc 
# Goes to the /etc directory  
$ | (e.g. ‘cd training_materials/dev1/ | ls’, goes to ‘dev1’ directory then lists all files under ‘dev1’)  # Sends output of one command to another  

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

#### Initialize Git repository
- `git init`

#### Then add and commit
- `git add FILE NAME`
- `git status`
- `git commit -m "first small text field" -m "optional extended description"`

#### Create new repo on Github for this local file
(Create new repo on Github, then use below code to connect)
- `git remote add origin GITHUB SSH LINK`

#### Check the connection
- `git remote -v`

#### Push it to GitHub
- `git push -U ORIGIN MASTER`

## **3. Git branch**

#### Check all branches
- `git branch` <br />
(* marks the branch you are on)

#### Create new branch
- `git checkout -b BRANCH NAME`

#### Change to a new branch
- `git checkout BRANCH NAME`

#### Check file changes comparing to another branch
- `git diff BRANCH NAME 2`

#### Push to GitHub
- `git push -u origin BRANCH NAME`

#### Pull request from master branch to merge feature branch
- `git pull origin BRANCH NAME`

#### Delete merged branch
- `git branch -d BRANCH NAME`
