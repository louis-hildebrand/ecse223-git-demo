# Git Demo

This repository demonstrates how to use Git and GitHub.

To install Git or consult the documentation, see https://git-scm.com/.

## Summary

Here are some of the commands I discussed during the tutorial.
You can also find the exact commands I ran in [history.txt](./history.txt).

- Creating a new repository:
  - `git init` (new local repo)
  - `git clone <url>` (make local copy of existing remote repo)
- Viewing the repository:
  - `git status` (current branch, changes in the workspace and staging area, etc.)
  - `git log` (history of the repo)
- Creating a commit:
  - `git add <files>` (add files to the staging area)
  - `git commit -m "<message>"` (create a new commit with the changes in the staging area)
- Undoing changes:
  - `git restore --staged <files>` (remove files from the staging area)
  - `git restore <files>` (discard changes in the workspace)
  - `git revert <commit>` (create a new commit that undoes a given commit)
  - `git reset <commit>` (update `HEAD` - this can be used to essentially delete a commit)
  - `git clean` (delete untracked or ignored files)
- Branches:
  - `git branch <new-branch-name>` (create a new branch)
  - `git switch <branch-name>` (switch to an existing branch)
  - `git switch -c <new-branch-name>` (create a new branch and switch to it)
  - `git merge <branch-name>` (merge another branch into the current branch)
- Remote repository:
  - `git remote add origin <url>` (create a remote called `origin` with the given URL)
  - `git fetch` (fetch changes from the local repo, but don't merge with your local changes)
  - `git pull` (fetch and then merge or rebase)
  - `git push` (send your local changes to the remote repo if there's already an upstream branch)
  - `git push -u origin HEAD` (push the current branch and set up the upstream branch - use this for pushing a branch the first time)
