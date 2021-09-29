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
 - `$ cat FILE1 FILE2 > FILE3 ` Joins two files and stores the output in a new file
 - `$ less FILE NAME ` Browses through a text file
 - `$ head FILE NAME ` Displays the first 10 lines of file
 - `$ tail FILE NAME ` Displays the last 10 lines of file
 - `$ tail -f FILE NAME ` Displays the last 10 lines of file and follows the file as it grows

### mv
 - `$ mv FILENAME NEW_FILENAME ` Renames the file to the new name
 - `$ mv FILE 'NEW PATH' ` Moves the file to the new location
 - `$ put FILENAME ` Uploads a file from local directory to remote directory
 - `$ get FILENAME ` Downloads a file from remote directory to local directory.

### rm
 - `$ rm FILENAME ` Deletes the file
 - `$ rm -r DIRECTORY ` Deletes the directory and its content recursively
 - `$ rm -f FILENAME ` Forces to remove the file without confirmation
 - `$ rm -rf DIRECTORY ` Forcefully deletes the directory and its content recursively

### cp
 - `$ cp FILENAME NEW_FILENAME ` Copies the file to the new file
 - `$ cp -r SOURCE_DIR DESTINATION_DIR ` Copies the source directory recursively to destination.

### pwd
 - `$ pwd ` Prints the path of the working directory

### mkdir
 - `$ mkdir DIRECTORY NAME` Creates a new directory
 - `$ rmdir DIRECTORY NAME` Deletes a new directory

### |
 - `$ | ` e.g. ‘cd training_materials/dev1/ | ls’, goes to ‘dev1’ directory then lists all files under ‘dev1’

 ### clear
 - `$ clear ` Clears the terminal
 - `$ quit` Logs out

 ### 