## Using sudo 
Use sudo access to read the flag.

## My solve
**Flag:** `pwn.college{wvO5jNIe5ntmuZKV1Z1VL0A92Kz.QX4UDN1wSOzgjNzEzW}`

Used  sudo to read the flag: sudo cat /flag.

```bash
hacker@users~using-sudo:~$ ls /
bin  boot  challenge  dev  etc  flag  home  lib  lib32  lib64  libx32  media  mnt  nix  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
hacker@users~using-sudo:~$ sudo cat /flag
pwn.college{wvO5jNIe5ntmuZKV1Z1VL0A92Kz.QX4UDN1wSOzgjNzEzW}
hacker@users~using-sudo:~$
```

## What I learned 
Learned how sudo works <br>
Unlike su, which defaults to launching a shell as a specified user, sudo defaults to running a command as root.

## References 
None
