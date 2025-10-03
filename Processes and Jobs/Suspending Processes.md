## Suspending Processes
Suspend /challenge/run o get the flag

## My solve
**Flag:** `pwn.college{8M_o-TnjpT1yCpgSqOvR8Okss00.QX1QDO0wSOzgjNzEzW}`
 
Executed /challenge/run which told me to susped it using ctrl +Z , which resulted in the process getting supended.<br>
Then launch /challenge/run which is a copy which will give you the flag .

```bash
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         176     143  0 22:31 pts/1    00:00:00 bash /challenge/run
root         178     176  0 22:31 pts/1    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         176     143  0 22:31 pts/1    00:00:00 bash /challenge/run
root         183     143  0 22:31 pts/1    00:00:00 bash /challenge/run
root         185     183  0 22:31 pts/1    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{8M_o-TnjpT1yCpgSqOvR8Okss00.QX1QDO0wSOzgjNzEzW}
hacker@processes~suspending-processes:~$
```

## What I learned 
Learned to suspend a process

## References
None
