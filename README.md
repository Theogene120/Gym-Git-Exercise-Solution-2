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

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ echo > home.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git add home.html
warning: in the working copy of 'home.html', LF will be replaced by CRLF the next time Git touches it

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 656dbef Some Code Add To README File

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ echo > about.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git add about.html
warning: in the working copy of 'about.html', LF will be replaced by CRLF the next time Git touches it

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 656dbef Some Code Add To README File

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git stash list
stash@{0}: WIP on main: 656dbef Some Code Add To README File
stash@{1}: WIP on main: 656dbef Some Code Add To README File

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ echo > team.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git add team.html
warning: in the working copy of 'team.html', LF will be replaced by CRLF the next time Git touches it

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 656dbef Some Code Add To README File

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git stash list
stash@{0}: WIP on main: 656dbef Some Code Add To README File
stash@{1}: WIP on main: 656dbef Some Code Add To README File
stash@{2}: WIP on main: 656dbef Some Code Add To README File

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git stash apply stash@{1}
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git stash apply stash@{3}
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git commit -m 'This Is The First Commit Of Stashed Files'
[main 3ecd5e0] This Is The First Commit Of Stashed Files
 2 files changed, 23 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git push -u origin main
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 16 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (7/7), 990 bytes | 990.00 KiB/s, done.
Total 7 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
   3009838..3ecd5e0  main -> main
branch 'main' set up to track 'origin/main'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git stash pop
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped refs/stash@{0} (29dfde42bb7aa1353bff2032ba192dd5664b67c9)

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git reset --hard
HEAD is now at 3ecd5e0 This Is The First Commit Of Stashed Files

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git stash list

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

```
## Bundle 2

### Exercise 1

```bash

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git branch ft/bundle-2

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git checkout ft/bundle-2
M       README.md
Switched to branch 'ft/bundle-2'

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/bundle-2)
$ echo > services.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/bundle-2)
$ git add services.html
warning: in the working copy of 'services.html', LF will be replaced by CRLF the next time Git touches it

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/bundle-2)
$ git commit -m 'Service Page Added'
[ft/bundle-2 00d9fdd] Service Page Added
 1 file changed, 16 insertions(+)
 create mode 100644 services.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/bundle-2)
$  git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 508 bytes | 254.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Theogene120/Gym-Git-Exercise-Solution/pull/new/ft/bundle-2
remote:
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
 
 ```
### Exercise 2

```bash

user@LAPTOP-GQ4K54L5 MINGW64 ~
$ cd Git-Exercises

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ code .

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git pull origin
Already up to date.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git branch ft/service-redesign

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/service-redesign)
$ git checkout ft/bundle-2
Switched to branch 'ft/bundle-2'
Your branch is up to date with 'origin/ft/bundle-2'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/service-redesign)
$ git add services.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/service-redesign)
$ git commit -m "Two Services Added On Service File"
[ft/service-redesign e2fa7df] Two Services Added On Service File
 1 file changed, 2 insertions(+)

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 16 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 672 bytes | 224.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Theogene120/Gym-Git-Exercise-Solution/pull/new/ft/service-redesign
remote:
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git add services.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git commit -m "Two Services Add To The Service File"
[main 8b44e9f] Two Services Add To The Service File
 1 file changed, 2 insertions(+)

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 372 bytes | 372.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
   a144c54..8b44e9f  main -> main

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/service-redesign)
$ git diff main ft/service-redesign
diff --git a/services.html b/services.html
index 186e4a4..1b816a8 100644
--- a/services.html
+++ b/services.html
@@ -11,8 +11,8 @@
         <li>Mobile App Development</li>
         <li>Wev App Development</li>
         <li>System Development</li>
-        <li>Electronic Divice Repair</li>
-        <li>Computer Supply From Dubai</li>
+        <li>Software Development Trainings</li>
+        <li>CCTV Camera Installation And Mentainance</li>
     </ol>
 </body>
 </html>

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git merge ft/service-redesign
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main|MERGING)
$ git add services.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main|MERGING)
$ git commit -m "Conflict solved"
[main 920fe56] Conflict solved

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git push
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 221 bytes | 221.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
   8b44e9f..920fe56  main -> main

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git merge ft/service-redesign
Already up to date.

