http://www.liaoxuefeng.com/
mac: xcode
windows:msysgit is Windows version Git, dowload from https://git-for-windows.github.io

$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"

pwd
git init (run in the current folder)
git add readme.txt (file exists)
git commit -m "comments"

git status
git diff
git log --pretty=oneline
git reflog
git reset --hard head^
git reset --hard 8797896
git reset --hard head^^
git reset --hard head~10
use "git reset HEAD <file>..." to unstage
git diff HEAD -- readme.txt

git checkout -- readme.txt "cancel the modifications to the repo or the stage - UNMODIFY" replace workspace with repo
git reset HEAD readme.txt "unstage"
git rm user.txt

$ ssh-keygen -t rsa -C "youremail@example.com"

echo "# tmsmonitor" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/dianbau/tmsmonitor.git
git push -u origin master

git@github.com:dianbau/tmsmonitor.git using SSH
$ git clone git@github.com:michaelliao/gitskills.git

Dev
Test merge
=====
Master
git remote add origin3 git@github.com:dianbau/tmsmonitor.git
git push -u origin3 master

git remote
git remote remove origin

git checkout -b dev

git branch dev
git checkout dev

git branch

$ git checkout master
Switched to branch 'master'
$ git merge dev         
merge DEV to current branch
$ git branch -d dev
Deleted branch dev (was fec145a).


git branch :list branches
git branch <name> :create branch
git checkout <name> :switch branch
git checkout -b <name> :create and switch branch
git merge <name>  :merge to the current branch
git branch -d <name> :delete branch


$ git log --graph --pretty=oneline --abbrev-commit

$ git merge --no-ff -m "merge with no-ff" dev
Merge made by the 'recursive' strategy.
 readme.txt |    1 +
 
git stash
git stash list
stash@{0}: WIP on dev: 6224937 add merge

$ git stash apply stash@{0}         git stash drop
$ git stash pop

$ git branch -D feature-vulcan     :force to delete
Deleted branch feature-vulcan (was 756d4af).


$ git checkout -b dev origin/dev     others checkout the branch code!
git pull       execute before push 

$ git clone git@github.com:michaelliao/learngit.git
$ git branch --set-upstream dev origin/dev
Branch dev set up to track remote branch dev from origin.

$ git tag v0.9 6224937
$ git tag -a v0.1 -m "version 0.1 released" 3628164
$ git show v0.9

$ git tag -d v0.1
Deleted tag 'v0.1' (was e078af9)

$ git push origin v1.0
Total 0 (delta 0), reused 0 (delta 0)
To git@github.com:michaelliao/learngit.git
 * [new tag]         v1.0 -> v1.0
 
$ git push origin --tags    push all!

$ git push origin :refs/tags/v0.9   remove delete
To git@github.com:michaelliao/learngit.git
 - [deleted]         v0.9
 
 .gitignore
 git check-ignore -v App.class