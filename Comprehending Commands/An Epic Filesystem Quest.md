# An Epic Filesystem Quest
use cd, ls , cat to get the hidden flag 

## My solve
**Flag:** `It is: pwn.college{syCkGHIcmV8IBchUNZ6LGQ2ZGy2.QX5IDO0wSOzgjNzEzW}`

This is byfar the longest task I've done <br>. 
It started with getting in the root directory , then I listed all the files in it , got a file named 'NUGGET' . <br>
Then I used cat to read that file which gave me a new directory , I used cd to get in the directory and again ls , then cat on the file (MEMO) and this goes on and on.<br>
Then I got one directory in which I has to use " ls -a " cuz the hint filename starts with '.' .<br>
Then continue the cd , ls command until you encounter that 'cd'ing into the directory will destroy the flag' .<br> 

Now we can't use cd to get in the directory but we need the hint file in that directory , so we'll use the ls command without getting in the directory ,<br>
by providing the path of the directory as argument.<br>
This will list the files in the directory without getting into the directory using cd. <br>
Now use cat and give the path of the file you get by listing this directory as an argument . <br>

You'll get another directory . Use cd to get in that directory and list the files using ls , use cat to read that file and you'll get the flag . 

```bash
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
NUGGET  bin  boot  challenge  dev  etc  flag  home  lib  lib32  lib64  libx32  media  mnt  nix  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
hacker@commands~an-epic-filesystem-quest:/$ cat NUGGET
Great sleuthing!
The next clue is in: /usr/share/racket/pkgs/wxme-lib/wxme/private/compiled
hacker@commands~an-epic-filesystem-quest:/$ cd  /usr/share/racket/pkgs/wxme-lib/wxme/private/compiled
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/wxme-lib/wxme/private/compiled$ ls
MEMO  class-help_rkt.dep  class-help_rkt.zo  compat_rkt.dep  compat_rkt.zo  readable-editor_rkt.dep  readable-editor_rkt.zo
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/wxme-lib/wxme/private/compiled$ cat MEMO
Yahaha, you found me!
The next clue is in: /usr/local/lib/python3.8/dist-packages/elftools/__pycache__

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/wxme-lib/wxme/private/compiled$ cd /usr/local/lib/python3.8/dist-packages/elftools/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/elftools/__pycache__$ ls
DISPATCH  __init__.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/elftools/__pycache__$ cat DISPATCH
Yahaha, you found me!
The next clue is in: /usr/local/lib/python3.8/dist-packages/sympy/matrices/__pycache__

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/elftools/__pycache__$ cd /usr/local/lib/python3.8/dist-packages/sympy/matrices/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/matrices/__pycache__$ ls
SECRET                         determinant.cpython-38.pyc  inverse.cpython-38.pyc      reductions.cpython-38.pyc   subspaces.cpython-38.pyc
__init__.cpython-38.pyc        eigen.cpython-38.pyc        kind.cpython-38.pyc         repmatrix.cpython-38.pyc    utilities.cpython-38.pyc
common.cpython-38.pyc          exceptions.cpython-38.pyc   matrices.cpython-38.pyc     solvers.cpython-38.pyc
decompositions.cpython-38.pyc  graph.cpython-38.pyc        matrixbase.cpython-38.pyc   sparse.cpython-38.pyc
dense.cpython-38.pyc           immutable.cpython-38.pyc    normalforms.cpython-38.pyc  sparsetools.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/matrices/__pycache__$ cat SECRET
Tubular find!
The next clue is in: /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/backports/tarfile/compat

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/matrices/__pycache__$ cd  /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/backports/tarfile/compat
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/setuptools/_vendor/backports/tarfile/compat$ ls -a
.  ..  .EVIDENCE  __init__.py  __pycache__  py38.py
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/setuptools/_vendor/backports/tarfile/compat$ cat .EVIDENCE
Tubular find!
The next clue is in: /opt/linux/linux-5.4/include/config/have/virt

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/setuptools/_vendor/backports/tarfile/compat$ cd /opt/linux/linux-5.4/include/config/have/virt
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/have/virt$ ls
BRIEF  cpu
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/have/virt$ cat BRIEF
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/have/virt$ cd  /usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party$ ls
2  2and3  3  DOSSIER
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party$ cat DOSSIER
Congratulations, you found the clue!
The next clue is in: /usr/share/racket/pkgs/realm/chapter12/compiled

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party$ ls  /usr/share/racket/pkgs/realm/chapter12/compiled
INSIGHT-TRAPPED  source_rkt.dep  source_rkt.zo
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party$ cat  /usr/share/racket/pkgs/realm/chapter12/compiled/INSIGHT-TRAPPED
Tubular find!
The next clue is in: /usr/share/javascript/mathjax/localization/es

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party$ cd /usr/share/javascript/mathjax/localization/es
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/localization/es$ ls
FontWarnings.js  HTML-CSS.js  HelpDialog.js  MathML.js  MathMenu.js  SPOILER  TeX.js  es.js
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/localization/es$ cat SPOILER
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{syCkGHIcmV8IBchUNZ6LGQ2ZGy2.QX5IDO0wSOzgjNzEzW}
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/localization/es$

```

## What I learned
Learned to use cd , ls , cat properly and in better ways .

## References 
None
