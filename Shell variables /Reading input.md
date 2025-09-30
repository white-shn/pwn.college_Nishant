## Reading input 
Use read to set the PWN variable to the value COLLEGE

## My solve
**Flag:** `pwn.college{0uv-WywCFsiz5Idclb_z1HHKFRe.QX4cTN0wSOzgjNzEzW}`

I used "read -p " to get the value of PWN from the user . "read" reads the input into a variable and -p argument lets you specify the prompt
then when asked for input , I entered COLLEGE cuz we had to set valeu of PWN variable as COLLEGE
which gave me the flag for the challenge.

```bash
hacker@variables~reading-input:~$ read -p "INPUT: " PWN
INPUT: COLLEGE
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{0uv-WywCFsiz5Idclb_z1HHKFRe.QX4cTN0wSOzgjNzEzW}
hacker@variables~reading-input:~$ read -p "PUT THE VALUE: " PWN 
PUT THE VALUE: COLLEGE 
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{0uv-WywCFsiz5Idclb_z1HHKFRe.QX4cTN0wSOzgjNzEzW}
hacker@variables~reading-input:~$ 

```

## What I learned
Learned to get input for a varibale from the user using 'read' which read input into a variable . <br>
Used the -p argument, which lets you specify a prompt.

## References
None
