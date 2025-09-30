## Process substitution for input
Used process substitution with diff to compare the outputs of two commmands and get the flag

## My solve
**Flag:** ` pwn.college{Yow-O5CuXBHsn6tB27wELjABJB2.0lNwMDOxwSOzgjNzEzW}`

I used process substitution with the diff command . <br>
<(/challenge/print_decoys) and <(/challenge/print_decoys_and_flag) saves the output of the commands in a temporary file called named pipe, then used diff command to 
compare them which printed the flag. 

```bash
hacker@piping~process-substitution-for-input:~$ diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
10a11
> pwn.college{Yow-O5CuXBHsn6tB27wELjABJB2.0lNwMDOxwSOzgjNzEzW}
hacker@piping~process-substitution-for-input:~$
```

## What I learned
Learned about process substitution.<br>
Process substituion can help treating the inputs and outputs of commands as arguments to a command . <br>
<(command) executes the command and saves it to a temporary file which is called named pipe . 

## References 
None
