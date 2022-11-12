## Basic permission part 2

- in last lecture, we took the symbolic method to deal with permissions.
- in this lecture, we will take the numeric method to deal with permissions.
- in numeric method r takes 4, w takes 2, and x takes 1. so, full permission is 7, r and w permission is 6, r and x permission is 5, and finally w and x permission is 3. Ex: giving the u as in user ,g as in group and o as in others the values 7 7 7 it means that they are taking full permission for each one.
- use the command `chmod 765 filename` that would give rwx rw- r-x permissions to the u g o type of users.
- use the command `chmod 000 filename` to give no permissions to any one.
- instead of using - and + to remove and add permissions we can set the permissions using = sign in that case whatever permissions a file has resetting the permission will be done. ex: `chmod ug=rw,o=rx filename` this command will reset the permissions and give the new stated permission after the = sign in the command'
- which is better to use numeric method or symbolic method? there is no better way to set your permissions as in numeric you have to set all permissions for all users types and in symbolic method you can set a permission to only one user type which is not possible in numeric method.
