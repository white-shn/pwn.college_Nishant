# making directories
create a directory and then a file in it . Then run /challenge/run to retrieve the flag 

## My solve
**Flag:** `pwn.college{04UMI9r04C2r9duczqDqUKr-F6-.QXxMDO0wSOzgjNzEzW}`

created the directory using mkdir then used cd to get in that directory . <br>
used touch to create the college file and then executed  /challenge/run to get the flag .

```bash
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ ls
college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{04UMI9r04C2r9duczqDqUKr-F6-.QXxMDO0wSOzgjNzEzW}
hacker@commands~making-directories:/tmp/pwn$
```

## What I learned
Learned to create directory using mkdir 

## References 
None
