To submit changes to any file
- go to that directory from git bash
- git add "filename.type"
- git commit -m "anotherCommit"
- git push origin master 
// eikhane origin agei add thakte hobe, jodi na thake then add it with this command: git remote add origin https://github.com/admtuku/HelloGit.git

** To go back to any previous commit
- git checkout "commit hash" // for example: git checkout 0d1d7fc32
//Your file will be changed to that commit i.e. your repo HEAD is at 0d1d7fc32
// Details link: http://stackoverflow.com/questions/4114095/revert-to-a-previous-git-commit

** To Know your current HEAD position
- git rev-parse HEAD
// link: http://stackoverflow.com/questions/949314/how-to-retrieve-the-hash-for-the-current-commit-in-git

** To View log of your changes
- git log

** delete a push :D
- git push -f origin HEAD^:master
example: git push -f origin a8330c2:master

** If you are messed and want to get sync with origin up to date
- git fetch origin && git reset --hard origin/master && git clean -f -d
http://ocpsoft.org/tutorials/git/reset-and-sync-local-respository-with-remote-branch/

**when pushing causes prob
- git push origin HEAD:master