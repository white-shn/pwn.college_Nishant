## Redirecting more output
 Redirect the output of /challenge/run to myflag to get the flag . 

## My solve
**Flag:** `pwn.college{oEvTF4PNFKffPOrN20GIc3_bNbC.QX1YTN0wSOzgjNzEzW}`

I redirected the output of /challenge/run to the file myflag using '>'<br>
After this I read the ' myflag' file using cat command and got the flag.

```bash
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{oEvTF4PNFKffPOrN20GIc3_bNbC.QX1YTN0wSOzgjNzEzW}
```

## What I learned
Learned to redirect the output of any command to other files . 

## References
None
