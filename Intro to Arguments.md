# Intro to arguments
In this challenge requires to  run the hello command with argument of hackers to get the flag

## My solve 

**Flag:** `pwn.college{0WAD6OX7JNmttZ1_oOVy5OYRK12.QX4YjM1wSOzgjNzEzW}`

When you type a line of text and hit enter, the shell resolves the text the input in command and it's arguements. The first word is the command and the next words are  arguments.
This challenge required to run the hello command with single argument of 'hackers'.
So we know that when we type 'hello hackers' , the shell resolves hello as a command and hackers as the argument . 
press enter and we get the flag .
```bash
hacker@hello~intro-to-arguments:~$ hello hackers
Success! Here is your flag:
pwn.college{0WAD6OX7JNmttZ1_oOVy5OYRK12.QX4YjM1wSOzgjNzEzW}
```

## What I learned
I learned that shell parses the input into command and arguments . For a line of text ,the first word is taken as the command and the rest is the argument.
In this challenge , 'hello' was the command and 'hackers' was the argument.


## References 
Just the instructions given in the pwn.college website 
