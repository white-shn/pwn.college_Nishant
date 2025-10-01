## Deleting new lines
Delete the newlines in the flag to get the correct flag. 

## My solve
**Flag:** `:pwn.college{M-yoagEe9aKwZDXYGll0Qp2mlVJ.0VNxEzNxwSOzgjNzEzW}`

Delete the newlines with the help of tr -d , and for the newlines use "\n".<br>
Use "\n" as arugment after tr -d and you'll get the corrected flag. 

```bash
hacker@data~deleting-newlines:~$ /challenge/run
Your line-split flag: 
p
wn
.
c
o
ll
eg
e
{
M
-y
oag
E
e9
a
Kw
Z
D
X
Y
Gl
l
0Q
p2m
l
VJ.0
VNx
E
zN
xw
SO
z
gjN
z
E
z
W}

hacker@data~deleting-newlines:~$ /challenge/run | tr -d " \n"
Yourline-splitflag:pwn.college{M-yoagEe9aKwZDXYGll0Qp2mlVJ.0VNxEzNxwSOzgjNzEzW}
hacker@data~deleting-newlines:~$ 
```

## What I learned 
Learned about "\n" which is used to specify new lines .

## References 
None
