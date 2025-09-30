## Duplicating piped data with tee
 /challenge/pwn must be piped into /challenge/college, but you'll need to intercept the data to see what pwn needs from you

## My solve
**Flag:** `pwn.college{cR_rWy45Tqnx5LbKq_Y0p4L_8yJ.QXxITO0wSOzgjNzEzW}`

Using the tee command I duplicated the data flowing to the output file. I to pipe the output of /challenge/pwn in /challenge/college. <br>
Then used cat to read the output file , which gave me the usage , and the SECRET_ARG which I had to use to get the flag.

```bash
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee /challenge/college
Processing...
You are trying to use 'tee' *instead* of /challenge/college. Use it *between* 
/challenge/pwn and /challenge/college!
You must pipe the output of /challenge/pwn into /challenge/college (or 'tee' 
for debugging).
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee output | /challenge/college
Processing...
The input to 'college' does not contain the correct secret code! This code 
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the 
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat output
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "cR_rWy45"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret cR_rWy45 | tee output | /challenge/college
Processing...
WARNING: you are overwriting file output with tee's output...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{cR_rWy45Tqnx5LbKq_Y0p4L_8yJ.QXxITO0wSOzgjNzEzW}
hacker@piping~duplicating-piped-data-with-tee:~$
```

## What I learned
Leanred about the tee command which duplicates the data flowing through the pipes to any number of files you provide
## References 
Resources given in pwn.college 

