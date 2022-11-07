## user and group administration and permissions

- use `groupadd groupName` to create a group , know that users information are stored in /etc/passwd and the goups info are in /etc/group
- use `useradd -g dcadmins user1` to create a user called user1 and its primary group is dcadmins as -g means primary group
- use `usermod -G networkadmins user1` to add a user called user1 to his only one secondary group called networkadmins as -G means secondary group
- use `usermod -G -a dbadmins user1` to add a user called user1 to another secondary group called dbadmins and avoid kicking him from other secondary groups as we use -a option without -a the system removes all other secondary groups and adds only one secondary group mentioned in the
- know that when a file is created the ownership of this file will belong to the user who created it and to the primary group that this user belong to
- use `usermod -g groupname username` to modify the user's primary group
- run `cat /etc/passwd` to get the users information notice that the information is organized like username ,the password is denoted by x and it is hashed password stored in `cat /etc/shadow`, userid , primarygroup id run `cat /etc/group` to get group id and name , :: which represents GECOS that we consider it as a description and it is empty as we didn't put a description for the user when created, home directory, and /bin/bash the default shell terminal for the user as there are many shell terminals types and bin/bash is the default one the user uses and we will know why we use it later.
- in /etc/group information are like group name, x that represents hashed password for the group found in /etc/gshadow note that ! means that the password for the group is not set yet and group number.
- in /etc/gshadow information are like group name , hashed password , group admin and list of members in the group
- use `userdel username` to delete the user without deleting his home directory files and it also delete the default primary group which was automatically set to the user as we didn't pick a primary group for him and we used the default primary group if we set it the system can't delete the primary group and use `userdel -r username` to delete the user with his home directory files and his primary group , note that this will not delete the primary group for this user if it is attached to another user as its his primary group so you can't delete the primary group if it belongs to more than one user.
- use `groupdel groupname` this will delete any secondary group even if it belongs to 1000 user.
- when mentioning group only in any exam this means a secondary group.
