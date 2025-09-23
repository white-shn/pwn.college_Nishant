# implicit relative paths, from /
run  /challenge/run using a relative path

## My solve
**Flag:** `pwn.college{g4cWjQQD0bhQGtNjeAUA1kLesrz.QX5QTN0wSOzgjNzEzW}`

I directly executed the /challenge/run program which helped me get the name of the current working directory 
then used cd command to get in the directory (cd /).

After this I executed the program by writing the relative path of the program (challenge/run) which gave me the flag .

```bash
hacker@paths~implicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{g4cWjQQD0bhQGtNjeAUA1kLesrz.QX5QTN0wSOzgjNzEzW}
hacker@paths~implicit-relative-paths-from-:/$
```

## What I learned
I learned that cwd is my current working directory and that a relative path doesn't start with root (i.e. it doesn't start with /).

Then I learned to execute a program by writing it's relative path. 

## References 
Slies of the video in pwn.college

