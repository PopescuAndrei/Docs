### Removing file already pushed to repository and later ignored in git ignore.
```
git rm -r one-of-the-directories
git commit -m "Remove duplicated directory"
git push origin <your-git-branch> (typically 'master', but not always)
```
---

### To do after I rename a repository.
git@github.com:someuser/someproject.git   ->    git@github.com:someuser/newprojectname.git
```
$ git remote set-url origin git@github.com:someuser/newprojectname.git
```
---

### Git Config Email and Password
```
$ git config --global user.email "your_email@example.com"
$ git config --global user.email //for confirming
```
---

### Init a repo for the first time
```
$ git init
$ git add -A
$ git commit -m "First Commit"
$ git remote add origin https://www.github.com/username/projectName.git #sets the repo
$ git remote -v #verifies the repo
$ git push origin master
```
---
