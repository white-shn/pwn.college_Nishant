# Position elsewhere
execute the /challenge/run program from a specific path

## My solve
**Flag:** `pwn.college{QbsvhXiI0gijtXwILSeVhayPGbs.QX3QTN0wSOzgjNzEzW}`

Firstly I used the pwd command to get my current working directory which I got as /home.
Then using cd command I get in the directory .(cd /home)
After this I write the path of the program to execute it . (/challenge/run)

```bash
hacker@paths~position-elsewhere:~$ pwd
/home/hacker
hacker@paths~position-elsewhere:~$ cd /home
hacker@paths~position-elsewhere:/home$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{QbsvhXiI0gijtXwILSeVhayPGbs.QX3QTN0wSOzgjNzEzW}
hacker@paths~position-elsewhere:/home$

```

## What I learned
I learned that using pwd you can view you current working directory .
I got familiar with the cd command which i used to get in the directory in which the /challenge/run program was there . 
I got familiar with writing the path of a program to execute it .
## References 
Slies of the video in pwn.college
