## Grepping live output 
/challenge/run contains a lot of  text including the flag . Grep the flag.

## My solve
**Flag:** `pwn.college{I8gelCGyMPClJVE93P6Xh9IdTwB.QX5EDO0wSOzgjNzEzW}`

This time , unlike the previous challenges , I didn't store the output in some file and then grepped it. Instead I used '|' (pipe) operator to connect the standard 
output from /challenge/run with the stdin of grep pwn.college .  This is how I got the flag for this challenge.

```bash
hacker@piping~grepping-live-output:~$ /challenge/run | grep pwn.college
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stdout : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/8b4vn1iyn6kqiisjvlmv67d1c0p3j6wj-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stdout!
[PASS] Success! You have satisfied all execution requirements.
pwn.college{I8gelCGyMPClJVE93P6Xh9IdTwB.QX5EDO0wSOzgjNzEzW}
hacker@piping~grepping-live-output:~$
```

## What I learned 
Learned about the pipe(|) operator which is used to connect the stdout of command to the left of pipe to the stdin of the command to the right of the pipe.<br>
Pipe is not considered a Redirect Operator but rather a Control Operator,
while pipe is used to redirect output not all control operators have this function.
## References
Resources given in pwn.college 
