# grepping for a needle in a haystack
using grep get the flag in the given file 

## My solve
**Flag:** `pwn.college{cqUTJDT0PVt1FLurDnvPiz4IGmE.QX3EDO0wSOzgjNzEzW}`

Invoke the grip command which will search for the string you need (in this case the flag which starts with pwn.college so our string is pwn.college).<br>
Invoke the command by writing the string and the path of the file in which you've to search so it'll be " grip pwn.college  path to file ". <br>
Hit enter and you'll get the flag , i.e you'll get the line of test in which the mentioned string is .

 ```bash
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/data.txt
pwn.college{cqUTJDT0PVt1FLurDnvPiz4IGmE.QX3EDO0wSOzgjNzEzW}
hacker@commands~grepping-for-a-needle-in-a-haystack:~$
```

## What I learned
Got familiar with grep command .<br>
One way to use grep is to search for a string of text in multiple lines of text.

## References 
None
