---
---

[HOME](index.md)
[ABOUT](README.md)
[WEB](https://git.vlsm.org/)
[GITHUB](https://github.com/UI-FASILKOM-OS/git/)
[TOP](#)
[BOTTOM](#endofpage)
[PREV](a01-git-basics.md)
[NEXT](a03-git-basics.md)

# Git Basics 2

<br>
## Command Lines

* cat
* cd
* echo
* git
   * git add
   * git init
   * git status
   * git rm --cached
* ls
   * ls -l
   * ls -al
* mkdir
* PS1="$ "
* pwd
* rm

<br>
## Git Status

Input (Cut and Paste):
```
pwd
git status
```

Output:
```
$ pwd
/home/demo/exercise/demo
$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
$
```

<br>
## Add "file.txt" to Stage

Input (Cut and Paste):
```
echo 'This is file.txt' > file.txt
cat file.txt
ls -al
git add file.txt 
git status
```

Output:
```
$ echo 'This is file.txt' > file.txt

$ cat file.txt
This is file.txt

$ ls -al
total 16
drwxr-xr-x 3 demo demo 4096 Aug 10 13:49 .
drwxr-xr-x 3 demo demo 4096 Aug 10 09:22 ..
-rw-r--r-- 1 demo demo   17 Aug 10 13:49 file.txt
drwxr-xr-x 7 demo demo 4096 Aug 10 13:46 .git

$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	file.txt

nothing added to commit but untracked files present (use "git add" to track)

$ git add file.txt 

$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   file.txt
$
```

<br>
## Unstage "file1.txt"

Input (Cut and Paste):
```
git rm --cached file.txt 
git status
```

Output:
```
$ git rm --cached file.txt 
rm 'file.txt'

$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	file.txt

nothing added to commit but untracked files present (use "git add" to track)
$
```


<br>
## Delete "file1.txt" from directory

Input (Cut and Paste):
```
rm file.txt 
git status
ls -al
```

Output:
```
$ rm file.txt 

$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)

$ ls -al
total 12
drwxr-xr-x 3 demo demo 4096 Aug 10 09:58 .
drwxr-xr-x 3 demo demo 4096 Aug 10 09:22 ..
drwxr-xr-x 7 demo demo 4096 Aug 10 09:58 .git
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
[PREV](a01-git-basics.md)
[NEXT](a03-git-basics.md)
<br>

