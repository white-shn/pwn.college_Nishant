## Resuming Processes
Suspend run and then resume it to get the flag. 

## My solve
**Flag:** `pwn.college{E4UQGZJRvjlpLSdKwrX25LmJxKQ.QX2QDO0wSOzgjNzEzW}` 

Executed /challenge/run, then suspended it with crtl + Z ,  then resumed it with fg command ,which gave me the flag for the challenge.

```bash
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg
/challenge/run
I'm back! Here's your flag:
pwn.college{E4UQGZJRvjlpLSdKwrX25LmJxKQ.QX2QDO0wSOzgjNzEzW}
Don't forget to press Enter to quit me!

Goodbye!
hacker@processes~resuming-processes:~$
```

## What I learned
Learned about fg command which is used to resume a suspended process. 


## References
None
