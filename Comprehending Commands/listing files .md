# listing files
listing files in /challenge and invoke the /challenge/run program which has a random name 

## My solve
**Flag:** `pwn.college{MG73qRw9DdzfeV4-IoBHj5vST_b.QX4IDO0wSOzgjNzEzW}`

Firstly I listed the files in the challenge directory , which gave me a name of the file . <br> 
Then I invoked the entire program using it which gave me the flag.

 ```bash
hacker@commands~listing-files:~$ ls /challenge
17663-renamed-run-24865  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/17663-renamed-run-24865
Yahaha, you found me! Here is your flag:
pwn.college{MG73qRw9DdzfeV4-IoBHj5vST_b.QX4IDO0wSOzgjNzEzW}
hacker@commands~listing-files:~$
```
Also while doing this I got another flag (probably a fake one)<br>
I listed the files in the home directory and got a file f , when I tried to read that file using cat , I got a flag , but it's obviously a fake one .

```bash
hacker@commands~listing-files:~$ ls
f
hacker@commands~listing-files:~$ cat f
pwn.college{oIXdrTEml7FfAbApdmEw4kAhIdh.QXzMDO0wSOzgjNzEzW}
```

## What I learned
Learned how to use the ls command which is used to list the files in a directory .
If no arguments are provided in the ls command it lists the files in the home directory 

## References 
None


















