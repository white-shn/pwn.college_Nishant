## Deleting characters.md

## My solve
**Flag:** `pwn.college{oG0qnOrzE7W6GnL5aHyXbHr-MVh.0FNxEzNxwSOzgjNzEzW}`

Firstly I executed the /challenge/run porgram to see what are the unwanted characters in the flag. <br>
Next I used the tr command and -d , giving the argument of the characters to be removed , in this case " %^ " which gave me the corrected flag .

```bash
hacker@data~deleting-characters:~$ /challenge/run
Your character-stuffed flag:
p%w%n%.%c^%o^%l^%l^e^g^e{^o%G^%0^q^n%O^%r%z^%E^%7^W^6^%Gn^%L^%5%a^H^yXb%H%r^-M^V%h.^0%F^Nx^%E^%z^N%x^%wSO^%z^%g%jN^z^Ez%W}%^%
hacker@data~deleting-characters:~$ /challenge/run | tr -d ^%
Your character-stuffed flag:
pwn.college{oG0qnOrzE7W6GnL5aHyXbHr-MVh.0FNxEzNxwSOzgjNzEzW}
hacker@data~deleting-characters:~$
```

## What I learned
Learned to remove characters using tr -d .

## References
None
