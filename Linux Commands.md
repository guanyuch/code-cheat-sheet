# **Command Line Cheat Sheet**

## **1. Basic Linux Commands**

### cd
 - `$ cd ~ ` Navigate to HOME directory
 - `$ cd / ` Navigate to the root directory
 - `$ cd .. ` Move one level up 
 - `$ cd DIRECTORY NAME ` Change to a particular directory

### ls
 - `$ ls ` Lists all files and directories
 - `$ ls-R ` Lists files in sub-directories as well
 - `$ ls-a ` Lists hidden files as well 
 - `$ ls-al ` Lists files and directories with detailed information like permissions, size, etc.

### cat
 - `$ cat FILE NAME ` Displays the file content
 - `$ cat > FILE NAME ` Creates a new file
 - `$ cat FILE1 FILE2 > FILE3 ` Joins two files and stores the output in a new file <br /> 
 - `$ less FILE NAME ` Browses through a text file
 - `$ head FILE NAME ` Displays the first 10 lines of file
 - `$ tail FILE NAME ` Displays the last 10 lines of file
 - `$ tail -f FILE NAME ` Displays the last 10 lines of file and follows the file as it grows

### mv
 - `$ mv FILENAME NEW_FILENAME ` Renames the file to the new name
 - `$ mv FILE 'NEW PATH' ` Moves the file to the new location

### rm
 - `$ rm FILENAME ` Deletes the file
 - `$ rm -r DIRECTORY ` Deletes the directory and its content recursively
 - `$ rm -f FILENAME ` Forces to remove the file without confirmation
 - `$ rm -rf DIRECTORY ` Forcefully deletes the directory and its content recursively

### cp
 - `$ cp FILENAME NEW_FILENAME ` Copies the file to the new file
 - `$ cp -r SOURCE_DIR DESTINATION_DIR ` Copies the source directory recursively to destination.

# Pan Yiqing

$ pwd 
# Displays the name/path of the current working directory  
$ mkdir directory_name
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
