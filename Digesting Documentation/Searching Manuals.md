# Searching Manuals
Search the manuals and find the option that'll give you the flag

## My solve

I used the man command 'man challenge' and the challenge manual opened and then I used '? flag' to search and 'n' and 'N' to move through the search results . <br>
I got the argument '--vzpbbf' that'll give me the flag .<br>
Then I invoked the /challenge/challenge with the argument and got the flag .<br>
**Flag:** `pwn.college{kA4vpv6EiblXNoGdmOTzQjit0m1.QX1EDO0wSOzgjNzEzW} `


```bash
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ /challenge/challenge        --vzpbbf
Initializing...
Correct usage! Your flag: pwn.college{kA4vpv6EiblXNoGdmOTzQjit0m1.QX1EDO0wSOzgjNzEzW}
hacker@man~searching-manuals:~$
```

## What I learned 
Learned to navigate in a manual and search things in a manual using '?' and '/'


## References 
None
