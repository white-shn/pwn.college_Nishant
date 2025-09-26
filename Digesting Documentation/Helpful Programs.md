# Helpful Programs
practice reading a program's documentation with --help

## My solve
**Flag:** `pwn.college{helloworld}`

Used the argument " --help" in /challenge/challenge , which gave me some information about the program , <br>
It gave me some arguments, one was -p which prints the value which will help me use the -g argument that'll give me the flag . <br>
I used the -p argument invoking /challenge/challenge . This gave me a secret value to use on -g argument , then I invoked the " /challenge/challenge -g 713 "which <br>
gave me the flag .

```bash
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -g
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]
a challenge to make you ask for help: error: argument -g/--give-the-flag: expected one argument
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 713
hacker@man~helpful-programs:~$ /challenge/challenge -g 713
Correct usage! Your flag: pwn.college{o71X3wVrGOuSM7DT_KCy6q8iWDP.QX3IDO0wSOzgjNzEzW}
hacker@man~helpful-programs:~$
```

## What I learned
Learned to use --help to get the description of a program , that tells me about the program and can help me invoke it . 


## References 
None
