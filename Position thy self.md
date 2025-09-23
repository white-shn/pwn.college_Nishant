# Position thy self
To execute the /challenge/run program from a specific path.

## My solve
**Flag:** `pwn.college{MBFLV0jmgJAwJQDAww6GjSWSnFK.QX2QTN0wSOzgjNzEzW}`

To get the specific directory in which I had to execute the program , I executed the program without getting in the directory which gave me the specific directory in which the entire program was stored .

After getting the directory name , get in the directory by 'cd /var/log' .
Then execute '/challenge/run' and you'll get the flag

```bash
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /var/log directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /var/log
hacker@paths~position-thy-self:/var/log$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{MBFLV0jmgJAwJQDAww6GjSWSnFK.QX2QTN0wSOzgjNzEzW}
hacker@paths~position-thy-self:/var/log$
```

## What I learned
I learned to navigate through directories using the cd(change directory) command and passing a path to it as an argument. 

Also i learned that if u execute a program without getting in the specific directory it won't run and tell you that you're not in the specific directory.

We need to get in that directory using cd command and then execute the program.


## References 
Slies of the videos in pwn.college
