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
  
