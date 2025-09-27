## Mixing globs
Write a single short glob that will match the files mentioned. 

## My solve
**Flag:** `pwn.college{oeE1oyL0yg9ZwXj0YBOUZ5_VP2L.QX1IDO0wSOzgjNzEzW}`

I got into the directory using cd then wrote the argument that I had to pass to /challenge/run to get the flag. <br>
"[cep]* " I entered the starting letter of the names of the files to get and then the ' * ' globe that can match the rest letters. 

```bash
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{oeE1oyL0yg9ZwXj0YBOUZ5_VP2L.QX1IDO0wSOzgjNzEzW}
hacker@globbing~mixing-globs:/challenge/files$
```
## What I learned
Learned to use multiple globes in a single argument .
