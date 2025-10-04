## Starting Backgrounded Processes
Background /challenge/run without suspending it . 

## My solve
**Flag:** `pwn.college{IzD_829ld7kflieFe_9QUQRwmjP.QX5QDO0wSOzgjNzEzW}`

Backgrounded /challenge/run without suspending it by adding an ' a' to it .

```bash
hacker@processes~starting-backgrounded-processes:~$ /challenge/run &
[1] 161
hacker@processes~starting-backgrounded-processes:~$ 


Yay, you started me in the background! Because of that, this text will probably 
overlap weirdly with the shell prompt, but you're used to that by now...

Anyways! Here is your flag!
pwn.college{IzD_829ld7kflieFe_9QUQRwmjP.QX5QDO0wSOzgjNzEzW}
^C
[1]+  Done                    /challenge/run
hacker@processes~starting-backgrounded-processes:~$
```

## What I learned 
Learned to background a process without suspending it .

## References
None
