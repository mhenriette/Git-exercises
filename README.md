# Git Exercises
## bundle 1
### exercise one
```bash
$ ls 
README.md

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise
$ git init 
Initialized empty Git repository in C:/Users/TheGym/Documents/The Gym/Git-Exercise/.git/

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (master)
$ git branch

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (master)
$ git branch main
fatal: not a valid object name: 'master'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (master)
$ git branch -m main

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git branch

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git stage
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Turn this message off by running
hint: "git config advice.addEmptyPathspec false"

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git add README.md 
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git commit -m 'First commit'
[main (root-commit) 2b9d3a1] First commit
 1 file changed, 3 insertions(+)
 create mode 100644 README.md

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git remote add origin https://github.com/mhenriette/Git-Exercises.git

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git push 
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git push origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 249 bytes | 124.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/mhenriette/Git-Exercises.git
 * [new branch]      main -> main

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git status 
On branch main
nothing to commit, working tree clean

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git stage 
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Turn this message off by running
hint: "git config advice.addEmptyPathspec false"

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git checkout -b dev
Switched to a new branch 'dev'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git checkout -b test
Switched to a new branch 'test'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (test)
$ git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/mhenriette/Git-Exercises/pull/new/test
remote:
To https://github.com/mhenriette/Git-Exercises.git
 * [new branch]      test -> test

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (test)
$ git checkout dev
Switched to branch 'dev'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git push origin dev 
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/mhenriette/Git-Exercises/pull/new/dev
remote:
To https://github.com/mhenriette/Git-Exercises.git
 * [new branch]      dev -> dev

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git branch -D test 
Deleted branch test (was 2b9d3a1).

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git push origin --delete test
To https://github.com/mhenriette/Git-Exercises.git
 - [deleted]         test
```
### Exercise 2 

```bash
$ ls
home.html  README.md

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git status 
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git add home.html 

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git status 
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html


TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git stash
Saved working directory and index state WIP on dev: 923f8e3 exercise one

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git stash list 
stash@{0}: WIP on dev: 923f8e3 exercise one

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git stash
No local changes to save

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git add about.html 

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git stash
Saved working directory and index state WIP on dev: 923f8e3 exercise one

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git stash list 
stash@{0}: WIP on dev: 923f8e3 exercise one
stash@{1}: WIP on dev: 923f8e3 exercise one

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git add team.html

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git stash
Saved working directory and index state WIP on dev: 923f8e3 exercise one

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git list stash
git: 'list' is not a git command. See 'git --help'.

The most similar commands are
        bisect
        rev-list

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git stash list 
stash@{0}: WIP on dev: 923f8e3 exercise one
stash@{1}: WIP on dev: 923f8e3 exercise one
stash@{2}: WIP on dev: 923f8e3 exercise one

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (de863c6cd9a963287a413f7c976cf0ad28a9db15)

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git stash list
stash@{0}: WIP on dev: 923f8e3 exercise one
stash@{1}: WIP on dev: 923f8e3 exercise one

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (03aa950d1a532882a336af8318850e5278a655c8)

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git status 
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html


TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git add .

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git commit -m 'about and home page '
[dev bee007b] about and home page
 2 files changed, 26 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git push origin dev 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 549 bytes | 274.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/mhenriette/Git-Exercises.git
   923f8e3..bee007b  dev -> dev

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git status 
On branch dev
nothing to commit, working tree clean

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ ls
about.html  home.html  README.md

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git stash pop 
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (bdeeb0fd971758df434eec2cc216a2b6afc46d68)

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html


TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git reset --hard 
HEAD is now at bee007b about and home page
```

## Bundle 2 
### Exercise 1

```bash
git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/bundle-2)
$ git status
On branch ft/bundle-2
nothing to commit, working tree clean

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/bundle-2)
$ git add services.html 

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/bundle-2)
$ git commit -m 'added service page '
[ft/bundle-2 ca026dc] added service page
 1 file changed, 13 insertions(+)
 create mode 100644 services.html

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/bundle-2)
$ git push origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 471 bytes | 235.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/mhenriette/Git-Exercises/pull/new/ft/bundle-2
remote:
To https://github.com/mhenriette/Git-Exercises.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/bundle-2)
$
```
