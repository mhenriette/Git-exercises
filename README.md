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
