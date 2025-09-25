# Learning Complex Usage
pass the --printfile argument which prints the argument to it , to /challenge/challenge.

## My solve
**Flag:** `pwn.college{wCQTsxNEaJh7Sl3ZZqi0dbq2A7g.QX1ITO0wSOzgjNzEzW}`

Cd'ing into the root directory ,then listing the files . <br>
Get the name of the file with flag and use the /challenge/challenge with --printfile argument . 
Pass the file as argument to the /challenge/challenge --printfile . 
This will print the flag 

```bash
hacker@man~learning-complex-usage:~$ cd /
hacker@man~learning-complex-usage:/$
hacker@man~learning-complex-usage:/$ ls
bin   challenge  etc   home  lib32  libx32  mnt  opt   root  sbin  sys  usr
boot  dev        flag  lib   lib64  media   nix  proc  run   srv   tmp  var
hacker@man~learning-complex-usage:/$ /challenge/challenge --printfil  /flag
Incorrect usage! You passed the wrong argument (read the challenge description
for details).
hacker@man~learning-complex-usage:/$ /challenge/challenge --printfile /flag
Correct argument! Here is the /flag file:
pwn.college{wCQTsxNEaJh7Sl3ZZqi0dbq2A7g.QX1ITO0wSOzgjNzEzW}
hacker@man~learning-complex-usage:/$
```

## What I learned
Learned about giving arguments to argument.



## References 
None
