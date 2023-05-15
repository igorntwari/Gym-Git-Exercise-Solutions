# Gym-Git-Exercise-Solutions
my terminal solution history
 ......bundle-1
  ######################################################################### exercise-1########################################################################
  ...>bash 
  
User@ntwali MINGW64 ~/Desktop/github-excercise
$ git init 
Initialized empty Git repository in C:/Users/User/Desktop/github-excercise/.git/

User@ntwali MINGW64 ~/Desktop/github-excercise (master)
$ git branch -M main

User@ntwali MINGW64 ~/Desktop/github-excercise (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        READ-ME.md
        index.html

nothing added to commit but untracked files present (use "git add" to track)

User@ntwali MINGW64 ~/Desktop/github-excercise (main)
$ git add .

User@ntwali MINGW64 ~/Desktop/github-excercise (main)
$ git commit -m "added 2 files"
[main (root-commit) df7f5b4] added 2 files
 2 files changed, 14 insertions(+)
 create mode 100644 READ-ME.md
 create mode 100644 index.html

User@ntwali MINGW64 ~/Desktop/github-excercise (main)
$ git remote add origin https://github.com/igorntwari/git-exercises.git

User@ntwali MINGW64 ~/Desktop/github-excercise (main)
$ git push -u origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 482 bytes | 241.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/igorntwari/git-exercises.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

User@ntwali MINGW64 ~/Desktop/github-excercise (main)
$ git checkout -b dev 
Switched to a new branch 'dev'

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git push 
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$  git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/igorntwari/git-exercises/pull/new/dev
remote:
To https://github.com/igorntwari/git-exercises.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git checkout -b test
Switched to a new branch 'test'

User@ntwali MINGW64 ~/Desktop/github-excercise (test)
$ push orgin test
bash: push: command not found

User@ntwali MINGW64 ~/Desktop/github-excercise (test)
$ git push orgin test 
fatal: 'orgin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

User@ntwali MINGW64 ~/Desktop/github-excercise (test)
$ git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/igorntwari/git-exercises/pull/new/test
remote:
To https://github.com/igorntwari/git-exercises.git
 * [new branch]      test -> test

User@ntwali MINGW64 ~/Desktop/github-excercise (test)
$ git checkout dev 
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git branch -D test
Deleted branch test (was df7f5b4).

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git push origin -d test
To https://github.com/igorntwari/git-exercises.git
 - [deleted]         test

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$
  ########################################################################### end of exercise-1#################################################################
   exercises-1
 >bash
 User@ntwali MINGW64 ~/Desktop/github-excercise (exercise-2)
$ git checkout dev 
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ touch home.html

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git add .

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html


User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git stash
Saved working directory and index state WIP on dev: df7f5b4 added 2 files

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git stash list
stash@{0}: WIP on dev: df7f5b4 added 2 files
stash@{1}: On exercise-2: added home.html file

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ touch about.html

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git add about.html

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git stash
Saved working directory and index state WIP on dev: df7f5b4 added 2 files

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git stash list
stash@{0}: WIP on dev: df7f5b4 added 2 files
stash@{1}: WIP on dev: df7f5b4 added 2 files
stash@{2}: On exercise-2: added home.html file

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ touch team.html

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git add team.html

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git stash
Saved working directory and index state WIP on dev: df7f5b4 added 2 files

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git stash list
stash@{0}: WIP on dev: df7f5b4 added 2 files
stash@{1}: WIP on dev: df7f5b4 added 2 files
stash@{2}: WIP on dev: df7f5b4 added 2 files
stash@{3}: On exercise-2: added home.html file

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git pop stash@{1}
git: 'pop' is not a git command. See 'git --help'.

The most similar command is
        log

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (8bbca9682b34641e8987ab40b7a0bb04f2f8fa79)

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git stash list
stash@{0}: WIP on dev: df7f5b4 added 2 files
stash@{1}: WIP on dev: df7f5b4 added 2 files
stash@{2}: On exercise-2: added home.html file

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (292f87568c904203dcfd30033c72689fe7e3afb2)

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git add .

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git commit -m "added home and about pages"
[dev 08c1390] added home and about pages
 2 files changed, 22 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 599 bytes | 299.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/igorntwari/git-exercises.git
   df7f5b4..08c1390  dev -> dev

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git stash list
stash@{0}: WIP on dev: df7f5b4 added 2 files
stash@{1}: On exercise-2: added home.html file

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (811e0d9043d3411989c2e37f2375d4aa1e964bbf)

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$ git reset --hard
HEAD is now at 08c1390 added home and about pages

User@ntwali MINGW64 ~/Desktop/github-excercise (dev)
$
 
 
 ................................................................end of exercise number 2
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
