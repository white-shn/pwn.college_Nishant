# hidden files
find the flag , hidden as a dot-prepended file in /

## My solve
**Flag:** `pwn.college{0sF6bpDFk3OJJK3ntO_oUSTalTM.QXwUDO0wSOzgjNzEzW}`

Get in the root file with cd . I listed the files in root directory without invoking it with '-a' to see the files . <br> 
Then used the ls command with '-a' to view the hidden files .<br>
Then I read the flag file with cat command to get the flag.

```bash
hacker@commands~hidden-files:/$  cd /
hacker@commands~hidden-files:/$ ls
bin  boot  challenge  dev  etc  home  lib  lib32  lib64  libx32  media  mnt  nix  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv           bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-2337316431094  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-2337316431094
pwn.college{0sF6bpDFk3OJJK3ntO_oUSTalTM.QXwUDO0wSOzgjNzEzW}
hacker@commands~hidden-files:/$
```

## What I learned
Got to know that ls doesn't list all the files by default . <br>
Files starting with '.' don't show up by default in ls.<br>
We've to invoke ls with -a flag to view the files starting with '.'

## References 
None
