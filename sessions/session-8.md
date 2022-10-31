## file system

- use command `tree` to show the current directory content as a tree
- use mkdir to create a directory. you can't name two directories with the same name. you can define the path to make directory to create directory on this path , without path it created in the same directory.
- use cp to copy a file from a file in the same directory or write the path to other directories `cp file1 file2 or cp file1 /tmp/file2`
- use cp to copy a directory to another direcory `cp direcory1/ directory2/` this won't work so use -r in the command `cp -r directory1/ directory2/`
- if the directory we are copying to a directory that has a dirctory with same name it takes only the content and it deoesnt create a new directory and if it is not exiting it makes a new directory `cp -r directroy1/ tmp/work/`
- to copy the directory with new name use the command `cp -r directory1/ tmp/report/`
- use mv to cut a directory from a directory and move it to another `mv dir1 /tmp/` with a new name us `mv dir1 /tmp/newdir'
- use rm to remove a file or directory `rm filenameorDirname` , use -r if the directory has files `rm -r dirName`
