# Program and aboslute paths
To invoke the run program in challenge directory .

## My solve
**Flag:** `pwn.college{UPlFOFLNwAjHG9PW3xEyu5CWN5I.QX1QTN0wSOzgjNzEzW}`

In this challenge , we had to invoke the run program in challenge directory and the challegene directory is in the root directory . 
To inovke a program we need to write it's path. The path to challenge directory is '/challenge'
The path to run program is '/challenge/run' because the program is in the challenge directory . 
When you press enter , you'll get the flag .

```bash
hacker@paths~program-and-absolute-paths:~$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{UPlFOFLNwAjHG9PW3xEyu5CWN5I.QX1QTN0wSOzgjNzEzW}
hacker@paths~program-and-absolute-paths:~$
```

## What I learned
Invoke a program in a directory . To invoke the program we need to write it's path. 
In this program we executed the run program which is in the challenge directory(the challenge directory is in root directory) by writing it's path which is '/challenge/run' . 

## References 
Slies of the video in pwn.college
