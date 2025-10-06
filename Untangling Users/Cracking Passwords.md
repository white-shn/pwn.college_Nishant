## Cracking Passwords
We've aleak of /etc/shadow (in /challenge/shadow-leak) and we've Crack it then su to zardus, and run /challenge/run to get the flag.

## My solve
**Flag:** `pwn.college{YWGWfBBv9jl1_9T6FrLwopw42ju.QX3UDN1wSOzgjNzEzW}`

Executed john /challenge/shadow-leak which cracked the hashed password for zardus,, then I switched to zardus using that passoword and then
executed /challenge/run to get the flag.

```bash
hacker@users~cracking-passwords:~$ john /etc/shadow
fopen: /etc/shadow: Permission denied
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04950g/s 288.2p/s 288.2c/s 288.2C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password: 
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{YWGWfBBv9jl1_9T6FrLwopw42ju.QX3UDN1wSOzgjNzEzW}
zardus@users~cracking-passwords:/home/hacker$
```

## What I learned
Learned how hashes are stored in /etc/shadow and how tools like "JOHN THE RIPPER" can crack passwords using hash

## References
https://www.openwall.com/john/
