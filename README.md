# 2021-11-03 git_collab

- `git clone <URL>`: "downloads" the git repostitory <URL> to current directory
    - `git init`: creates git repo in current folder
- `git branch <NAME>`: creates a new branch <NAME> where HEAD is
    - `git branch -a`: lists all your branches, including the remote
- `git switch <BRANCH>`: move to the <BRANCH>
    - `git checkout <BRANCH>`: "older" way to switch

# branches

- `git log --oneline --graph --all`: shows you the git log with all the branches and history
- `git switch -c <BRANCH>`: create and switch to <BRANCH> in a single step
    - `git checkout -b <BRANCH>`: the "older" way
- pull request: (aka merge request), doing a merge on the remote (e.g., GitHub) interface
    - This is where you do code review
    - PRs will auto update if you push new commits
