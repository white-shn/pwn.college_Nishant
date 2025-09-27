## Redirecting output
Use output redirection to write the word PWN to filename COLLEGE.

## My solve
**Flag:** `pwn.college{c29zur4AMWr30uO59wZQYe1TYFa.QX0YTN0wSOzgjNzEzW}`

I used the echo command with the help of ' >' to redirect the ouput of echo PWN in the COLLEGE.

```bash
hacker@piping~redirecting-output:~$ echo PWN > COLLEGE
Correct! You successfully redirected 'PWN' to the file 'COLLEGE'! Here is your 
flag:
pwn.college{c29zur4AMWr30uO59wZQYe1TYFa.QX0YTN0wSOzgjNzEzW}
hacker@piping~redirecting-output:~$ cat COLLEGE
PWN
```

## What I learned
Learned to redirect standard output to files using '>'

## References
The resources given in pwn.college website.
