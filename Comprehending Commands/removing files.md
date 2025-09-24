# removing files 
delete the given file and execute /challenge/check to get the flag

## My solve
**Flag:** `pwn.college{0eLjonitR8zPL1itP66-RyLD16y.QX2kDM1wSOzgjNzEzW}`

Used ls to list the files in the home directory. <br>
Then used rm command to delete the specified file. <br>

```bash
hacker@commands~removing-files:~$ ls
delete_me  f  flag
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{0eLjonitR8zPL1itP66-RyLD16y.QX2kDM1wSOzgjNzEzW}
hacker@commands~removing-files:~$
```

## What I learned
Got familiar with rm command which is used to delete files . 

## References 
None
