# Searching For Manuals
Find hidden man page that'll tell you how to use /challenge/challenge then use /challenge/challenge with proper directions given in hidden man page

## My solve

I used the man man to see the usage of man, there I got "man -k printf<br>
           Search  the  short  descriptions  and  manual page names for the keyword printf as regular expression.  Print out any matches.  Equivalent to<br>
           apropos printf." <br>
Then I used the same command and instead of printf I used flag " man -k flag" which gave me a list of man pages which contains the keyword flag <br>
and I got a man page "wbcdeunxet" which had the description "print the flag!" .<br>
I did " man wbcdeunxet" which opened the wbcdeunxet manual and there , in it's description I got the following argument which can help me get the flag . <br>
 --wbcdeu NUM<br>
              print the flag if NUM is 511<br>
Then I did " /challenge/challenge --wbcdeu 511" <br>
This gave me the flag.

**Flag:** `pwn.college{MXwDObcdS5CWeunxetAiXvJ1pP1.QX2EDO0wSOzgjNzEzW}`

```bash
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -k flag
dpkg-buildflags (1)  - returns build flags to use during package build
Dpkg::BuildFlags (3perl) - query build flags
fegetexceptflag (3)  - floating-point rounding and exception handling
fesetexceptflag (3)  - floating-point rounding and exception handling
i386 (8)             - change reported architecture in new program environment and/or set personality flags
ioctl_iflags (2)     - ioctl() operations for inode flags
linux32 (1)          - change reported architecture in new program environment and/or set personality flags
linux64 (1)          - change reported architecture in new program environment and/or set personality flags
pcap-config (1)      - write libpcap compiler and linker flags to standard output
security_compute_av_flags (3) - query the SELinux policy database in the kernel
security_compute_av_flags_raw (3) - query the SELinux policy database in the kernel
set_matchpathcon_flags (3) - set flags controlling the operation of matchpathcon or matchpathcon_index and configure the behaviour of validity checking a...
set_matchpathcon_invalidcon (3) - set flags controlling the operation of matchpathcon or matchpathcon_index and configure the behaviour of validity check...
set_matchpathcon_printf (3) - set flags controlling the operation of matchpathcon or matchpathcon_index and configure the behaviour of validity checking ...
setarch (1)          - change reported architecture in new program environment and/or set personality flags
setarch (8)          - change reported architecture in new program environment and/or set personality flags
wbcdeunxet (1)       - print the flag!
x86_64 (8)           - change reported architecture in new program environment and/or set personality flags
hacker@man~searching-for-manuals:~$
hacker@man~searching-for-manuals:~$ /challenge/challenge wbcdeunxet
Incorrect usage! Please read the hidden challenge man page!
hacker@man~searching-for-manuals:~$ man wbcdeunxet
hacker@man~searching-for-manuals:~$ /challenge/challenge --wbcdeu 511
Correct usage! Your flag: pwn.college{MXwDObcdS5CWeunxetAiXvJ1pP1.QX2EDO0wSOzgjNzEzW}
hacker@man~searching-for-manuals:~$
```

## What I learned 
Learned how to propely use the manuals and how to read them which helped me get various commands which were useful to get the flag. 

## References 
None