```

## Bundle-3

### Exercise-1

```bash
user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/team-page)
$ echo team.html
team.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/team-page)
$ echo > team.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/team-page)
$ git add team.html
warning: in the working copy of 'team.html', LF will be replaced by CRLF the next time Git touches it

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/team-page)
$ git commit -m "Instruction to join the team"
[ft/team-page d224911] Instruction to join the team
 1 file changed, 11 insertions(+)
 create mode 100644 team.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 470 bytes | 235.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Theogene120/Gym-Git-Exercise-Solution/pull/new/ft/team-page
remote:
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/team-page)
$ git log
commit d2249119dbc093ff1cc8d8097fc0299f90d3e821 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Theogene <igiranezatheogene4@gmail.com>
Date:   Thu Jul 31 11:17:23 2025 +1100

    Instruction to join the team

commit e200ddf21ab8b630935c2d8ec5c44747eac97090 (origin/main, origin/HEAD, main, ft/contact-page)
Author: Theogene <igiranezatheogene4@gmail.com>
Date:   Thu Jul 31 09:32:00 2025 +1100

    Solution Of Bundle 2 Exercise 2 Added

commit 920fe56c770897623cfe48195ddc14a7c5e9b221
Merge: 8b44e9f e2fa7df
Author: Theogene <igiranezatheogene4@gmail.com>
Date:   Thu Jul 31 08:51:39 2025 +1100

    Conflict solved

commit 8b44e9fe8e8f354a0d73e79cacd8ceff247a6b49
Author: Theogene <igiranezatheogene4@gmail.com>
Date:   Thu Jul 31 08:32:56 2025 +1100

    Two Services Add To The Service File

commit e2fa7dfdd096978eb7b292ec44535e9772a23984 (origin/ft/service-redesign, ft/service-redesign)
Author: Theogene <igiranezatheogene4@gmail.com>
Date:   Thu Jul 31 08:23:18 2025 +1100

    Two Services Added On Service File

commit fd0ea9c386b7de7fd5803e056f891c1f7e1742b3
Merge: a144c54 00d9fdd
Author: Theogene <igiranezatheogene4@gmail.com>
Date:   Thu Jul 31 08:11:07 2025 +1100

    I Merge branch 'ft/bundle-2' to main to have service file

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/contact-page)
$ git cherry-pick d2249119dbc093ff1cc8d8097fc0299f90d3e821
[ft/contact-page 733d577] Instruction to join the team
 Date: Thu Jul 31 11:17:23 2025 +1100
 1 file changed, 11 insertions(+)
 create mode 100644 team.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/contact-page)
$ git echo > contact.html
git: 'echo' is not a git command. See 'git --help'.

The most similar command is
        fetch

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/contact-page)
$ git add contact.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/contact-page)
$ git commit -m "Contact page is added"
[ft/contact-page 3e64832] Contact page is added
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 16 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 767 bytes | 191.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/Theogene120/Gym-Git-Exercise-Solution/pull/new/ft/contact-page
remote:
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.


user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/faq-page)
$ echo > faq.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/faq-page)
$ git add faq.html
warning: in the working copy of 'faq.html', LF will be replaced by CRLF the next time Git touches it

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/faq-page)
$ git commit -m "faq file added to the project"
[ft/faq-page 9beda4f] faq file added to the project
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 440 bytes | 440.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Theogene120/Gym-Git-Exercise-Solution/pull/new/ft/faq-page
remote:
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.


user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/faq-page)
$ git revert d2249119dbc093ff1cc8d8097fc0299f90d3e821
[ft/faq-page 4dfb8b9] Revert "Instruction to join the team"
 1 file changed, 11 deletions(-)
 delete mode 100644 team.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/faq-page)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 296 bytes | 296.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
   9beda4f..4dfb8b9  ft/faq-page -> ft/faq-page
 
 ```

 ### Exercise-2

```bash
user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'
Your branch is up to date with 'origin/ft/faq-page'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        fro-change-main.html

