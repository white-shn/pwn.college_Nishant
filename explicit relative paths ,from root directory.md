# explicit relative paths ,from /
run the program using . in the relative program

## My solve
**Flag:** `pwn.college{8gHzY0jC-TOdD8BY-sQEq_iSKmz.QXwUTN0wSOzgjNzEzW}`

First I directly executed the code to get the directory . 
After this , I got into the directory using the cd command .

'.' refers to the same directory and we had to use '.' in relative program . 
So the path would be './challenge/run'. Also since we're working in the root directory this relative path is also same as the absolute path.

```bash
hacker@paths~explicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{8gHzY0jC-TOdD8BY-sQEq_iSKmz.QXwUTN0wSOzgjNzEzW}
hacker@paths~explicit-relative-paths-from-:/$
```

## What I learned
Learned that every directory has two implicit entries that we can refernce path in '.' amd '..' . 
  
  . refers to the same directory so relative paths like /challenge , ././challenge , /challenge/. are identical .

  Relaive paths like ./challenge , ./././challenge , challenge/. are identical .  
  
  I learned how the implicit entry "." works . 

## References 
Slides in the video given in pwn.college 
