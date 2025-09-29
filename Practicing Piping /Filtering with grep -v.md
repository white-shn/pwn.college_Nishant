## Filtering with grep -v
Filter the decoy flags we get as an output of /challenge/run to get the real flag. 

## My solve
**Flag:** `pwn.college{YEqQGeQqPn6kxCSgfZDqc5-PPOk.0FOxEzNxwSOzgjNzEzW}`

Using | (pipe) to redirect the output of /challenge/run to grep -v , which will help me filte the DECOY flags, and list the lines that don't have the string " DEOCY"
in them which will be the real flag .

```bash
hacker@piping~filtering-with-grep-v:~$ /challenge/run | grep -v DECOY
pwn.college{YEqQGeQqPn6kxCSgfZDqc5-PPOk.0FOxEzNxwSOzgjNzEzW}
hacker@piping~filtering-with-grep-v:~$
```
## What I learned
Learned about the useful option of grep command , -v (invert match ) which helps us to filter the data we don't want. <br>
Normal grep matches the lines and lists the lines that are matching whereas , grep -v lists the lines except for the ones that have the string you gave. 

## References 
None
