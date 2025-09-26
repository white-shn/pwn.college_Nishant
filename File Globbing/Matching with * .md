# Matching with *
Get in the /challenge directory with cd'ing but the argument to cd must be atmost 4 chracters , then run /challenge/run

## My solve
**Flag:** `pwn.college{IFPWldwv6fDhRKvSAQA2gXENKlf.QXxIDO0wSOzgjNzEzW}`

I tried cd'ing into the file directly but obviously failed and then I used cd and gave the argument to cd in 3 characters using globbing as "cd /c*" .<br>
After getting into the directory I executed /challenge/run to get the flag. 

```bash
hacker@globbing~matching-with-:~$ cd /challenge
You specified the path to 'cd' to in more than 4 characters. Disallowed!
This challenge resets your working directory to /home/hacker unless you change 
directory properly...
This challenge resets your working directory to /home/hacker unless you change 
directory properly...
hacker@globbing~matching-with-:~$ cd /c*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{IFPWldwv6fDhRKvSAQA2gXENKlf.QXxIDO0wSOzgjNzEzW}
hacker@globbing~matching-with-:/challenge$ 
```

## What I learned
Learned about first globe '*' , Whenever the shell encounter * character in any argument , the shell tries to replace it with any files that matches the pattern . <br>
When zero files are matched the shell leaves the glob unchanged.<br>
 * matches any part of the filename except for / or leading '.' character. 

## References 
None
