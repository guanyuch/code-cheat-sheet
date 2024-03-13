# **Linux Commands Cheat Sheet**

## **1. Basic Linux Commands**

### cd
- `$ cd ~` Navigate to HOME directory.
- `$ cd /` Navigate to the root directory.
- `$ cd ..` Move one level up.
- `$ cd DIRECTORY_NAME` Change to a particular directory.

### ls
- `$ ls` Lists all files and directories.
- `$ ls -R` Lists files in sub-directories as well.
- `$ ls -a` Lists hidden files as well.
- `$ ls -al` Lists files and directories with detailed information like permissions, size, etc.

### cat
- `$ cat FILE_NAME` Displays the file content.
- `$ cat > FILE_NAME` Creates a new file or replaces an existing file with new content (Content added until a CTRL+D signal is sent).
- `$ cat FILE1 FILE2 > FILE3` Joins two files (FILE1 and FILE2) and stores the output in a new file (FILE3).
- `$ less FILE_NAME` Browses through a text file.
- `$ head FILE_NAME` Displays the first 10 lines of a file.
- `$ tail FILE_NAME` Displays the last 10 lines of a file.
- `$ tail -f FILE_NAME` Displays the last 10 lines of a file and follows the file as it grows.

### mv
- `$ mv FILENAME NEW_FILENAME` Renames the file to the new name.
- `$ mv FILENAME NEW_PATH` Moves the file to the new location.

### rm
- `$ rm FILENAME` Deletes the file.
- `$ rm -r DIRECTORY` Deletes the directory and its content recursively.
- `$ rm -f FILENAME` Forces to remove the file without confirmation.
- `$ rm -rf DIRECTORY` Forcefully deletes the directory and its content recursively.

### cp
- `$ cp FILENAME NEW_FILENAME` Copies the file to the new file.
- `$ cp -r SOURCE_DIR DESTINATION_DIR` Copies the source directory recursively to the destination.

### pwd
- `$ pwd` Prints the path of the working directory.

### mkdir and rmdir
- `$ mkdir DIRECTORY_NAME` Creates a new directory.
- `$ rmdir DIRECTORY_NAME` Deletes an empty directory.

### Pipes and Filters
- `|` is used to pass the output of one command as input to another. For example, `$ ls | grep 'search_term'` lists files and directories, then filters those containing 'search_term'.

### clear
- `$ clear` Clears the terminal screen.
- Note: `$ quit` is not a standard command for logging out or clearing the terminal. To log out of the current session, use `logout` or press `CTRL+D`.
