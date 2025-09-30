## Reading Files
Read /challenge/read_me into the PWN environment variable

## My solve
**Flag:** `pwn.college{IPmkAXxY5FFkwQFjxf2BzdFa-Y0.QXwIDO0wSOzgjNzEzW}`

Used 'read' and < to redirect the output of /challenge/read_me in PWN and read it . <br>
I combined the read with file redirection to get the output directly into the PWN variable.

```bash
hacker@variables~reading-files:~$ read PWN < /challenge/read_me
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{IPmkAXxY5FFkwQFjxf2BzdFa-Y0.QXwIDO0wSOzgjNzEzW}
hacker@variables~reading-files:~$ 
```

## What I learned 
Learned to read the output of a file directly using the features of shell

## References
None
