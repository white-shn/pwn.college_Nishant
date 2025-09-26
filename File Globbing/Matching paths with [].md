# Matching paths with []


## My solve
**Flag:** `hacker@globbing~matching-paths-with-:~$ /challenge/run/challenge/file/file_[bash]`

I tried to run  /challeng/run/file_[bash] but it was wrong cuz this command considered it as a directory which it was not , then I tried to pass file_[bash] as argument
while executing /challenge/run but I did that while I wsas in /challenge/files directory so it didn't give me the flag .<br>
Then I got in the home directory, and executed /challenge/run with proper argument involving the [] globe and go the flag.

```bash
hacker@globbing~matching-paths-with-:~$ /challenge/run/file_[bash]
bash: /challenge/run/file_[bash]: Not a directory
hacker@globbing~matching-paths-with-:~$ cd /challenge/files
hacker@globbing~matching-paths-with-:/challenge/files$ /challenge/run file_[bash]
Error: please run with a working directory of /home/hacker!
hacker@globbing~matching-paths-with-:/challenge/files$ cd ~
hacker@globbing~matching-paths-with-:~$ /challenge/run file_[bash]
Error: you will need to specify the path to the files as part of your glob
argument, since they are in a different directory than your current working
directory!
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[bash]
You got it! Here is your flag!
pwn.college{8h7iKPDXDz_5i0f0TalcuwMvrAd.QX0IDO0wSOzgjNzEzW}
```
## What I learned
Learned to match paths with the [] globe. Learned to expand paths with [] globe argument . 

## References 
None
