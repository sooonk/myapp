# myapp
Sample app - GIT

sonia@sonia-VB:/$ cd /home/sonia/Desktop/my\ app/ //przejście do danego folderu

sonia@sonia-VB:~/Desktop$ mv  my\ app/ myapp
sonia@sonia-VB:~/Desktop$ cd /home/sonia/Desktop/myapp/
sonia@sonia-VB:~/Desktop/myapp$ touch index.html
sonia@sonia-VB:~/Desktop/myapp$ touch app.js
sonia@sonia-VB:~/Desktop/myapp$ git init
Initialized empty Git repository in /home/sonia/Desktop/myapp/.git/
sonia@sonia-VB:~/Desktop/myapp$ git config --global user.name 'Sonia'
sonia@sonia-VB:~/Desktop/myapp$ git config --global user.emai 'sonia@przenioslo.eu'
sonia@sonia-VB:~/Desktop/myapp$ git add intex.html
fatal: pathspec 'intex.html' did not match any files
sonia@sonia-VB:~/Desktop/myapp$ git add index.html
sonia@sonia-VB:~/Desktop/myapp$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	app.js

sonia@sonia-VB:~/Desktop/myapp$ git rm --cached index.html
rm 'index.html'
sonia@sonia-VB:~/Desktop/myapp$ git add *.html
sonia@sonia-VB:~/Desktop/myapp$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	app.js

sonia@sonia-VB:~/Desktop/myapp$ git rm --cached index.html
rm 'index.html'
sonia@sonia-VB:~/Desktop/myapp$ git add .
sonia@sonia-VB:~/Desktop/myapp$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   app.js
	new file:   index.html

sonia@sonia-VB:~/Desktop/myapp$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   app.js
	new file:   index.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   index.html

sonia@sonia-VB:~/Desktop/myapp$ git add .
sonia@sonia-VB:~/Desktop/myapp$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   app.js
	new file:   index.html

sonia@sonia-VB:~/Desktop/myapp$ git commit

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

sonia@sonia-VB:~/Desktop/myapp$ git config --global user.email 'sonia@przenioslo.eu'
sonia@sonia-VB:~/Desktop/myapp$ git commit
Use "fg" to return to nano.or to close the file... 

[1]+  Stopped                 git commit
sonia@sonia-VB:~/Desktop/myapp$ git commit
Use "fg" to return to nano.or to close the file... 

[2]+  Stopped                 git commit
sonia@sonia-VB:~/Desktop/myapp$ git commit
[master (root-commit) 7aa9de0]  Initial commit
 2 files changed, 8 insertions(+)
 create mode 100644 app.js
 create mode 100644 index.html
sonia@sonia-VB:~/Desktop/myapp$ git status
On branch master
nothing to commit, working tree clean
sonia@sonia-VB:~/Desktop/myapp$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   app.js

no changes added to commit (use "git add" and/or "git commit -a")
sonia@sonia-VB:~/Desktop/myapp$ git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
	add
sonia@sonia-VB:~/Desktop/myapp$ git add .
sonia@sonia-VB:~/Desktop/myapp$ git commit 'changed app.js'
error: pathspec 'changed app.js' did not match any file(s) known to git.
sonia@sonia-VB:~/Desktop/myapp$ git commit -m  'changed app.js'
[master 973bad0] changed app.js
 1 file changed, 1 insertion(+)
sonia@sonia-VB:~/Desktop/myapp$ touch .gitignore
sonia@sonia-VB:~/Desktop/myapp$ ls
app.js  index.html
sonia@sonia-VB:~/Desktop/myapp$ ls a
ls: cannot access 'a': No such file or directory
sonia@sonia-VB:~/Desktop/myapp$ ls -a
.  ..  app.js  .git  .gitignore  index.html
sonia@sonia-VB:~/Desktop/myapp$ touch log.txt
sonia@sonia-VB:~/Desktop/myapp$ git add .
sonia@sonia-VB:~/Desktop/myapp$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   .gitignore

sonia@sonia-VB:~/Desktop/myapp$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   .gitignore

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	dir1/
	dir2/

sonia@sonia-VB:~/Desktop/myapp$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   .gitignore

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   .gitignore

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	dir1/

sonia@sonia-VB:~/Desktop/myapp$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   .gitignore

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   .gitignore

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	dir1/

sonia@sonia-VB:~/Desktop/myapp$ git add .
sonia@sonia-VB:~/Desktop/myapp$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   .gitignore
	new file:   dir1/app1.js

sonia@sonia-VB:~/Desktop/myapp$ git branch login
sonia@sonia-VB:~/Desktop/myapp$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   .gitignore
	new file:   dir1/app1.js

sonia@sonia-VB:~/Desktop/myapp$ git commit -m 'Another change'
[master 8fa4014] Another change
 2 files changed, 2 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 dir1/app1.js
sonia@sonia-VB:~/Desktop/myapp$ git checkout login
Switched to branch 'login'
sonia@sonia-VB:~/Desktop/myapp$ touch login.html
sonia@sonia-VB:~/Desktop/myapp$ git add .
sonia@sonia-VB:~/Desktop/myapp$ git commit -m 'login form'
[login 7a2f3c4] login form
 4 files changed, 3 insertions(+)
 create mode 100644 dir2/app2.js
 create mode 100644 log.txt
 create mode 100644 login.html
sonia@sonia-VB:~/Desktop/myapp$ git checkout master
Switched to branch 'master'
sonia@sonia-VB:~/Desktop/myapp$ git merge login
Merge made by the 'recursive' strategy.
 dir2/app2.js | 1 +
 index.html   | 1 +
 log.txt      | 1 +
 login.html   | 0
 4 files changed, 3 insertions(+)
 create mode 100644 dir2/app2.js
 create mode 100644 log.txt
 create mode 100644 login.html
sonia@sonia-VB:~/Desktop/myapp$ git commit -m "first commit"
On branch master
nothing to commit, working tree clean
sonia@sonia-VB:~/Desktop/myapp$ git remote add origin https://github.com/sooonk/myapp.git
sonia@sonia-VB:~/Desktop/myapp$ git push -u origin master
Username for 'https://github.com': sooonk
Password for 'https://sooonk@github.com': 
Counting objects: 19, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (12/12), done.
Writing objects: 100% (19/19), 1.49 KiB | 382.00 KiB/s, done.
Total 19 (delta 4), reused 0 (delta 0)
remote: Resolving deltas: 100% (4/4), done.
To https://github.com/sooonk/myapp.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
sonia@sonia-VB:~/Desktop/myapp$ git remote
origin
sonia@sonia-VB:~/Desktop/myapp$ git push -u origin master
Username for 'https://github.com': sooonk
Password for 'https://sooonk@github.com': 
remote: Invalid username or password.
fatal: Authentication failed for 'https://github.com/sooonk/myapp.git/'
sonia@sonia-VB:~/Desktop/myapp$ git push -u origin master
Username for 'https://github.com': sooonk
Password for 'https://sooonk@github.com': 
Branch 'master' set up to track remote branch 'master' from 'origin'.
Everything up-to-date
sonia@sonia-VB:~/Desktop/myapp$ ^C
sonia@sonia-VB:~/Desktop/myapp$ 
