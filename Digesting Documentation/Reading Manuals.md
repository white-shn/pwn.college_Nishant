# Reading Manuals
use the man page for challenge and get the flag 

## My solve
**Flag:** ` `

I used the man command . The man page of challenge opened and looked something like this: 
```bash
CHALLENGE(1)                                      Challenge Commands                                     CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --olkfit NUM
              print the flag if NUM is 450

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                                            May 2024                                          CHALLENGE(1)
```

From here we can see in DESCRIPTION that --olkfit NUM will print the flag when NUM is 450 .<br>
I used this as an argument to /challenge/challenge , and put NUM = 450 . <br>

```bash
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge --olkfit 450
Correct usage! Your flag: pwn.college{olkfYiTtTulBC-XUbFE45Oc_vYc.QX0EDO0wSOzgjNzEzW}
hacker@man~reading-manuals:~$ 
```

## What I learned 
Learned about the man command which is short for manual , and displays the manual of the command you pass as argument .<br>
The arguments given to man aren't file paths but just the name of the entries . 

## References 
None
