## Extracting specific sections of text
Use cut to extract the flag characters from the output of /challenge/run , 
then pipe them to tr -d "\n" to join them together into a single line.

## My solve
**Flag:** `pwn.college{Q6K9Np4dbTjqAni6lleWz3Pw4um.01NxEzNxwSOzgjNzEzW}`

Used cut to extract the column with flag characters from the output of /challenge/run.
Then piped them to tr -d "\n" to delete newlines which gave me the flag.

```bash
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run
24948 p
4338 w
15179 n
21731 .
1115 c
11518 o
2721 l
24875 l
27882 e
11274 g
1327 e
23982 {
21580 Q
18908 6
6601 K
28090 9
31708 N
10771 p
26971 4
26673 d
27145 b
11798 T
11439 j
12097 q
29539 A
30661 n
19839 i
26766 6
19964 l
846 l
31381 e
28707 W
16064 z
27976 3
5319 P
19281 w
29147 4
31842 u
10682 m
31567 .
10959 0
12827 1
10652 N
17556 x
23125 E
8040 z
1624 N
5769 x
4325 w
11318 S
16945 O
22416 z
21320 g
12933 j
26993 N
12189 z
31637 E
1817 z
10570 W
18289 }
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run | cut -d " " -f 2 | tr -d "\n"
pwn.college{Q6K9Np4dbTjqAni6lleWz3Pw4um.01NxEzNxwSOzgjNzEzW}hacker@data~extracting-specific-sections-of-text:~$
```

## What I learned
Learned about use cut command to get specific columns of data , such as the first column etc. <br>
The -d argument after cut specifies how the columns are separated ,in this challenge they were seperated by space character . 

## References
None
