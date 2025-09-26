## Help for Builtins 
Using help on challenge command which is a shell builtin, rather than a program to get the flag

## My solve
**Flag:** `pwn.college{49BRKYc36LbZ-8xYYRShU7s-pMH.QX0ETO0wSOzgjNzEzW}`

I used 'help challenge' which gave me some arguments, " --secret VALUE " which prints the flag , and it also gave me the value to provide to --secret. <br>
Then invoked /challenge with the --secret argument and the proper value , which gave me the flag for the challenge.
```bash
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "49BRKYc3".
hacker@man~help-for-builtins:~$ /challenge --secret 49BRKYc3
bash: /challenge: Is a directory
hacker@man~help-for-builtins:~$ challenge --secret 49BRKYc3
Correct! Here is your flag!
pwn.college{49BRKYc36LbZ-8xYYRShU7s-pMH.QX0ETO0wSOzgjNzEzW}

hacker@man~help-for-builtins:~$

```

## What I learned
Builtins are commands which rather than being programs with man pages and help options, are built into the shell itself.<br>
Builtins are inovked just like commmands but insted of launching other programs , the shell handles them internally .<br>
Using help builtin can help us get help on a builtin which in this challenge helped me get the flag. 

## References 
None
