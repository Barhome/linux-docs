## file system

- use command `tree` to show the current directory content as a tree , this command needs to be added on the system.
- use mkdir to create a directory. you can't name two directories with the same name. you can define the path to make directory to create directory on this path , without path it created in the same directory.
- use cp to copy a file with a new name in the same directory or write the path to other directories `cp file1 file2 or cp file1 /tmp/file2`
- use cp to copy a directory to another direcory `cp direcory1/ directory2/` this won't work as cp is used to copy files not directories so use -r in the command `cp -r directory1/ directory2/` it is like asking the command to copy the files inside of the directory
- if the directory we are copying to a directory that has a dirctory with same name it takes only the content and it doesnt create a new directory and if it is not exiting it makes a new directory `cp -r directroy1/ tmp/work/`
- to copy the directory with new name use the command `cp -r directory1/ tmp/NewDirName/`
- to view a file content use `cat filename`
- use mv to cut a directory from a directory and move it to another `mv dir1 /tmp/` with a new name us `mv dir1 /tmp/NewDirName'
- use rmdir to remove empty directory `rmdir filenameorDirname` , use rm to remove a file and with -r if you want to remove a directory has files `rm -r dirName` , -rf instead of -r to avoid the system to notifing you about every file , make sure not to leave a space between / and directory as this mean you want to delete the root file system / , note that in the new version no 7 you have to use --no-preserve-root if you want to remove / and this is a new update to avoid removing the root file system / accidentily.
- to rename a file there is no command to explicitly rename a file but you can use `mv oldfile newfilename`
