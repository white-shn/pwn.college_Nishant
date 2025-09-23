# catting absolute paths
read the flag with cat command , using absolute path. 

## My solve
**Flag:** `pwn.college{UQzXh3QQEavxNNfgOf2xm_cGbtu.QX5ETO0wSOzgjNzEzW}`

Since the flag wasn't directly copied in the home directory, we had to use '/' , using the absolute path of the file to read it using cat command .
 ```bash
hacker@commands~catting-absolute-paths:~$ cat /flag
pwn.college{UQzXh3QQEavxNNfgOf2xm_cGbtu.QX5ETO0wSOzgjNzEzW}
```

## What I learned
Learned to use cat command and read a file by it's absolute path

## References 
None
