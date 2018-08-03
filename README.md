# Git Cheat Sheet

command|description
---|---
git clone [repo-URL]|downloads a project and its entire version history
git status|lista ll new or modified files to be committed
git add [file]|snapshots the file in preparation for versioning
git commit -m "[commit message]"|records snapshots permanently in version history
git push [alias] [branch] |uploads all local branch commits to GitHub
git pull|downloads bookmark history and incorporates changes
git revert -m 1 <merge-commit>|revert to the first parent of the merge commit on the master branch
git mv [file-original] [file-renamed]|changes the filename and prepares it for commit
git rm [file]|deletes the file from the working directory and stages the deletion
git rm --cached [file]|removes the files from version control but preserves the file locally
git init [project-name]|creates a new local repository
git init|initialize existing directory

## Reference Links
[Adding an existing project to GitHub using the command line](https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line)


