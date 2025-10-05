## Becoming root with su
 provide the password to su to become root.

 ## Mysolve
 **Flag:** ` pwn.college{AUDV3_LYIyRESzZMXNmxWSemptG.QX1UDN1wSOzgjNzEzW}` 

 Used su (the substitute user command) and entered the root passoword to become the root .

 ```bash
hacker@users~becoming-root-with-su:~$ su
Password: 
su: Authentication failure
hacker@users~becoming-root-with-su:~$ su
Password: 
root@users~becoming-root-with-su:/home/hacker# cat flag
cat: flag: No such file or directory
root@users~becoming-root-with-su:/home/hacker# cat /flag
pwn.college{AUDV3_LYIyRESzZMXNmxWSemptG.QX1UDN1wSOzgjNzEzW}
root@users~becoming-root-with-su:/home/hacker#
 ```

## What I learned
Learned about the 2 commands(su and sudo) used to access root access of a system.<br>
For this challenge we used `su` which is the outdated one. 

## References
None
