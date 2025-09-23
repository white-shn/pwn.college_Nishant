# Position elsewhere
execute the /challenge/run program from a specific path

## My solve
**Flag:** `pwn.college{QbsvhXiI0gijtXwILSeVhayPGbs.QX3QTN0wSOzgjNzEzW}`

Firstly I executed the /challenge/run program without getting in the specified directory which helped me get the name of the specified directory.

Then using cd command I get in the directory .(cd /home)

After this I write the path of the program to execute it . (/challenge/run)

```bash
/cjuahacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /home directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /home
hacker@paths~position-elsewhere:/home$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{QbsvhXiI0gijtXwILSeVhayPGbs.QX3QTN0wSOzgjNzEzW}
hacker@paths~position-elsewhere:/home$
```

## What I learned
Got to know that the directory in which a particular program is stored is executed by writing it's path. 

I got familiar with the cd command which i used to get in the directory in which the /challenge/run program was there . 

I got familiar with writing the path of a program to executing it .

## References 
Slies of the video in pwn.college
