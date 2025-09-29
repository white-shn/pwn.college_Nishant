## Redirecting input
Redirect the PWN file to /challene/run and have the PWN file contain the value COLLEGE

## My solve
**Flag:** `pwn.college{MBydETNUGZQ2ZQF7qYAdP9qX68d.QXwcTN0wSOzgjNzEzW}`

I used the echo command to redirect the value 'COLLEGE' to the PWN file . Then I used input redirecting to redirect the PWN file to /challenge/run which gave me
the flag .
```bash
hacker@piping~redirecting-input:~$ echo PWN
PWN
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read 
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{MBydETNUGZQ2ZQF7qYAdP9qX68d.QXwcTN0wSOzgjNzEzW}
hacker@piping~redirecting-input:~$
```
## What I learned
Learned to redirect inputs to a program using ' <' 

## References
Resources in pwn.college
