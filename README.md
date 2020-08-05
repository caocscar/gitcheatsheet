# Git Cheat Sheet

command|description
---|---
`git checkout <branch>` OR `git switch <branch>` | checkout branch
`git checkout -b <new-branch>` OR `git switch -c <new-branch>` | create & checkout new branch
`git checkout --track <remote>/<branch>` OR `git switch -c <new-branch> --track <remote>/<branch>`| checkout remote branch
`git branch` | list available and current branches
`git branch <new-branch>` | create new branch
`git branch -d <branch>` | delete branch
`git branch -u origin/<branch>` | set upstream branch
`git branch -m <newname>` | rename git branch
`git branch -vv` | see which remote branch the current branch is tracking
`git status` | see current status of files
`git add <filename>` | add filename to staging area
`git commit -m "message"` | commit files and add message
`git commit -am "message"` | add & commit files and add message
`git commit --amend -m "new-message"` | amend last commit message (if not pushed to remote already)
`git reset <filename>` | unstage filename from staging area
`git reset --soft HEAD~1` | soft reset (keep all changes) back 1 commit
`git reset --hard HEAD~1` | hard reset (discard all changes) back 1 commit
`git merge <branch>` | merge branch into current branch
`git rebase <branch>` | rebase current branch onto branch
`git push -f` | force push
`git diff` | see existing changes
`git stash` | stash working directory
`git stash list` | list stashes
`git stash pop` | pop stash
`git stash drop stash@{index}` | delete stash
`git stash clear` | delete all stashes
`git tag` | list existing tags
`git tag <tag-name>` | create lightweight tag
`git tag -a <tag-name> -m "<tag-message>"` | create annotated tag with message at current commit
`git tag -a <tag-name> -m "<tag-message>" commit_id` | create annotated tag with message at specific commit id
`git tag -d <tag-name>` | delete tag
`git show <tag-name>` | show tag
`git push origin <tag-name>` | push tag to remote
`git push origin --tags` | push all tags to remote
`git push origin --delete <tag-name>` | delete tag on remote
`git log --pretty=oneline` | view commit history
`git version` | list git version

## Reference
The [Pro Git book](https://git-scm.com/book/en/v2) (with translations into other languages too)  
