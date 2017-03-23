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