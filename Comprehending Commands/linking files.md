# linking files
Using symlink  

## My solve
**Flag:** `pwn.college{8z-ZBwWahjyiaiAzVtWh-pOSJVk.QX5ETN1wSOzgjNzEzW}`


I did this challenge but didn't write the writeup , but since the pwncollege website preserves the server state, /challenge/catflag is directly giving me the key<br>.

For this challenge , firstly I tried to inovke  /challenge/catflag to get the flag but it obviouslt didn't give me the flag , instead it read  /home/hacker/not-the-flag
file <br>
Then I used the ln -s command to create a symlink of /flag file which contains the flag , " ln -s /flag /home/hacker/not-the-flag" . I did this so that the next time I 
invoke the /challenge/catflag command which'll read the /home/hacker/not-the-flag , that'll help me get the flag , cuz it's the symlink to /flag.

 
 ```bash
hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag
ln: failed to create symbolic link '/home/hacker/not-the-flag': File exists
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{8z-ZBwWahjyiaiAzVtWh-pOSJVk.QX5ETN1wSOzgjNzEzW}
hacker@commands~linking-files:~$
```


## What I learned
Got to know about hard and soft links . Accesses to the hard link and accesses to the original file are completely identical, in that they immediately yield the necessary data.<br>
The soft /symbolic link instead contains the original file name , and when you access it , Linux will read the original file name and access that file , though in most cases both result 
in accessing the original data, but the mechanism to access them is different . <br>
ln -s command is used to create symbolic links "ln -s /tmp/myfile /home/hacker/ourfile" <br>
This will make /home/hacker/ourfile as the symbolic link to /tmp/myfile.

## References 
Symbolic links video in the module .
