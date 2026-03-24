Initial commit on main

User@216-17 MINGW64 ~
$ git clone https://github.com/tumpen11/soril1.git
Cloning into 'soril1'...
warning: You appear to have cloned an empty repository.

User@216-17 MINGW64 ~
$ cd soril1

User@216-17 MINGW64 ~/soril1 (main)
$ echo "My project" > README.md

User@216-17 MINGW64 ~/soril1 (main)
$ git add README.md
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

User@216-17 MINGW64 ~/soril1 (main)
$ git commit -m "Add README"
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'User@216-17.(none)')

User@216-17 MINGW64 ~/soril1 (main)
$ git config user.email "mmigaa434@gmail.com"

User@216-17 MINGW64 ~/soril1 (main)
$ git config user.name "mygmarjav"

User@216-17 MINGW64 ~/soril1 (main)
$ git checkout -b feature-test
Switched to a new branch 'feature-test'

User@216-17 MINGW64 ~/soril1 (feature-test)
$ echo "Git PR туршилт" >> README.md

User@216-17 MINGW64 ~/soril1 (feature-test)
$ git add README.md
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

User@216-17 MINGW64 ~/soril1 (feature-test)
$ git commit -m "Add PR test text"
[feature-test (root-commit) 00c020a] Add PR test text
 1 file changed, 2 insertions(+)
 create mode 100644 README.md

User@216-17 MINGW64 ~/soril1 (feature-test)
$ git push origin feature-test
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 252 bytes | 252.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/tumpen11/soril1.git
 * [new branch]      feature-test -> feature-test

User@216-17 MINGW64 ~/soril1 (feature-test)
$ git push -u origin feature-test
branch 'feature-test' set up to track 'origin/feature-test'.
Everything up-to-date

User@216-17 MINGW64 ~/soril1 (feature-test)
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/tumpen11/soril1.git'

User@216-17 MINGW64 ~/soril1 (feature-test)
$ git checkout -b main
Switched to a new branch 'main'
Your branch is based on 'origin/main', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

User@216-17 MINGW64 ~/soril1 (main)
$ echo "Initial commit on main" > README.md

User@216-17 MINGW64 ~/soril1 (main)
$ git add README.md
warning: in the working copy of 'README.md', LF will be replaced by CRLF the nex

User@216-17 MINGW64 ~/soril1 (main)
$ git commit -m "Initial commit on main"
[main 982db57] Initial commit on main
 1 file changed, 1 insertion(+), 2 deletions(-)

User@216-17 MINGW64 ~/soril1 (main)
$ git push -u origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 270 bytes | 270.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'main' on GitHub by visiting:
remote:      https://github.com/tumpen11/soril1/pull/new/main
remote:
To https://github.com/tumpen11/soril1.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

User@216-17 MINGW64 ~/soril1 (main)
$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.

User@216-17 MINGW64 ~/soril1 (main)
$ git pull origin main
From https://github.com/tumpen11/soril1
 * branch            main       -> FETCH_HEAD
Already up to date.

User@216-17 MINGW64 ~/soril1 (main)
$ git log --oneline --graph
* 982db57 (HEAD -> main, origin/main) Initial commit on main
* 00c020a (origin/feature-test, feature-test) Add PR test text

User@216-17 MINGW64 ~/soril1 (main)
