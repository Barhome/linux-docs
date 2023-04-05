## some rule

- / the first one is called root file system and the next / in a directory is called a separator
- names of directories is case sensetive
- when writing a directory like document you can write like this document/ ending it with / or like this document
- when writing a file in a directory make sure not to end it with /
- use ls to list the content of a directory
- files are colored with white and directories are colored with blue
- use cat command to view the content of a file `cat /var/log/messages` this will show you messages content , cat stands for concatinate
- use pwd command to show you your working directory , pwd stands for print working directory
- use cd command to move change directories as cd stands for change directory , use `cd - ` to go to the last working directory , use `cd` or `cd ~` to move to the current user home directory or `cd ~imohamed` to move to the home directory of any other user like imohamed or `cd ~/Downloads` to move to Downloads directory in the the current user home directory
- use dir command to list the content same as ls command but ls uses colors to differentiate between fils types and directories, dir list the content without any colors
- use touch to create a text file `touch file1` if file1 doesn't exit it will create it if it exit it will only update last access time (the time stamp) of file1 without changing its content.
- absolute path is when we write the full path from the start of inverted tree form the root file system / ex: `cd /home/imohamed , absolute path is a full path
- relative path is when we write a path relative to current working directory or parent working directory , we denote current working directory with a single dot . and parent working directory is denoted with double dots ..
- `cd ./..` means move from the current directory to the parent directory it is same as `cd ..` but we use `cd ./..` when we do shell scripting
- `cd ../..` means move to the parent's parent of the current directory.
- use `nano filename` to open a file and edit it` to save a file in nano program press ctrl+o
