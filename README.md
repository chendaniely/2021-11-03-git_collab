# 2021-11-03 Git Collaboration

- `git clone <URL>`: "downloads" the git repostitory <URL> to current directory
    - `git init`: creates git repo in current folder
- `git branch <NAME>`: creates a new branch <NAME> where HEAD is
    - `git branch -a`: lists all your branches, including the remote
- `git switch <BRANCH>`: move to the <BRANCH>
    - `git checkout <BRANCH>`: "older" way to switch

# Branches

- `git log --oneline --graph --all`: shows you the git log with all the branches and history
- `git switch -c <BRANCH>`: create and switch to <BRANCH> in a single step
    - `git checkout -b <BRANCH>`: the "older" way
- pull request: (aka merge request), doing a merge on the remote (e.g., GitHub) interface
    - This is where you do code review
    - PRs will auto update if you push new commits

- `git stash`: makes a temp commit with current changes
    - `git stash pop`: takes the last stash and re-applies it current state

# Rebase

1. `git switch <BRANCH>`
2. `git rebase main`

this will rebase <BRANCH> against main.

# Cleanup

- `git fetch --prune`: clean up the git history and remove remote branches that were deleted
- `git branch -d <BRANCH>`: delete the branch, will fail if branch is not merged
    - `git branch -D <BRANCH>`: force delete branch

# git flow

special branch names and a convention on how to work in branches

# cherry pick

- `git cherry-pick <HASH>`: moves hash to current location (like a copy)
    - `git cherry-pick <HASH>^..<HASH>`: picks all the commits from both sides inclusive
    - by default it is exclusive left, inclusive right
    - the ^ makes it inclusive on both sides

