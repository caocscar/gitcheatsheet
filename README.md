# Git Cheat Sheet

command|description
---|---
`git checkout <branch>` OR `git switch <branch>` | checkout branch
`git checkout -b <new-branch>` OR `git switch -c <new-branch>` | create & checkout new branch
`git checkout --track <remote>/<branch>` OR `git switch -c <new-branch> --track <remote>/<branch>`| checkout remote branch
`git checkout -- <file>` | discard changes in working directory
`git branch` | list available and current branches
`git branch <new-branch>` | create new branch
`git branch -d <branch>` | delete branch
`git push origin --delete <branch>` | delete remote branch
`git branch -u origin/<branch>` | set upstream branch
`git branch -m <newname>` | rename current git branch
`git branch -m <branch> <newname>` | rename non-current git branch
`git branch -vv` | see which remote branch the current branch is tracking
`git status` | see current status of files
`git add <filename>` | add filename to staging area
`git add --patch <filename>` | add hunks of code to staging area
`git commit -m "message"` | commit files and add message
`git commit -am "message"` | add & commit files and add message
`git commit --amend -m "new-message"` | amend last commit message (if not pushed to remote already)
`git reset <filename>` | unstage filename from staging area
`git reset --soft HEAD~1` | soft reset (keep all changes) back 1 commit
`git reset --hard HEAD~1` | hard reset (discard all changes) back 1 commit
`git reset --hard` | hard reset (discard all local changes)
`git reset HEAD <filename>` | unstage changes
`git revert <commitSha>` | revert specific commit
`git clean -fd` | remove untracked files from working tree (force options with recursive directories)
`git merge <branch>` | merge branch into current branch
`git rebase <branch>` | rebase current branch onto branch
`git rebase --abort` | check out the original branch and stop rebasing 
`git push -f` | force push
`git diff` | see existing changes
`git diff <branch1> <branch2> -- <file>` | see file diff between two branches
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
`git show <commitSha>` | show commit with changes
`git show <tag-name>` | show tag
`git push <remote> <tag-name>` | push tag to remote
`git push <remote> --tags` | push all tags to remote
`git push <remote> --delete <tag-name>` | delete tag on remote
`git push -u <remote> <branch>` | set upstream branch and push to it
`git branch --set-upstream-to origin/<branch>` | set current branch to track upstream origin branch
`git log --pretty=oneline` | view commit history
`git log -p` | view commit history with changes shown
`git version` | list git version
`git init` | initialize git repo in current directory
`git remote` | list short names of each remote handle
`git remote -v` | list urls for each short names of each remote handle
`git remote add <short-name> <url>` | add remote repository
`git remote show <remote>` | show information about a remote
`git remote set-url origin git@ssh-code.maymobility.com:data-products/<repo.git>` | update the remote url in your local repository after transfer for ssh
`git remote set-url origin <url>/<repo.git>` |  update the remote url in your local repository after transfer for https
`git fetch <remote>` | pulls down all data from remote for inspection or merging
`git rm <filename>` | removes files from the working tree and from the index
`git cherry-pick <commitSha>` | cherry-pick specific commit to current working HEAD
`git reflog` | displays log of all the changes made to the repo including changes made to branches, commits, and merges 

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
  
## Renaming default branch from Master to Main
1. `git branch -m master main` on local machine.  
2. Gitlab -> settings -> repository -> Default branch -> main (you might have to push main onto origin).  
3. [Optional] Make changes to protected branches. 
4. `git push origin --delete master` to remove remote master branch. Remove master branch from protected status as required.

## Reference
The [Pro Git book](https://git-scm.com/book/en/v2) (with translations into other languages too)  
