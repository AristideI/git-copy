
walte@Walter MINGW64 ~
$ cd d:

walte@Walter MINGW64 /d
$ cd The\ Gym/Gym-Git-Exercise-Solutions/

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ cd ..

walte@Walter MINGW64 /d/The Gym
$ mkdir git-copy

walte@Walter MINGW64 /d/The Gym
$ cd git-copy/

walte@Walter MINGW64 /d/The Gym/git-copy
$ git init
Initialized empty Git repository in D:/The Gym/git-copy/.git/

walte@Walter MINGW64 /d/The Gym/git-copy (master)
$ git branch -m master main

walte@Walter MINGW64 /d/The Gym/git-copy (main)
$ ls

walte@Walter MINGW64 /d/The Gym/git-copy (main)
$ git branch

walte@Walter MINGW64 /d/The Gym/git-copy (main)
$ touch home.html

walte@Walter MINGW64 /d/The Gym/git-copy (main)
$ git add .

walte@Walter MINGW64 /d/The Gym/git-copy (main)
$ git commit -m "adding new home page"
[main (root-commit) 56c2099] adding new home page
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 home.html

walte@Walter MINGW64 /d/The Gym/git-copy (main)
$ git push -u origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

walte@Walter MINGW64 /d/The Gym/git-copy (main)
$ git remote add origin https://github.com/AristideI/git-copy.git

walte@Walter MINGW64 /d/The Gym/git-copy (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 222 bytes | 222.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/AristideI/git-copy.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

walte@Walter MINGW64 /d/The Gym/git-copy (main)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

walte@Walter MINGW64 /d/The Gym/git-copy (ft/footer)
$ touch homes.html

walte@Walter MINGW64 /d/The Gym/git-copy (ft/footer)
$ git add .

walte@Walter MINGW64 /d/The Gym/git-copy (ft/footer)
$ git commit -m "first cahnges"
[ft/footer e7e94f0] first cahnges
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 homes.html

walte@Walter MINGW64 /d/The Gym/git-copy (ft/footer)
$ touch homee.html

walte@Walter MINGW64 /d/The Gym/git-copy (ft/footer)
$ git add .

walte@Walter MINGW64 /d/The Gym/git-copy (ft/footer)
$ git commit -m "second commit"
[ft/footer 364c08f] second commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 homee.html

walte@Walter MINGW64 /d/The Gym/git-copy (ft/footer)
$ git push origin ft/footer
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 420 bytes | 420.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/AristideI/git-copy/pull/new/ft/footer
remote:
To https://github.com/AristideI/git-copy.git
 * [new branch]      ft/footer -> ft/footer

walte@Walter MINGW64 /d/The Gym/git-copy (ft/footer)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

walte@Walter MINGW64 /d/The Gym/git-copy (main)
$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'

walte@Walter MINGW64 /d/The Gym/git-copy (ft/squashing)
$ git merge squash ft/footer
merge: squash - not something we can merge

walte@Walter MINGW64 /d/The Gym/git-copy (ft/squashing)
$ git merge ft/footer
Updating 56c2099..364c08f
Fast-forward
 homee.html | 0
 homes.html | 0
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 homee.html
 create mode 100644 homes.html

walte@Walter MINGW64 /d/The Gym/git-copy (ft/squashing)
$ git add .

walte@Walter MINGW64 /d/The Gym/git-copy (ft/squashing)
$ git commit -m "squashing the footer"
On branch ft/squashing
nothing to commit, working tree clean

walte@Walter MINGW64 /d/The Gym/git-copy (ft/squashing)
$ git push
fatal: The current branch ft/squashing has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/squashing

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


walte@Walter MINGW64 /d/The Gym/git-copy (ft/squashing)

