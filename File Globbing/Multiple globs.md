# Multiple globs
run /challenge/run after getting into /challenge/files , provinding single argument of 3 characters such that it cover every word that contains letter 'p'.

## My solve
**Flag:** `pwn.college{8Breq9odzlYxjI_87XPrCfMllAm.0lM3kjNxwSOzgjNzEzW}`

I went in the /challenge/files directory using cd, then I executed the /challenge/run command with proper argument such that it covers all the words that contain the 
letter 'p' in them. Also I could only use  3 characters with two * globe. <br>
We know that * match multiple character so I used it before p and after p so that the entire word can be matched , so my argument was " *p* "
The final command I executed was " /challenge/run *p* " which gave me the flag . 

```bash
hacker@globbing~multiple-globs:~$ cd /challenge/files
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run /challenge/files/*p*
Error: your argument is too long! It must be 3 characters or less.
hacker@globbing~multiple-globs:/challenge/files$ /challegne/run *p*
bash: /challegne/run: No such file or directory
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run *p*
You got it! Here is your flag!
pwn.college{8Breq9odzlYxjI_87XPrCfMllAm.0lM3kjNxwSOzgjNzEzW}
```
## What I learned
Learned to use multiple globs at once , for ex : /*f* , for this argument the shell will look for every file that have a f in it . 

## References
None
