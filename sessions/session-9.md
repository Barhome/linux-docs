## Basic commands for file sys part two

- the general form of any command , `commandName [options] [arguments]` where [] means that this is optional and options changes the behavior of the command and arguments are is needed information that the command requires , ex: `ls` shows short listing without hidden files, `ls -l -a` shows long listing and hidden files
  `ls -r` show in reversed alphapatic order `ls -R` shows all the directories and the files inside them recursively which means the directories and the files inside.

- use ctrl+a to so the cursor moves to the begining of the command
- use ctrl+e to move it to the end of the command
- use ctrl+k to delete from where the cursor exist till the end
- use ctrl+u to delete from where the cursor exist till the beginning
- use ctrl+d to logout or the command `logout` or `exit` to logout the ssh session. t
- use ctrl+l or the command `clear` to clear the terminal and keep your commands up hidden in the terminal.
- use the command `reset` to clear the terminal completely .
- use shift+pgUP or shift+pgDn to move up and down
- use ctrl+z to stop the terminal loading temporarily and use `bg` to bring the loading job in the background again
- use ctrl+c to terminate the command and start new line or to end loading command resaults completely.
- use ctrl+s to lock your screen so that what your write doesn't show up and to show it and to unlock your screen use ctrl+q
- use command `reboot` or `shutdown -r now` or `systemctl reboot` or `init 6` to reboot your machine
- use command `shutdown -h now` or `systemctl poweroff` or `poweroff` or `init 0` to shudown the machine completely.
- use ; to write and execute two commands on the terminals

## users and groups

- once you create a user a group is created for him with the same name and it's the primary group for this user and no one else joins it(as administration preference offcousre a primary group can be set to many users) and it's called the private group for this user.
- use command `useradd ali` a user is created called ali and to check its id use `id ali` to get its id and its group id information for the private primary group and the other secondary groups he has joined as he can join only one private primary group and many secondary groups.
- this user is active but he needs a password use command `passwd ali` and do this with the root user as normal users can't change other users passwords.
- as a user use `passwd` to change your password.
