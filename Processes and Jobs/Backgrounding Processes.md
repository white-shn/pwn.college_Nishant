## Backgrounding Processes
Launch run , then suspend it , then background and launch another copy while the first is running in the background.

## My solve
**Flag:** `pwn.college{QHxjO0P3jSc6Lt6pmTrYaJaz03g.QX3QDO0wSOzgjNzEzW}`

Executed /challenge/run then suspended it using ctrl+Z, then resumed it in background with bg .<br>
Then relaunched it which gave me the flag.

```bash
hacker@processes~backgrounding-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!

UID          PID STAT CMD
root         159 S+   bash /challenge/run
root         161 R+   ps -o user=UID,pid,stat,cmd

I don't see a second me!

To pass this level, you need to suspend me, resume the suspended process in the
background, and then launch a new version of me! You can background me with
Ctrl-Z (and resume me in the background with 'bg') or, if you're not ready to
do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~backgrounding-processes:~$ bg
[1]+ /challenge/run &
hacker@processes~backgrounding-processes:~$


Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out.

hacker@processes~backgrounding-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!

UID          PID STAT CMD
root         159 S    bash /challenge/run
root         169 S    sleep 6h
root         170 S+   bash /challenge/run
root         172 R+   ps -o user=UID,pid,stat,cmd

Yay, I found another version of me running in the background! Here is the flag:
pwn.college{QHxjO0P3jSc6Lt6pmTrYaJaz03g.QX3QDO0wSOzgjNzEzW}
hacker@processes~backgrounding-processes:~$
```

## What I learned
Learned about bg command which is used to resume a process in background. 

## References

