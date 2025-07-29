# Git Exercise

## Bundle 1

### Exercise 1

```bash

user@LAPTOP-GQ4K54L5 MINGW64 ~
$ pwd
/c/Users/user

user@LAPTOP-GQ4K54L5 MINGW64 ~
$ mkdir git-exercises

user@LAPTOP-GQ4K54L5 MINGW64 ~
$ cd git-exercises

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises
$ git init
Initialized empty Git repository in C:/Users/user/git-exercises/.git/

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (master)
$ code .

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (master)
$ git branch -m master main

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (main)
$ git add --all

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (main)
$ git commit -m "This Is The First Change"
[main (root-commit) e81119a] This Is The First Change
 1 file changed, 12 insertions(+)
 create mode 100644 index.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (main)
$ git add README.md

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (main)
$ git commit -m "The README File Add To Keep Track Of The Bash Code"
[main 36de133] The README File Add To Keep Track Of The Bash Code
 1 file changed, 7 insertions(+)
 create mode 100644 README.md

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (main)
$ git remote add origin git@github.com:Theogene120/Gym-Git-Exercise-Solution.git




user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (main)
$ git branch dev

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (main)
$ git branch
  dev
* main

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (main)
$ git checkout dev
M       README.md
Switched to branch 'dev'

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (dev)
$ git branch test

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (dev)
$ git branch
* dev
  main
  test

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (dev)
$ git branch -d test
Deleted branch test (was 36de133).

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (dev)
$ git branch
* dev
  main



```