## Redirecting Errors
redirect the output of /challenge/run to myflag, and the "errors" (in our case, the instructions) to instructions.

## My solve
**Flag:** `pwn.college{ck47Qg6SimGC3hhu68hmdPbXUlw.QX3YTN0wSOzgjNzEzW}`

I redirected the output of /challenge/run to myflag using '>' which redirects FD 1(Standard output) and the instructions to the file ' instructions' by ' 2>' which 
will redirect FD 2(Standard error).  Next using cat command read both the files and you'll get the instructions as well as the flag.
```bash
hacker@piping~redirecting-errors:~$ /challenge/run > myflag 2> instructions
hacker@piping~redirecting-errors:~$ ls /home/hacker
COLLEGE  a  catflag  file  flag  instructions  link  myflag  not-the-flag  not_the_flag  our  pwn  the-flag
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{ck47Qg6SimGC3hhu68hmdPbXUlw.QX3YTN0wSOzgjNzEzW}

hacker@piping~redirecting-errors:~$ cat instructions
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will check that error output is redirected to a specific file path : instructions
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!

[TEST] You should have redirected my stderr to instructions. Checking...

[PASS] The file at the other end of my stderr looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-errors:~$ 
```

## What I learned 
Learned to redirect error of commands .<br>
Learned about  File Descriptor (FD) which is a number that describes a communication channel in Linux.
FD 0: Standard Input<br>
FD 1: Standard Output<br>
FD 2: Standard Error<br>
A '>' without any number implies ' 1>' . <br>

                                        
