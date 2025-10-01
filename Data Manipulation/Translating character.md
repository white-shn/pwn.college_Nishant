## Translating character
/challenge/run will give you the flag with the character case swapped, use tr to get the correct flag 

## My solve
**Flag:** `pwn.college{EoAzVF9kneTVNLqMsrtijV7zeSO.01MxEzNxwSOzgjNzEzW}`

Get the case swapped flag by executing /challenge/run. Then use tr which translated the argument you provide at first to the argument you give as second. <br>
The first and second arguments will be "PWN.COLLEGE{eOaZvf9KNEtvnlQmSRTIJv7ZEso.01mXeZnXWsoZGJnZeZw}" and "pwn.college{EoAzVF9kneTVNLqMsrtijV7zeSO.01MxEzNxwSOzgjNzEzW}" respectively which will give you the
corrected flag. 

```bash
hacker@data~translating-characters:~$ /challenge/run
Your case-swapped flag:
PWN.COLLEGE{eOaZvf9KNEtvnlQmSRTIJv7ZEso.01mXeZnXWsoZGJnZeZw}

hacker@data~translating-characters:~$ /challenge/run | tr PWN.COLLEGE{eOaZvf9KNEtvnlQmSRTIJv7ZEso.01mXeZnXWsoZGJnZeZw} pwn.college{EoAzVF9kneTVNLqMsrtijV7zeSO.01MxEzNxwSOzgjNzEzW}
YOur cASE-SWAppEd FLAg:
pwn.college{EoAzVF9kneTVNLqMsrtijV7zeSO.01MxEzNxwSOzgjNzEzW}

hacker@data~translating-characters:~$
```

## What I learned 
Learned about the tr command which translates the character provided in its first argument to the character provided in its second argument.

## References 
None
