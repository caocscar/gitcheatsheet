# Git Cheat Sheet

command|description
---|---
`git checkout <branch>` | checkout branch
`git checkout -b <branch>` | create and checkout new branch
`git branch` | list available and current branches
`git branch -d <branch>` | delete branch
`git branch -u origin/<branch>` | set upstream branch
`git branch -m <newname>` | rename git branch
`git branch -vv` | see which remote, branch is tracking
`git status` | see current status of files
`git add <filename>` | add filename to staging area
`git reset <filename>` | unstage filename from staging area
`git commit -m "message"` | commit files and add message
`git commit -am "message"` | add and commit files (in one command) and add message
`git commit --amend -m "new message"` | amend last commit message (if not pushed to remote already)
`git reset --soft HEAD~1` | soft reset (keep all changes) back 1 commit
`git reset --hard HEAD~1` | hard reset (discard all changes) back 1 commit
`git merge <branch>` | merge branch into current branch
`git rebase <branch>` | rebase current branch onto branch
`git push -f` | force push
`git diff` | see existing changes
`git checkout --track origin/<branch>` | checkout remote branch

## Reference
The [Pro Git book](https://git-scm.com/book/en/v2) (with translations into other languages too)  
