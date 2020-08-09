---
---

[HOME](index.md)
[ABOUT](README.md)
[WEB](https://git.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/git/)
[TOP](#)
[BOTTOM](#endofpage)

# Create Git Repositories

<br>
* Create an Exercise Directory

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
* Create Git Repository "demo"

Input (Cut and Paste):
```
git init demo
ls -l
ls -al demo/
```

Output:
```
$ git init demo
Initialized empty Git repository in /home/demo/exercise/demo/.git/

$ ls -l
total 8
drwxr-xr-x 3 demo demo 4096 Aug  9 14:53 demo

$ ls -al demo/
total 12
drwxr-xr-x 3 demo demo 4096 Aug  9 14:53 .
drwxr-xr-x 4 demo demo 4096 Aug  9 14:53 ..
drwxr-xr-x 7 demo demo 4096 Aug  9 14:53 .git
$
```

<br>
* Create (bare) remote Git Repository "remote"

Input (Cut and Paste):
```
git init remote --bare
ls -l
ls -al remote/
```

Output:
```
$ git init remote --bare
Initialized empty Git repository in /home/demo/exercise/remote/

$ ls -l
total 8
drwxr-xr-x 3 demo demo 4096 Aug  9 14:53 demo
drwxr-xr-x 7 demo demo 4096 Aug  9 14:53 remote

$ ls -al remote/
total 40
drwxr-xr-x 7 demo demo 4096 Aug  9 14:53 .
drwxr-xr-x 4 demo demo 4096 Aug  9 14:53 ..
drwxr-xr-x 2 demo demo 4096 Aug  9 14:53 branches
-rw-r--r-- 1 demo demo   66 Aug  9 14:53 config
-rw-r--r-- 1 demo demo   73 Aug  9 14:53 description
-rw-r--r-- 1 demo demo   23 Aug  9 14:53 HEAD
drwxr-xr-x 2 demo demo 4096 Aug  9 14:53 hooks
drwxr-xr-x 2 demo demo 4096 Aug  9 14:53 info
drwxr-xr-x 4 demo demo 4096 Aug  9 14:53 objects
drwxr-xr-x 4 demo demo 4096 Aug  9 14:53 refs

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
<br>

