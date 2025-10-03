## Killing Processes
Find the dont_run process and kill it to run /challenge/run

## My solve
**Flag:** `pwn.college{Y9K_FeJNl_BzLypKbwvFS3aER_5.QXyQDO0wSOzgjNzEzW}`

Use ps command to list the running process and get the dont_run process and kill it using the kill command with the argument as the PID of the dont_run process.<br>
Next run the /challenge/run command and you'll get the flag.

```bash
hacker@processes~killing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 20:57 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-init /run/dojo/bin/sleep 6h
root           7       1  0 20:57 ?        00:00:00 /run/dojo/bin/sleep 6h
root         135       1  0 20:57 ?        00:00:00 su -c /challenge/.launcher hacker
hacker       136     135  0 20:57 ?        00:00:00 /challenge/dont_run
hacker       137     136  0 20:57 ?        00:00:00 sleep 6h
hacker       148       1  0 20:57 ?        00:00:00 /nix/store/g0q8n7xfjp7znj41hcgrq893a9m0i474-ttyd-1.7.7/bin/ttyd --port 7681 --interface 0.0.0.
hacker       150     148  0 20:57 pts/0    00:00:00 /run/dojo/bin/bash --login
hacker       160     150  0 20:57 pts/0    00:00:00 ps -ef
hacker@processes~killing-processes:~$ kill 136
hacker@processes~killing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 20:57 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-init /run/dojo/bin/sleep 6h
root           7       1  0 20:57 ?        00:00:00 /run/dojo/bin/sleep 6h
hacker       137       1  0 20:57 ?        00:00:00 sleep 6h
hacker       148       1  0 20:57 ?        00:00:00 /nix/store/g0q8n7xfjp7znj41hcgrq893a9m0i474-ttyd-1.7.7/bin/ttyd --port 7681 --interface 0.0.0.
hacker       150     148  0 20:57 pts/0    00:00:00 /run/dojo/bin/bash --login
hacker       162     150  0 20:58 pts/0    00:00:00 ps -ef
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{Y9K_FeJNl_BzLypKbwvFS3aER_5.QXyQDO0wSOzgjNzEzW}
hacker@processes~killing-processes:~$
```

## What I learned
Learned to use the kill command which is used to terminate a process running on your terminal. 

## References
None
```
