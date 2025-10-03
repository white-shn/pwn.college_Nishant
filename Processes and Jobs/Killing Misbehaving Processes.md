## Killing Misbehaving Processes
Kill /challenge/decoy and get the flag from /challene/run

## My solve
**Flag:** `pwn.college{cBAwpM8uLk4DVKDM5A0RmIQ5vNP.0FNzMDOxwSOzgjNzEzW}`

Listed the running processes using ps -ef , killed /challenge/decoy by kill command , then executed /challenge/run and used cat command to read /tmp/flag_fifo.

```bash
hacker@processes~killing-misbehaving-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 22:25 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-init /run/dojo/bin/sleep 6h
root           7       1  0 22:25 ?        00:00:00 /run/dojo/bin/sleep 6h
root         137       1  0 22:25 ?        00:00:00 /bin/bash /challenge/.init
root         138       1  0 22:25 ?        00:00:00 /bin/bash /challenge/.init
root         139       1  0 22:25 ?        00:00:00 su -c exec /challenge/decoy > /tmp/flag_fifo hacker
root         140     137  0 22:25 ?        00:00:00 sleep 6h
root         141     138  0 22:25 ?        00:00:00 sleep 6h
hacker       142     139  0 22:25 ?        00:00:00 /usr/bin/python /challenge/decoy
hacker       144       0  0 22:25 pts/0    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/bin/bash /run/dojo/bin/ssh
hacker       150     144  0 22:25 pts/0    00:00:00 /run/dojo/bin/bash --login
hacker       168       1  0 22:25 ?        00:00:00 /nix/store/g0q8n7xfjp7znj41hcgrq893a9m0i474-ttyd-1.7.7/bin/ttyd --port 7681 --interface 0.0.0.
hacker       172     168  0 22:25 pts/1    00:00:00 /run/dojo/bin/bash --login
hacker       182     172  0 22:25 pts/1    00:00:00 ps -ef
hacker@processes~killing-misbehaving-processes:~$ kill 142
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!
hacker@processes~killing-misbehaving-processes:~$ cat /tmp/flag_fifo
pwn.college{cBAwpM8uLk4DVKDM5A0RmIQ5vNP.0FNzMDOxwSOzgjNzEzW}
hacker@processes~killing-misbehaving-processes:~$
```

## What I learned
It was a practice challenge

## References
None


