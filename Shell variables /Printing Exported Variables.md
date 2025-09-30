## Printing Exported Variables
Used the evn command to print the value of the exported variable FLAG 

## My solve
**Flag:** `pwn.college{4sLHVMcFj2DNI3irvAVi65B2weK.QX4UTN0wSOzgjNzEzW}`

I used the evn command to print the value of FLAG , also remember to add $ to access your variable.

```bash
hacker@variables~printing-exported-variables:~$ env  $FLAG
env: ‘pwn.college{4sLHVMcFj2DNI3irvAVi65B2weK.QX4UTN0wSOzgjNzEzW}’: Permission denied
hacker@variables~printing-exported-variables:~$
```

## What I learned
Learned to access variables using evn command. evn variable prints out every exported variable set in your shell. 

## References
None
