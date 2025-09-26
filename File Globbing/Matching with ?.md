# Matching with ?
Used the ? glob to cd in the /challenge directory and then execute /challenge/run

## My solve
**Flag:** `pwn.college{sNYVzMDvBJqBeL-9fspuFUd_xO-.QXyIDO0wSOzgjNzEzW}`

Since shell treats ? as a single character, we can only used it as a replacement for a single character here. <br>
The challenge asked to use ? for c and l , so I did  " cd /?ha??enge"<br>
With this I got into the /challenge directory , next the executed  /challenge/run to get the flag.

```bash
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{sNYVzMDvBJqBeL-9fspuFUd_xO-.QXyIDO0wSOzgjNzEzW}
hacker@globbing~matching-with-:/challenge$ 
```

## What I learned
Learned about the ?  globe .This is similiar the the * globe but the shell treats ? only as a single character so ? works like * but matches only one character.

## References 
None
