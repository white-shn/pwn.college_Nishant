## Exporting Variables
invoke /challenge/run with the PWN variable exported and set to the value COLLEGE,
and the COLLEGE variable set to the value PWN but not exported .

## My solve
**Flag:** `pwn.college{YCgKyc0db-J4ZT-cPipUNba7Xt7.QXyYTN0wSOzgjNzEzW}`

I exported PWN variable with value set as COLLEGE , and set the value of COLLEGE variable as PWN. <br>
Then I executed /challenge/run to get the flag for the challenge. 

```bash
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{YCgKyc0db-J4ZT-cPipUNba7Xt7.QXyYTN0wSOzgjNzEzW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$
```

## What I learned 
Learned to export variables .  

## References
None
