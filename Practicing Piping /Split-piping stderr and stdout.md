## Split-piping stderr and stdout
/challenge/hack: this produces data on stdout and stderr
/challenge/the: you must redirect hack's stderr to this program
/challenge/planet: you must redirect hack's stdout to this program

## My solve
**Flag:** `pwn.college{URjggkm0qiKAVLC9igmg1kNoDME.QXxQDM2wSOzgjNzEzW}`

Used process substitution to redirect the stdout and stderr of /challenge/hack to /challenge/planet and /challenge/the respectively .<br>
I was trying to do piping but pipe only handles output so it didn't work . I used '>' for stdout and '2>' for stderr.<br>
Combining all this give me the flag for the challenge.

```bash
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack | tee 2>(/challenge/the) >(/challenge/planet)
tee: 2/dev/fd/63: No such file or directory
This secret data must directly make it to /challenge/planet over my stdout.
Don't try to copy-paste it; it changes too fast.
28401205891665012089
You must redirect my standard error into '/challenge/the'!
Are you sure you're properly redirecting /challenge/hack's standard error into
'/challenge/the'?
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack  2>(/challenge/the) >(/challenge/planet)
It looks like you passed something like '>(something)' as an *argument* to
/challenge/hack rather than redirecting /challenge/hack's out/error to
'>(something)'. Remember, 'cmd1 >(cmd2)' does *NOT* redirect output of cmd1;
rather, it'll run cmd2, hook a file up to its standard input, and pass that
file as an argument to cmd1. If you want to redirect cmd1's output into that
file, you will need to do: 'cmd1 > >(cmd2)', which is equivalent to 'cmd1 |
cmd2'.
You must redirect my standard output into '/challenge/planet'!
You must redirect my standard error into '/challenge/the'!
Are you sure you're properly redirecting /challenge/hack's standard output into
'/challenge/planet'?
Are you sure you're properly redirecting /challenge/hack's standard error into
'/challenge/the'?
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack  2> >(/challenge/the) > >(/challenge/planet)
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{URjggkm0qiKAVLC9igmg1kNoDME.QXxQDM2wSOzgjNzEzW}
hacker@piping~split-piping-stderr-and-stdout:~$
```

## What I learned 
Learned to redirect stdout and stderr of a command to two command simultaneously . 

## References
None
