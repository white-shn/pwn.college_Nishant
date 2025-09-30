## Writing to multiple programs
Run the /challenge/hack command, and duplicate its output as input to both the /challenge/the and the /challenge/planet commands

## My solve
**Flag:** `pwn.college{w5vOauscwkylnWBQ6LYOmtcWmeV.QXwgDN1wSOzgjNzEzW}`

I duplicated the output of /challenge/hack to /challenge/the and /challenge/planet as input. <br>
Used tee and '>' to dulpicate the output of the command, as input to the two commands. 

```bash
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
32585208721898132308
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
2939739951498820572
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{w5vOauscwkylnWBQ6LYOmtcWmeV.QXwgDN1wSOzgjNzEzW}
hacker@piping~writing-to-multiple-programs:~$
```

## What I learned 
Learned to use tee and '>' to get the output of a command as an input to other commands.

## References 
None
