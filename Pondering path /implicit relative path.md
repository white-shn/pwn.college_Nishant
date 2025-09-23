# Implicit relative path
explicitly use relative paths to launch run

## My solve
**Flag:** `pwn.college{IWLvOlIiBgBZ_w83gmUBUB6lxWN.QXxUTN0wSOzgjNzEzW}`

Get in the '/challenge' directory using cd . 
To launch run explicity using relative paths we will use '.' 
The relative path for run program will be ' ./run ' then press enter and you'll get the flag 

```bash
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{IWLvOlIiBgBZ_w83gmUBUB6lxWN.QXxUTN0wSOzgjNzEzW}
hacker@paths~implicit-relative-path:/challenge$

```

## What I learned
Got familiar using relative paths explicitly to launch a program . 

## References 
Slides of the video in pwn.college
