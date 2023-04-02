## Accessing a system

- you can access a system through GUI or CLI
- if you don't have GUI, you will only have TTY stands for tele type terminal.
- you can access the machine through this TTY if you have physical access on the machine this is the terminal we use
- use Alt+CTRl+Fn where n= 1 is for accessing the GUI if you have GUI and from 2-6 is for accessing TTY 2 to TTY6 , and tty 1 is available if you don't have GUI
- we can use many TTY from 2 to 6 if the command is taking to long on TTY 2 we can move to another TTY 6
- to know in which tty you are using write command `tty`
- to move between ttys use ALT+Fn of TTY or use command `chvt 3` where chvt stands for change virtual terminal and 3 is the number of the tty you want to acces
- you can increase the number of TTYs

## User Types

- root is super user and user is a normal user
- every user has an id , root is zero, normal users have a range of numbers from 1000 and up
- use the command `id` to get a user id
- use the commands `date`
- use the command `cal` to see current month calender or `cal 9 2016` for a month in specific year and so on.
- use the command `su - username` to switch users su stands for switch user
- use the command `su -` or `su - root` to switch to root
- `exit` to exit current session and move to the previous session
- note that the system doesn't require the password for user with less priviliges so if you are in root session you can move to a user with less privilages without a password.
