# The Root
Invoke the the pwn program in /(root directory)

## My solve
**Flag:** `pwn.college{sK8Zp51QiV_iNgLH28q2HSziVdu.QX4cTO0wSOzgjNzEzW}`

we have to invoke the pwn programm in the root direectly and we can do that by providing it's path ,
The path will be '/pwn' . Press enter and you'll get the flag.
This type of path starting with the root directory is called absolute path.
```bash
hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{sK8Zp51QiV_iNgLH28q2HSziVdu.QX4cTO0wSOzgjNzEzW}
hacker@paths~the-root:~$
```

## What I learned
I learned about how directories are stored in another directory and the largest directory is the root directory .
I learned to invoke a program under a directory by provinding it's path, in this case '/pwn'. 
The path that starts with the root directory is called the absoulte path. 


## References 
The slides of the video in pwn.college
