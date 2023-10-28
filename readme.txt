git init  -> set the working directory
ls -a
git status

it shows:
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        chapter1.txt

nothing added to commit but untracked files present (use "git add" to track)

git add chapter1.txt  --> add the file to staging area

git status
it shows:
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   chapter1.txt

git config user.email "daveleesk@gmail.com"
git config user.name "Dave"

git commit -"Complete chapter1"

git log
it shows:
commit 778fae96451bc2a207adfbee84786167e61ffe21 (HEAD -> master)
Author: Dave <daveleesk@gmail.com>
Date:   Thu Oct 26 11:07:45 2023 +0800

    Complete chapter1

git checkout <file>

git diff <file>

For upload local repository to remote repository in GitHub:

at working directory (1st setup)
git remote add origin https://github.com/Daveleesk/GIT-demo.git
git branch -M main
git push -u origin main  (for subsequent changes)

git rm --cached -r .   : to remove files from staging -r:recursive

To ignore file:
1. create file .gitignore
2. add file name in .gitignore

git clone <url>

git branch <name of branch>

use git branch <enter> to check which the current branch is

git checkout <name of branch> to switch branch

use git add and git commit to commit changes in the branch

for merging, must go to the main branch first then
git merge <name of branch>
