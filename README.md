# Git Cheat Sheet

command|description
---|---
`git checkout <branch>` OR `git switch <branch>` | checkout branch
`git checkout -b <new-branch>` OR `git switch -c <new-branch>` | create & checkout new branch
`git checkout --track <remote>/<branch>` OR `git switch -c <new-branch> --track <remote>/<branch>`| checkout remote branch
`git branch` | list available and current branches
`git branch <new-branch>` | create new branch
`git branch -d <branch>` | delete branch
`git push origin --delete <branch>` | delete remote branch
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
`git push <remote> <tag-name>` | push tag to remote
`git push <remote> --tags` | push all tags to remote
`git push <remote> --delete <tag-name>` | delete tag on remote
`git push -u <remote> <branch>` | set upstream branch and push to it
`git log --pretty=oneline` | view commit history
`git version` | list git version
`git init` | initialize git repo in current directory
`git remote` | list short names of each remote handle
`git remote -v` | list urls for each short names of each remote handle
`git remote add <short-name> <url>` | add remote repository
`git remote show <remote>` | show information about a remote
`git fetch <remote>` | pulls down all data from remote for inspection or merging
`git rm <filename>` | removes files from the working tree and from the index
`git cherry-pick <commitSha>` | cherry-pick specific commit to current working HEAD

shorthand|switch
:---:|---
-d|--delete
-f|--force
-m|--move
-c|--copy
-i|--ignore-case
-r|--remotes
-a|--all
-l|--list
-v,-vv|--verbose
-q|--quiet
-t|--track
-u \<upstream>|--set-upstream-to=\<upstream>
  

## Reference
The [Pro Git book](https://git-scm.com/book/en/v2) (with translations into other languages too)  
