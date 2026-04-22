# Git Practice

## Description
This file records the steps I followed based on the given instructions to practice basic Git commands.

---

## Windows Powershell
```bash
PS D:\Wecamp> cd .\training-demo\
PS D:\Wecamp\training-demo> git init
Initialized empty Git repository in D:/Wecamp/training-demo/.git/
PS D:\Wecamp\training-demo> ni demo01.js


    Directory: D:\Wecamp\training-demo


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         4/22/2026   8:25 AM              0 demo01.js


PS D:\Wecamp\training-demo> echo 'console.log("Hello World!");' > demo01.js
PS D:\Wecamp\training-demo> git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        demo01.js

nothing added to commit but untracked files present (use "git add" to track)
PS D:\Wecamp\training-demo> git add .\demo01.js
PS D:\Wecamp\training-demo> git commit -m "Add demo01.js and print a greeting"
[master (root-commit) cadf493] Add demo01.js and print a greeting
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 demo01.js
PS D:\Wecamp\training-demo> git log
commit cadf493a4feb373dbfeaca1fc417efc82411fbb4 (HEAD -> master)
Author: ungdungthanhha <ungdungthanhha@gmail.com>
Date:   Wed Apr 22 08:26:46 2026 +0700

    Add demo01.js and print a greeting
PS D:\Wecamp\training-demo> git checkout -b feature/login
Switched to a new branch 'feature/login'
PS D:\Wecamp\training-demo> ni demo02.js


    Directory: D:\Wecamp\training-demo


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         4/22/2026   8:28 AM              0 demo02.js


PS D:\Wecamp\training-demo> git add .\demo02.js
PS D:\Wecamp\training-demo> git commit -m "Add demo02.js"
[feature/login f07afca] Add demo02.js
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 demo02.js
PS D:\Wecamp\training-demo> git branch
* feature/login
  master
PS D:\Wecamp\training-demo> git branch -m master main
PS D:\Wecamp\training-demo> git checkout main
Switched to branch 'main'
PS D:\Wecamp\training-demo> git branch
  feature/login
* main
PS D:\Wecamp\training-demo> git merge feature/login
Updating cadf493..f07afca
Fast-forward
 demo02.js | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 demo02.js
```

---

## Summary
I followed the instructions to initialize a Git repository, create and commit files, work with branches, and merge changes into the main branch.
