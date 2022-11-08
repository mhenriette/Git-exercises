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
### Exercise 2 

```bash
TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (dev)
$ git checkout main
Switched to branch 'main'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git pull origin main
From https://github.com/mhenriette/Git-Exercises
 * branch            main       -> FETCH_HEAD
Updating 2b9d3a1..2e12323
Fast-forward
 README.md     | 341 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 about.html    |  13 +++
 home.html     |  13 +++
 services.html |  13 +++
 4 files changed, 380 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 services.html

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* main

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git branch -D ft/service-redesign 
Deleted branch ft/service-redesign (was 2b9d3a1).

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git branch
  dev
  ft/bundle-2
* main

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git add .

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git commit -m 'added changes to service file'
[ft/service-redesign 83cdd48] added changes to service file
 1 file changed, 9 insertions(+)

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git push origin ft/service-redesign 
fatal: unable to access 'https://github.com/mhenriette/Git-Exercises.git/': Failed to connect to github.com port 443 after 21118 ms: Timed out

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git push origin ft/service-redesign 
fatal: unable to access 'https://github.com/mhenriette/Git-Exercises.git/': OpenSSL SSL_read: Connection was reset, errno 10054

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git push origin ft/service-redesign 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 411 bytes | 411.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/mhenriette/Git-Exercises/pull/new/ft/service-redesign
remote:
To https://github.com/mhenriette/Git-Exercises.git
 * [new branch]      ft/service-redesign -> ft/service-redesign

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ ls -a
./  ../  .git/  about.html  home.html  README.md  services.html

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git status 
On branch ft/service-redesign
nothing to commit, working tree clean

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git checkout main
Switched to branch 'main'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git checkout 

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git status
On branch main
nothing to commit, working tree clean

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git add .

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git commit -m 'added different changes on main'
[main a6e09a3] added different changes on main
 1 file changed, 6 insertions(+), 1 deletion(-)

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 380 bytes | 190.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/mhenriette/Git-Exercises.git
   2e12323..a6e09a3  main -> main

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git checkout ft/service-redesign 
Switched to branch 'ft/service-redesign'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git status 
On branch ft/service-redesign
nothing to commit, working tree clean

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git diff

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git diff ?

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git diff main
diff --git a/services.html b/services.html
index ec30e19..1ac01dc 100644
--- a/services.html
+++ b/services.html
@@ -7,12 +7,16 @@
     <title>Services</title>
 </head>
 <body>
-    <h1>this is the old Services page</h1>
+    <h1>this is the Services page</h1>
+    <h1>These are the Services </h1>
+
+
diff --git a/services.html b/services.html
index ec30e19..1ac01dc 100644
--- a/services.html
+++ b/services.html
@@ -7,12 +7,16 @@
     <title>Services</title>
 </head>
 <body>
-    <h1>this is the old Services page</h1>
+    <h1>this is the Services page</h1>
+    <h1>These are the Services </h1>
+
     <ul>
-        <li>OUR SERVICES:</li>
...skipping...
     <ul>
-        <li>OUR SERVICES:</li>
-        <li>Fix Computers</li>
-    </ul>
+        <li>Sell phones </li>
+        <li>Sell computers </li>
+        <li>make softwares </li>
+        <li>Install Internet</li>

+    </ul>



TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign|MERGING)
$ git merge main
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign|MERGING)
$ git merge main
Already up to date.

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git add .

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git status 
On branch ft/service-redesign
nothing to commit, working tree clean

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git status 
On branch ft/service-redesign
nothing to commit, working tree clean

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git commit -m 'resolved conflicts'
On branch ft/service-redesign
nothing to commit, working tree clean

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git status
On branch ft/service-redesign
nothing to commit, working tree clean

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git add .

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git status 
On branch ft/service-redesign
nothing to commit, working tree clean

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git merge 
fatal: No remote for the current branch.

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git diff

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git diff main
diff --git a/services.html b/services.html
index ec30e19..c3818b9 100644
--- a/services.html
+++ b/services.html
@@ -7,12 +7,7 @@
     <title>Services</title>
 </head>
 <body>
-    <h1>this is the old Services page</h1>
-    <ul>
-        <li>OUR SERVICES:</li>
-        <li>Fix Computers</li>
-    </ul>
-

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git merge main
Already up to date.

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git add .

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git commit -m 'resolved conflicts '
On branch ft/service-redesign
nothing to commit, working tree clean

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git push origin ft/service-redesign 
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 344 bytes | 86.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/mhenriette/Git-Exercises.git
   83cdd48..b3580a2  ft/service-redesign -> ft/service-redesign

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/service-redesign)
$ git checkout main
Switched to branch 'main'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$
```



# Bundle 3

## Exercise 1

