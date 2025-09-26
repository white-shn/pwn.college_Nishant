# Matching with []
Get in /challenge/files and run /challenge/run with a single argument that bracket-globs into file_b, file_a, file_s, and file_h

## My solve
**Flag:** `pwn.college{MNlHQBU1cXHfEc2xLJP1FH2yygm.QXzIDO0wSOzgjNzEzW} `

I got in the /challenge/files directory using cd command , then I executed the /challenge/run program with argument such that bracket-glob into given files. <br>
/challenge/run file_[bash].

```bash
hacker@globbing~matching-with-:~$ cd /challenge/files
hacker@globbing~matching-with-:/challenge/files$ ls
file_a  file_c  file_e  file_g  file_i  file_k  file_m  file_o  file_q  file_s  file_u  file_w  file_y
file_b  file_d  file_f  file_h  file_j  file_l  file_n  file_p  file_r  file_t  file_v  file_x  file_z
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[bash]
You got it! Here is your flag!
pwn.college{MNlHQBU1cXHfEc2xLJP1FH2yygm.QXzIDO0wSOzgjNzEzW}
```

## What I learned
Learned about [] globe which matches the characters , specified in the bracket . for ex, [ab] will match characters a and b .

## References 
None
