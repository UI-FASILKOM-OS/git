---
---

[HOME](index.md)
[ABOUT](README.md)
[WEB](https://git.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/git/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](index.md)
[NEXT](a02-git-basics.md)

# Git Basics 1

<br>
## Command Lines

* cd
* git
   * git init
* ls
   * ls -l
   * ls -al
* mkdir
* PS1="$ "
* pwd


<br>
## Create Directory "exercise/"

Input (Cut and Paste):
```
PS1="$ "
mkdir exercise
cd exercise/
ls -al
pwd
```

Output:
```
(WHATEVER PROMPT) $ PS1="$ "
$ mkdir exercise

$ cd exercise/

$ ls -al
total 8
drwxr-xr-x 2 demo demo 4096 Aug  9 14:52 .
drwxr-xr-x 4 demo demo 4096 Aug  9 14:52 ..

$ pwd
/home/demo/exercise
$
```

<br>
## First Git Repository "demo/"

Input (Cut and Paste):
```
ls -al
git init demo
ls -l
cd demo/
ls -al
```

Output:
```
$ ls -al
total 8
drwxr-xr-x 2 demo demo 4096 Aug 10 09:21 .
drwxr-xr-x 4 demo demo 4096 Aug  9 15:59 ..

$ git init demo
Initialized empty Git repository in /home/demo/exercise/demo/.git/

$ ls -l
total 4
drwxr-xr-x 3 demo demo 4096 Aug 10 09:22 demo

$ cd demo/

$ ls -al
total 12
drwxr-xr-x 3 demo demo 4096 Aug 10 09:22 .
drwxr-xr-x 3 demo demo 4096 Aug 10 09:22 ..
drwxr-xr-x 7 demo demo 4096 Aug 10 09:22 .git
$ 
```

<br>
<hr>
<br>
#### ENDOFPAGE
[HOME](index.md)
[ABOUT](README.md)
[WEB](https://git.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/git/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](index.md)
[NEXT](a02-git-basics.md)
<br>

