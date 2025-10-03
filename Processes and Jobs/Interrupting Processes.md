## Interrupting Processes
Interrupt /challenge/run to get the flag. 

## My solve
**Flag:** `pwn.college{8ZbN15GaZbHy49SkHlTdlI7x3aQ.QXzQDO0wSOzgjNzEzW}`

I executed  /challenge/run but it obviously didn't give me the flag without geting interrupted, so I used ctrl+ c to interrupt it and got the flag.

```bash
hacker@processes~interrupting-processes:~$ /challenge/run
I could give you the flag... but I won't, until this process exits. Remember,
you can force me to exit with Ctrl-C. Try it now!
^C
Good job! You have used Ctrl-C to interrupt this process! Here is your flag:
pwn.college{8ZbN15GaZbHy49SkHlTdlI7x3aQ.QXzQDO0wSOzgjNzEzW}
hacker@processes~interrupting-processes:~$
```

## What I learned 
Learned to interrupt a process .<br>
Ctrl+C sends an "interrupt" to whatever application is waiting on input from the terminal and 
this causes the application to cleanly exit.

## References 
None
