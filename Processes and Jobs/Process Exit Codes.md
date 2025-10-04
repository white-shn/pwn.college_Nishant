## Process Exit Codes
Retrieve the exit code returned by /challenge/get-code and then run /challenge/submit-code with that error code as an argument

## My solve
**Flag:** `pwn.college{o_ZIR3M8PlNP6fyaoGBWTTjzLMX.QX5YDO1wSOzgjNzEzW}`

Execute /challenge/get-code then echo $? to get the error code , then use that error code as an argument with /challenge/submit-code to get the flag .

```bash
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
56
hacker@processes~process-exit-codes:~$ /challenge/submit-code 56
CORRECT! Here is your flag:
pwn.college{o_ZIR3M8PlNP6fyaoGBWTTjzLMX.QX5YDO1wSOzgjNzEzW}
hacker@processes~process-exit-codes:~$
```

## What I learnd 
Learnd about ? which helps us get the exit code for a proceess,commands that succeed typically return 0 and commands that fail typically return a non-zero value.

## References
None
