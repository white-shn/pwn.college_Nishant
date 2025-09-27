## Exclusionary globbing
With the help of exclusionary globbing get into /challenge/files and run /challenge/run with all files that don't start with p, w, or n.

## My solve
**Flag:** `pwn.college{EpcLdlBFgScLV2aZfalOPn4YWgp.QX2IDO0wSOzgjNzEzW}`

I got into the directory /challenge/files using cd , then listed the files in it using ls .<br>
Then I executed /challenge/run with argument " [^pwn]* " that helped me get the files that don't start with p , w , n . <br>
The '^' is used to list character that aren't in the  [ ] globe. 

```bash
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ ls 
amazing    challenging  educational  great  incredible  kind      magical  optimistic  queenly  splendid   uplifting   wonderful  youthful
beautiful  delightful   fantastic    happy  jovial      laughing  nice     pwning      radiant  thrilling  victorious  xenial     zesty
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [pwn]*
Your expansion did not expand to the requested files (amazing beautiful 
challenging delightful educational fantastic great happy incredible jovial kind 
laughing magical optimistic queenly radiant splendid thrilling uplifting 
victorious xenial youthful zesty).
Instead, it expanded to:
nice pwning wonderful
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [^pwn]*
You got it! Here is your flag!
pwn.college{EpcLdlBFgScLV2aZfalOPn4YWgp.QX2IDO0wSOzgjNzEzW}
hacker@globbing~exclusionary-globbing:/challenge/files$
```
## What I learned
Learned about exclusionary globbing that helps us get files excluding certain files we don't want . 

## References
None
