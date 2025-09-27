## Tab completion
Use tab completion to complete the file name while cat'ing it .

## My solve
**Flag:** `pwn.college{MwX2WLag--Da0YyesGtiyaThQq5.0FN0EzNxwSOzgjNzEzW}`

I listed the files in the /challenge directory after entering it . then I did cat /challenge/pwn and press TAB which completed my file name and then I got the flag.

```bash
hacker@globbing~tab-completion:~$ cd /challenge
hacker@globbing~tab-completion:/challenge$ ls
DESCRIPTION.md  pwncollege​
hacker@globbing~tab-completion:/challenge$ cat /challenge/pwn   
cat: /challenge/pwn: No such file or directory
hacker@globbing~tab-completion:/challenge$ cat /challenge/pwncollege​ 
pwn.college{MwX2WLag--Da0YyesGtiyaThQq5.0FN0EzNxwSOzgjNzEzW}
```
## What I learned 
Learned to use Tab completion which when presses tries to figure out what you're typing and tries to complete it .

## Reference
None
