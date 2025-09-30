## Named pipes
Create a name pipe and redirect the output of /challenge/run to it and then cat the fifo .

## My solve
**Flag:** `pwn.college{wwf9rCB00A3jeoSoShwV-MkgLPo.01MzMDOxwSOzgjNzEzW}`


```bash
hacker@piping~named-pipes:~$ mkfifo /tmp/flag_fifo
hacker@piping~named-pipes:~$ /challenge/run > /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo! 
Bash will now try to open the FIFO for writing, to pass it as the stdout of 
/challenge/run. Recall that operations on FIFOs will *block* until both the 
read side and the write side is open, so /challenge/run will not actually be 
launched until you start reading from the FIFO!
^C
hacker@piping~named-pipes:~$ cat /tmp/flag_fifo
You've correctly redirected /challenge/run's stdout to a FIFO at 
/tmp/flag_fifo! Here is your flag:
pwn.college{wwf9rCB00A3jeoSoShwV-MkgLPo.01MzMDOxwSOzgjNzEzW}
hacker@piping~named-pipes:~$
```

## What I learned 
Learned about FIFO ,which are named pipes created by user . <br>
Unlike the automatic named pipes from process substitution we can control where the FIFO is created and they stay until you delete them and you can see them 
with ls and examine them like files.<br>
One problem with FIFOs is that they "block" any operations on them until both the read side of the pipe and the write side of the pipe are ready. 
