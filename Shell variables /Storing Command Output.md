## Storing Command Output
Read the output of the /challenge/run command directly into a variable called PWN

## My solve
**Flag:** `pwn.college{Um33b14JDZcn7EA4aVLaPtAV_cx.QX1cDN1wSOzgjNzEzW}`

Store the output of /challenge/run in the PWN variable , use backticks to get the output of /challenge/run as a value to be assigned to PWN.<br>
Next print the flag by cat , echo or env to get the flag for this challenge. 

```bash
hacker@variables~storing-command-output:~$ PWN=`/challenge/run`
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo "$PWN"
pwn.college{Um33b14JDZcn7EA4aVLaPtAV_cx.QX1cDN1wSOzgjNzEzW}
hacker@variables~storing-command-output:~$ env $PWN
env: ‘pwn.college{Um33b14JDZcn7EA4aVLaPtAV_cx.QX1cDN1wSOzgjNzEzW}’: Permission denied
hacker@variables~storing-command-output:~$
```

## What I learned
Learned to store the output of a command in a variable.

## References 
None
