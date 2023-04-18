## Inodes and file systems

- It is really important to understand how the kernal deals with the files , how files are stored and retrieved, how to deal with different file systems and how to maintain them.
- The kernal deals with any thing with numbers, for example every user and group has a number and naming them is just a convention to facilitate them. The same thing happens with files. the kernal deals with files with numbers and these numbers represents these files.
- We need to know how data is stored and read in the desk, in our hard desk when we get a new one it is called raw desk or raw space which is like a whole one piece that needs to be divides. we divides the desk into MBR that stands for Master Boot Record and the rest are called partitions. the MBR is a piece of the desk that we use to manage the rest of the desk. MBR consist of three parts, the first part is the partition table to define where each partition starts and ends, it is like marks to separate partations. if we lost or corrupted the partation table then the desk becomes raw desk again. Each partition has a file system that we need to store and retrieve so the file system is the way to store and retrieve files from your hard desk like ntfs , fat32 , ext2, ext3, ext4, xfs , btrfs and many more. we use a file system depending on your business needs, example fat32 doesn't support big files more than 4 gigas for one block volume , doesn't support encryption and compression. one of the biggest feature in fat32 that is supported by natively by many operating systems.you can google each file system type to know its features and limitations.

- Why new file systems supports big sizes, Because of the use of unstructured data and the use of storing big data like video feeds.

- Each partition or files system needs inode table that the partition uses to know the data inside on it. by the use of inode tables that contains the files info where the file is stored in a block ex: the file x is stored in the block number this is called the meta data of the files and each partition has its own inode table .
- note that in inode table we have inodes, each inode refer to only one block. if we have a big file then many blocks are reserved and the first one is the inode number for this file and the rest are marked used.
- in inode table we store inforamtion about the files . the file that is stored could be a file or directory. the directory is a special type of file that points to other files.
- if we take an entry of a file we find that we have the inode numbers that shows the block number in which the file is stored, permissions, owner, access time , creation time , modificatin time and the link count.
- if we take an entry of a directory we have the same info of a file plus the name of the other files that the directory points to and their pointers so directories doesn't contains files but it has pointers to other files.
- note that each block by default has a size of 128 byte and we can change it when formatting.
- note that when changing the size of the blocks that affects the wasted size of a hard desk and the performance of our system if we want to store big files and small numbers of files we can enlarge the blocks, also if the file is small and the block is big, the rest of the block size will be wasted.
- note that the partition table has the partitions info like partitions number and block range for each partition.
- if inode table is corrupted it only affects its partiton not the whole desk.
- the kernal checks on the partition tables and then the partition or file system or inode table when we add a desk so then the kernal can access the data.
- note that each BMR has only one partition table and each partition has a file system or inode table.
- we need to make partition table if we have a new desk or we want to delete data by deleting the old partition table and create a new one.
- The process of creating files systems is called format which means if we have three partition we will need to format each one.
- in windows file system defragmentation process is rearrange parts of the files written on the distinct blocks on the desk to be on continuous blocks.
- in linux file systems the system does journaling process where it writes the files temperorly and then move it to final continuous blocks to avoid spreading files on distinct blocks. this journaling process is differes from file system to another.
- use the command `ls -li` to get inodes numbers for files`
- use `df` to get your partitions and you will get logical and virtual file systems , we will talk about virtual file systems later. this command show for the partition, the total number of blocks , used blocks , available blocks , used ratio and where it is mounted . -h means use human readable format for the previous info.
- use `df -i` to get the number of inodes for each file system.
