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
