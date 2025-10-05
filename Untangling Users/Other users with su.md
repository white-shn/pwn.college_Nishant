## Other users with su 
For this challenge you must switch to the zardus user and then run /challenge/run

## My solve
**Flag:** `pwn.college{gDI0idTHQBsu6A3mq96rBofZAem.QX2UDN1wSOzgjNzEzW}`

Switch to zardus by giving `su` an argument of zardus , then entered the password and executed `/challenge/run` .

```bash
hacker@users~other-users-with-su:~$ su zardas
WARNING: you are invoking 'su' without specifying the 'zardus' user.
su: user zardas does not exist
hacker@users~other-users-with-su:~$ su zardus
Password: 
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{gDI0idTHQBsu6A3mq96rBofZAem.QX2UDN1wSOzgjNzEzW}
zardus@users~other-users-with-su:/home/hacker$
```

## What I learned
Learned to switch users. 

## References
None
