# Home sweet home
Copy  flag in a file by passing it as an argument to /challenge/run

## My solve
**Flag:** `pwn.college{oIXdrTEml7FfAbApdmEw4kAhIdh.QXzMDO0wSOzgjNzEzW}`

we had to provide a path like this "hacker@dojo:~$ /challenge/run YOUR_PATH_HERE" 
~ is the shorthand for /home/hacker. 
So I wrote the file as an argument by writing " ~/f "
'/' used cuz it was specified that argument must be absolute path. 
I wrote only f in the argument cuz only three letters were to be used . 

```bash
hacker@paths~home-sweet-home:~$ /challenge/run ~/flag
The argument you provided must not have been longer than 3 characters (it's 
currently 6 characters long)!
hacker@paths~home-sweet-home:~$ /challenge/run ~/f
Writing the file to /home/hacker/f!
... and reading it back to you:
pwn.college{oIXdrTEml7FfAbApdmEw4kAhIdh.QXzMDO0wSOzgjNzEzW}
hacker@paths~home-sweet-home:~$ 

```

## What I learned
~ is a shorthand for /home/hacker.
Learned copying flag in a file by passing it as an argument .

## References
None