```bash
TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git status 
On branch main
nothing to commit, working tree clean

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/team-page)
$ git add .

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/team-page)
$ git commit -m 'created team file '
[ft/team-page dee64ea] created team file
 1 file changed, 13 insertions(+)
 create mode 100644 team.html

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/team-page)
$ git push origin ft/team-page 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 471 bytes | 235.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/mhenriette/Git-Exercises/pull/new/ft/team-page
remote:
To https://github.com/mhenriette/Git-Exercises.git
 * [new branch]      ft/team-page -> ft/team-page

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/team-page)
$ git checkout main
Switched to branch 'main'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/contact-page)
$ git checkout ft/team-page 
Switched to branch 'ft/team-page'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/team-page)
$ git log 
commit dee64eaa64c4c51413107b638aa8de5f1e2c7fbb (HEAD -> ft/team-page, origin/ft/team-page)
Author: mhenriette <mhenriette00@gnmail.com>
Date:   Mon Nov 7 13:17:15 2022 +0200

    created team file

commit f59b8f81bfd85d035548fd3100d2c454c775920b (origin/main, main, ft/contact-page)
Author: mhenriette <mhenriette00@gnmail.com>
Date:   Mon Nov 7 13:09:08 2022 +0200

    added exercise 2 in Readme file

commit a6e09a35bf0fad3a8c028ac5b142799797075819
Author: mhenriette <mhenriette00@gnmail.com>

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/team-page)
$ git checkout ft/contact-page 
Switched to branch 'ft/contact-page'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/contact-page)
$ git cherry-pick dee64eaa64c4c51413107b638aa8de5f1e2c7fbb1
fatal: bad revision 'dee64eaa64c4c51413107b638aa8de5f1e2c7fbb1'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/contact-page)
$ git cherry-pick dee64eaa64c4c51413107b638aa8de5f1e2c7fbb
[ft/contact-page ad9c29e] created team file
 Date: Mon Nov 7 13:17:15 2022 +0200
 1 file changed, 13 insertions(+)
 create mode 100644 team.html

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/contact-page)
$ git add .

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/contact-page)
$ git commit -m 'added Contact page'
[ft/contact-page 2826874] added Contact page
 1 file changed, 13 insertions(+)
 create mode 100644 contact.html

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/contact-page)
$ git  push origin ft/contact-page 
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 742 bytes | 371.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/mhenriette/Git-Exercises/pull/new/ft/contact-page
remote:
To https://github.com/mhenriette/Git-Exercises.git
 * [new branch]      ft/contact-page -> ft/contact-page

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/faq-page)
$ ls
about.html  contact.html  home.html  README.md  services.html  team.html

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/faq-page)
$ git add .

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/faq-page)
$ git commit -m 'added faq page '
[ft/faq-page 46468de] added faq page
 1 file changed, 13 insertions(+)
 create mode 100644 faq.html

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/faq-page)
$ git push origin ft/faq-page 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 459 bytes | 229.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/mhenriette/Git-Exercises/pull/new/ft/faq-page
remote:
To https://github.com/mhenriette/Git-Exercises.git
 * [new branch]      ft/faq-page -> ft/faq-page

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/faq-page)
$ git revert dee64eaa64c4c51413107b638aa8de5f1e2c7fbb
[ft/faq-page 2d9ec19] Revert "created team file"
 1 file changed, 13 deletions(-)
 delete mode 100644 team.html

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/faq-page)
$ git add .

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/faq-page)
$ git commit -m 'reverted last commit of team page '
On branch ft/faq-page
nothing to commit, working tree clean

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/faq-page)
$ git origin push ft/faq-page
git: 'origin' is not a git command. See 'git --help'.

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/faq-page)
$ git push origin ft/faq-page 
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 270 bytes | 135.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/mhenriette/Git-Exercises.git
   46468de..2d9ec19  ft/faq-page -> ft/faq-page

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/faq-page)
$
```

### Exercise 2 
```bash
TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/service-redesign
  ft/team-page
* main

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/home-page-redesign)
$ git checkout main 
Switched to branch 'main'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git add .

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git commit 'made changes on home page'
error: pathspec 'made changes on home page' did not match any file(s) known to git

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git commit -m  'made changes on home page'
[main 3ce6451] made changes on home page
 1 file changed, 1 insertion(+)

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 308 bytes | 154.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/mhenriette/Git-Exercises.git
   d1488bc..3ce6451  main -> main

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$ git checkout ft/home-page-redesign 
Switched to branch 'ft/home-page-redesign'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/home-page-redesign)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/home-page-redesign)
$ git add .

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/home-page-redesign)
$ git commit -m 'added changes on home page via ft/home-page-redesign'
[ft/home-page-redesign 163cf4d] added changes on home page via ft/home-page-redesign
 1 file changed, 2 insertions(+), 1 deletion(-)

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/home-page-redesign)
$ git push origin main
Everything up-to-date

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/home-page-redesign)
$ git push origin ft/home-page-redesign 
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 4 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (14/14), 1.59 KiB | 271.00 KiB/s, done.
Total 14 (delta 7), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (7/7), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/mhenriette/Git-Exercises/pull/new/ft/home-page-redesign
remote:
To https://github.com/mhenriette/Git-Exercises.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'

TheGym@DESKTOP-829KDOL MINGW64 ~/Documents/The Gym/Git-Exercise (main)
$
```