nothing added to commit but untracked files present (use "git add" to track)

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git add fro-change-main.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git commit -m "This file is for making change to main branch"
[main 2b53e17] This file is for making change to main branch
 1 file changed, 11 insertions(+)
 create mode 100644 fro-change-main.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 475 bytes | 475.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
   bde19f3..2b53e17  main -> main

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/home-page-redesign)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/home-page-redesign)
$ git add home.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/home-page-redesign)
$ git commit -m 'Some changes made to the home page'
[ft/home-page-redesign 740cc6c] Some changes made to the home page
 1 file changed, 1 insertion(+)

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 16 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (14/14), 1.57 KiB | 321.00 KiB/s, done.
Total 14 (delta 8), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (8/8), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/Theogene120/Gym-Git-Exercise-Solution/pull/new/ft/home-page-redesign
remote:
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

```

## Bundle-4

### Exercise-1

```bash

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/contact-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git remote add origin git@github.com:Theogene120/Gym-Git-Exercise-Solution-2.git
error: remote origin already exists.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git remote add git-copy git@github.com:Theogene120/Gym-Git-Exercise-Solution-2.git

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git add home.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git commit -m "Change Add After Adding New Remote"
[main f4a89f9] Change Add After Adding New Remote
 1 file changed, 1 insertion(+)

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git push git-copy main
Enumerating objects: 58, done.
Counting objects: 100% (58/58), done.
Delta compression using up to 16 threads
Compressing objects: 100% (57/57), done.
Writing objects: 100% (58/58), 10.22 KiB | 872.00 KiB/s, done.
Total 58 (delta 25), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (25/25), done.
To github.com:Theogene120/Gym-Git-Exercise-Solution-2.git
 * [new branch]      main -> main

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 381 bytes | 381.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
   a31c2c5..f4a89f9  main -> main

```
### Exercise-2

```bash
user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/footer)
$ echo > footer.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/footer)
$ git add footer.html
warning: in the working copy of 'footer.html', LF will be replaced by CRLF the next time Git touches it

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/footer)
$ git commit -m "Footer File Added"
[ft/footer 586be2e] Footer File Added
 1 file changed, 11 insertions(+)
 create mode 100644 footer.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/footer)
$ git status
On branch ft/footer
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   footer.html

no changes added to commit (use "git add" and/or "git commit -a")

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/footer)
$ git add footer.html
warning: in the working copy of 'footer.html', LF will be replaced by CRLF the next time Git touches it

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/footer)
$ git commit -m "More Changes Added On Footer File"
[ft/footer 4a8dceb] More Changes Added On Footer File
 1 file changed, 1 insertion(+)

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/footer)
$ git push
fatal: The current branch ft/footer has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/footer

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/footer)
$ git push --set-upstream origin ft/footer
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 16 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 773 bytes | 257.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/Theogene120/Gym-Git-Exercise-Solution/pull/new/ft/footer
remote:
To github.com:Theogene120/Gym-Git-Exercise-Solution.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/footer)
$ git push --set-upstream git-copy ft/footer
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 16 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 773 bytes | 773.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/Theogene120/Gym-Git-Exercise-Solution-2/pull/new/ft/footer
remote:
To github.com:Theogene120/Gym-Git-Exercise-Solution-2.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'git-copy/ft/footer'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/footer)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (main)
$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/squashing)
$ git merge --squash ft/footer
Updating 4326a6d..4a8dceb
Fast-forward
Squash commit -- not updating HEAD
 footer.html | 12 ++++++++++++
 1 file changed, 12 insertions(+)
 create mode 100644 footer.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/squashing)
$ git commit -m "Footer Changes Squashing"
[ft/squashing 0cb1dc8] Footer Changes Squashing
 1 file changed, 12 insertions(+)
 create mode 100644 footer.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/squashing)
$ git push git-copy main
Everything up-to-date

user@LAPTOP-GQ4K54L5 MINGW64 ~/Git-Exercises (ft/squashing)
$ git push git-copy ft/squashing
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 497 bytes | 248.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/Theogene120/Gym-Git-Exercise-Solution-2/pull/new/ft/squashing
remote:
To github.com:Theogene120/Gym-Git-Exercise-Solution-2.git
 * [new branch]      ft/squashing -> ft/squashing

```