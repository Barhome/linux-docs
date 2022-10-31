## Some useful commands

- use `eject` to open your cd room and `eject -t` to close it
- use `ls` to view your files on the current directory

## Types of users

- root and its id is zero
- normal users their id > =1000
- system users or services users 0 < id < 1000 from 1 to 999 that is in the new release ,previously on old releases 6 release and before was between 1 to 499 , if we have a web server with root privilidges and if there is an attack on this service the attacker will get root privilidges and this is a big crisis. so, to solve this issue, we create a dummy user for the service, and give this user priviliges for only the files of the service. note that the service doesnt get an id but the each service gets a user with specific priviledges. also note that all users are stored in /etc/password

## The file system

- in linux directories are organized in a certain way it is like an inverted tree , the first main directory is called root file system / slash and it represent the begining of the file system and it doesn't really exit and the operating system operates the files of the system from this directory, under this / we get the operating system directories like home , var , etc , dev, temp , users and many more and under each of these direcotries there is sub directories
- in home we get sub directories home directories of the users where they keep their files and work, each directory for a user.
- in etc , in which all configration of the system is stored. ex: configration file for the user or the sound card and many more services where their configration files and configration directories are stored.
- note there is a rule in linux that everything is a file. ex: hard disk, partition , sound card is a file.
- in dev directory is stands for devices and every device is a file and if the os wants to access a device it access from this directory.
- in tmp where temparatory files are saved and the application save these files in this directory temporatory. ex: if you are watching a movie on youtube stream is saved in this directory to be diplayed. this stream is saved temperatory. you can set the temp period to remove saved files and to clean up. we will do that later in the course.
- in usr is short name for users. in any on os there are shared files for the users. and they are kept here. ex: to keep shared themes, fonts, help files and many more.
- in bin is for binaries or apps , note that commands like ls , date, and many other programs are considered binaries or apps that are kept in bin, note that these binaries can be accessable by all users.
- in sbin is for super user binaries , the super user is root and these binaries or commands for root user these are adminstrative commands.
- in var we keep variable files and things that always change and updates , ex: log files, emails , databases as they always have data that change.
- in root directory, root user is a special user and it has a home directory called root , in this root folder you can find files that keep passwords for the users or the services.
- in proc directory it is also called virtual file system, note that kernal while processing it keeps information about the your system and your machine hardware and information your running application and it is kept in this director . ex: cpu info file keeps all the info that the kernal know about the processer as a hard. as the os deals with the user with their id no. the kernal also deals with all the services and the processes with their id and these numbers are kept in the proc. Note that proc doesn't exit in real if restart your machine everything inside this proc will be removed. you can read only the file in proc.
- in opt directory, if you open it it is empty. it is used by some application vendors they like to separate their application installation to be done in this folder to make things easy and avoid complication when the user likes to uninstall the application.
- in srv directory, it is an empty directory too that is used by you to install future services in it that has big files if you like so. ex: if you want to install the apatchi with virtual hosting and you will have many website and evety website will have its own files and these files are kept in directory for this website in the srv directory.
- in media "mount check if it is the same as mount "directory, if you add a flash card or external hard disk, and a drive name is assigned to it this process is called mounting and this flash card or external hard disk in the media directory. so it is used for removable media
- in mnt is like media but for floppy desk.
- in boot directory, where the kernal and boot loader are kept, the boot loader allows you to boot the os or the kernal. so boot files that you need for booting like kernal and boot loader are kept in this directory.
- note that you have a root user with id 0 and root file system which is the / and root directory which is the home directory for the root.
- in lib directory, it is where libraries saved and kept so application can use them. lib is for 32bit os and lib64 is for 64bit os. note that 64bit os can use lib64 and lib but 32bit os don't have lib64 and can't use it.
- in sys directory , kernal uses it to save info about the device hardware only , you will know more about it in the future.
-
