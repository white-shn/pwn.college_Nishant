## Extracting the first lines with head
/challenge/pwn outputs a bunch of data, and you'll need to pipe it through head to grab just the first 7 lines and then pipe them onwards to /challenge/college.

## My solve 
**Flag:** `pwn.college{0_6oKsdIUCS3ZVETpVIMM_S3-Qd.0lNxEzNxwSOzgjNzEzW}`

Pipe the output of /challenge/run through head to get the first 7 lines and pipe them to /challenge/college .

```bash
hacker@data~extracting-the-first-lines-with-head:~$ /challenge/pwn | head -n 7 | /challenge/college
Congratulations, you piped the right codes!
pwn.college{0_6oKsdIUCS3ZVETpVIMM_S3-Qd.0lNxEzNxwSOzgjNzEzW}
hacker@data~extracting-the-first-lines-with-head:~$ 
```

## What I learned 
Learned about head command which is used to display the first few lines of it's input. 

## References
None
