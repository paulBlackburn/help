# All the commands I use in my daily workflow to be productive as possible as a Software Engineer
## grep
grep --exclude-dir=env "" -r --include=\*py .
## Chrome Developer Tools
toggle Ctrl Shift j
## git
#### Stash
git stash\
git stash list\
git stash pop\
git add [file you don't want to stash]\
git stash --keep-index
#### Undo commit
git reset --soft HEAD~ (undo the last commit from local repo, but the file changes will stay in your working tree)\
git push -f (if the commit was pushed to remote repo)\
git revert [commit-hash]
#### Branches
I believe feature branches are a great tool to limit scope creep\
When a feature branch is merged the feature branch can be deleted\
git checkout -b [branch_name] --track origin/[branch_name]\
git branch -d [branch_name]\
git remote update origin --prune\
To reuse the same branch\
git pull origin [branch_name]
#### PRs
git merge --no-commit [branch_name]\
git merge --abort
#### Rebase
git checkout feature-branch
git pull origin main
git rebase main
## venv
env\scripts\activate.bat\
deactivate
## VS Code
Ctrl / (multiline comment)

