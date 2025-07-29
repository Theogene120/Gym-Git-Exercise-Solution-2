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

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git add README.md

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git commit -m "Some Code Added To README File"
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git push -u origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 816 bytes | 408.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
   36de133..d4e3180  main -> main
branch 'main' set up to track 'origin/main'.


user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (main)
$ git branch dev

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git push origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Theogene120/Gym-Git-Exercise-Solution/pull/new/dev
remote:
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
 * [new branch]      dev -> dev

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

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (dev)
$ git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/Theogene120/Gym-Git-Exercise-Solution/pull/new/test
remote:
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
 * [new branch]      test -> test

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (dev)
$ git branch
* dev
  main
  test

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (dev)
$ git branch -d test
Deleted branch test (was 36de133).

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (dev)
$ git push origin --delete test
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
 - [deleted]         test

user@LAPTOP-GQ4K54L5 MINGW64 ~/git-exercises (dev)
$ git branch
* dev
  main
```

### Exercise 2

```bash
