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
* Name and Email
  * Replace "my@e.mail" with your (fake?) email.
  * Replace "My Name" with you (fake?) name.

Input (Cut and Paste):
```
git config --global user.email "my@e.mail"
git config --global user.name "My Name"
```

Output:
```
$ git config --global user.email "my@e.mail"
$ git config --global user.name "My Name"
$
```

<br>
* Initial Commit

Input (Cut and Paste):
```
git commit -am "Initial Commit" --allow-empty
git log --stat
```

Output:
```
$ git commit -am "Initial Commit" --allow-empty
[master (root-commit) 498dda4] Initial Commit
$ git log --stat
commit 498dda4b0ca033599960e404b4a02cadcbb65acc (HEAD -> master)
Author: My Name <my@e.mail>
Date:   Sun Aug 9 15:44:46 2020 +0700

    Initial Commit
$ 
```

<br>
* Add Remote to Repo

Input (Cut and Paste):
```
git remote add origin ../remote/
git push --set-upstream origin master;
```

Output:
```
$ git remote add origin ../remote/
$ git push --set-upstream origin master;
Enumerating objects: 2, done.
Counting objects: 100% (2/2), done.
Writing objects: 100% (2/2), 159 bytes | 159.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0)
To ../remote/
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
```

<br>
* Status

Input (Cut and Paste):
```
git branch -v
git remote -v
git status
git log --stat
```

Output:
```
$ git branch -v
* master 498dda4 Initial Commit

$ git remote -v
origin	../remote/ (fetch)
origin	../remote/ (push)

$ git status

On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

$ git log --stat
commit 498dda4b0ca033599960e404b4a02cadcbb65acc (HEAD -> master, origin/master)
Author: My Name <my@e.mail>
Date:   Sun Aug 9 15:44:46 2020 +0700

    Initial Commit
$ 
```

<br>
* Clone

Input (Cut and Paste):
```
cd ..
ls -l
git clone remote/ democlone
ls -l
ls -al demo/ democlone/
```

Output:
```
$ ls -l
total 16
drwxr-xr-x 3 demo demo 4096 Aug  9 14:53 demo
drwxr-xr-x 7 demo demo 4096 Aug  9 15:55 remote

$ git clone remote/ democlone
Cloning into 'democlone'...
done.

$ ls -l
total 12
drwxr-xr-x 3 demo demo 4096 Aug  9 14:53 demo
drwxr-xr-x 3 demo demo 4096 Aug  9 21:43 democlone
drwxr-xr-x 7 demo demo 4096 Aug  9 15:55 remote

$ ls -al demo/ democlone/
demo/:
total 12
drwxr-xr-x 3 demo demo 4096 Aug  9 14:53 .
drwxr-xr-x 5 demo demo 4096 Aug  9 21:43 ..
drwxr-xr-x 8 demo demo 4096 Aug  9 21:39 .git

democlone/:
total 12
drwxr-xr-x 3 demo demo 4096 Aug  9 21:43 .
drwxr-xr-x 5 demo demo 4096 Aug  9 21:43 ..
drwxr-xr-x 8 demo demo 4096 Aug  9 21:43 .git
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

