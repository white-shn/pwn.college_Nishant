## Processes and Jobs


## My solve
**Flag:** `pwn.college{s0loU5to-lTmv9I9Y61fRfBm0RZ.QX4MDO0wSOzgjNzEzW}`

The challenge command was already running so I used the ps -ef command to get the list of processes running which helped me get the name of challeng command<br>
Then I executed the challenge command to get the flag .

```bash
hacker@processes~listing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 18:47 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-init /run/dojo/bin/sleep 6h
root           7       1  0 18:47 ?        00:00:00 /run/dojo/bin/sleep 6h
root         132       1  0 18:47 ?        00:00:00 /challenge/10180-run-28270
root         135     132  0 18:47 ?        00:00:00 sleep 6h
hacker       146       1  0 18:47 ?        00:00:00 /nix/store/g0q8n7xfjp7znj41hcgrq893a9m0i474-ttyd-1.7.7/bin/ttyd --port 7681 --interface 0.0.0.
hacker       150     146  0 18:47 pts/0    00:00:00 /run/dojo/bin/bash --login
hacker       160     150  0 18:47 pts/0    00:00:00 ps -ef
hacker@processes~listing-processes:~$ /challenge/10180-run-28270
Yahaha, you found me! Here is your flag:
pwn.college{s0loU5to-lTmv9I9Y61fRfBm0RZ.QX4MDO0wSOzgjNzEzW}
Now I will sleep for a while (so that you could find me with 'ps').
```

## What I learned
Learned about the ps command which lists the process running in your terminal.<br>
We can use -e to list "every" process and -f for a "full format" output, including arguments. These can be combined into a single argument -ef.<br>
We use a to list processes for all users, x to list processes that aren't running in a terminal, and u for a "user-readable" output. 
These can be combined into a single argument aux.

##  References 
None
