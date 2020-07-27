# Git Cheat Sheet
command|description
---|---
`git branch` | list available and current branches
`git checkout *branch*` | checkout branch
`git checkout -b *branch*` | create and checkout new branch
`git branch -d *branch*` | delete branch
`git branch -vv` | see which remote, branch is tracking
`git add .` | add all files for staging
`git status` | see current status of files
`git commit -m "message"` | commit files and add message
`git commit --amend -m "new message"` | amend last commit message (if not pushed to remote already)
`git reset --soft HEAD~1` | soft reset back 1 commit
