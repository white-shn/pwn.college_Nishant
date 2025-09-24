# comparing files 
compare two files and get the flag 

## My solve
**Flag:** `pwn.college{AaWpw1AJhNHg_OZzPoc6i2Vfvyr.01MwMDOxwSOzgjNzEzW}`

used the diff command to get the flag. It was given that both the files have 100 command fake flags and one file has the real flag , which I was able to retrieve using the diff command . <br>
58a59 tells us " after line 58 of file 1, add line 59 of file 2" 
i.e there is an different line 59 in file 2 which isn't in file 1

 ```bash
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt   /challenge/decoys_and_real.txt
58a59
> pwn.college{AaWpw1AJhNHg_OZzPoc6i2Vfvyr.01MwMDOxwSOzgjNzEzW}
```

## What I learned
Got familiar with diff command.<br>
Got to know that the diff command is used to compare two files line by line and shows the difference between them.

## References 
None
