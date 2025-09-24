# Touching files 
create two files using touch and then invoke /challenge/run to get the flag.

## My solve
**Flag:** `pwn.college{wFNQRvB9jZ7tO-9od1v6mBfQqkP.QXwMDO0wSOzgjNzEzW}`


Used touch to create the two files given and then executed /challenge/run

```bash
hacker@commands~touching-files:~$ touch /tmp/pwn
hacker@commands~touching-files:~$ /challenge/run
Uh oh! /tmp/college does not exist. Please use the 'touch' command to create it!
hacker@commands~touching-files:~$ touch /tmp/college
hacker@commands~touching-files:~$ /challenge/run
Success! Here is your flag:
pwn.college{wFNQRvB9jZ7tO-9od1v6mBfQqkP.QXwMDO0wSOzgjNzEzW}
hacker@commands~touching-files:~$

```

## What I learned
Learned about the touch command which is used to create new empty files .


## References 
none
