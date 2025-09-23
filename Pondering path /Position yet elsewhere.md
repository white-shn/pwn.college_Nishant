# Position yet elsewhere
execute the /challenge/run program from a specific path

## My solve
**Flag:** `pwn.college{0j-apdewQgUHXLeLoAO51FyQad9.QX4QTN0wSOzgjNzEzW}`

I executed the /challenge/run program without getting in the 'specific directory' , it then showed incorrect and that I'm not in the directory specified .
I used the cd command to get in the directory then I did the rerunning of the '/challenge/run' program which gave me the flag for the challenge 
```bash
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/build-essential directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /usr/share/build-essential
hacker@paths~position-yet-elsewhere:/usr/share/build-essential$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{0j-apdewQgUHXLeLoAO51FyQad9.QX4QTN0wSOzgjNzEzW}
hacker@paths~position-yet-elsewhere:/usr/share/build-essential$
```

## What I learned
Learned to use the cd command which is used to navigate around directories . 
Learned to invoke a program which is in a specific directory by firstly getting in the directory using cd command and then executing the program by writing it's path . 

## References 
Slies of the video given in pwn.college



