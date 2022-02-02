<!-- git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/dreibona/cheatsheets-vault.git
git push -u origin main

push an existing repository from the command line
git remote add origin https://github.com/dreibona/cheatsheets-vault.git
git branch -M main
git push -u origin main -->

# Git cheatsheet

## Table of contents

- [Git cheatsheet](#git-cheatsheet)
  - [Table of contents](#table-of-contents)
    - [Setup](#setup)
    - [Init](#init)
    - [Stage-Snapshot](#stage-snapshot)
    - [Branch-Merge](#branch-merge)
    - [Share-Update Repos](#share-update-repos)
    - [Inspect-Compare](#inspect-compare)
    - [Tracking path changes](#tracking-path-changes)
    - [Rewrite History](#rewrite-history)
    - [Temporary Commits](#temporary-commits)
    - [Formulas](#formulas)

### Setup

Configuring user information used across all local repositories.

| Command                                                | Description                                                            |
| :----------------------------------------------------- | :--------------------------------------------------------------------- |
| `git config --global user.name “[firstname lastname]”` | Set a name that is identifiable for credit when review version history |
| `git config --global user.email “[valid-email]”`       | Set automatic command line coloring for Git for easy reviewing         |
| `git config --global color.ui auto`                    | Set automatic command line coloring for Git for easy reviewing         |
| `git config --global core.excludesfile [file]`         | System wide ignore pattern for all local repositories                  |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Init

Configuring user information, initializing and cloning repositories.

| Command           | Description                                          |
| :---------------- | :--------------------------------------------------- |
| `git init`        | Initialize an existing directory as a Git repository |
| `git clone [url]` | Create a local copy of a remote repository           |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Stage-Snapshot

Working with snapshots and the Git staging area.

| Command                                 | Description                                                               |
| :-------------------------------------- | :------------------------------------------------------------------------ |
| `git status`                            | Show modified files in working directory, staged for your next commit     |
| `git add [file]`                        | Add a file as it looks now to your next commit (stage)                    |
| `git add -A` / `git add .`              | Add all new and changed files as it looks now to your next commit (stage) |
| `git reset [file]`                      | Unstage a file while retaining the changes in working directory           |
| `git diff`                              | Diff of what is changed but not staged                                    |
| `git diff --staged`                     | Diff of what is staged but not yet committed                              |
| `git commit -m "[descriptive message]"` | Commit your staged content as a new commit snapshot                       |
| `git rm -r [file]`                      | Remove a file (or folder)                                                 |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Branch-Merge

Isolating work in branches, changing context, and integrating changes.

| Command                                              | Description                                      |
| :--------------------------------------------------- | :----------------------------------------------- |
| `git branch`                                         | List branches, the \* denotes the current branch |
| `git branch -a`                                      | List all branches, local and remote              |
| `git branch [branch-name]`                           | Create a new branch at the current commit        |
| `git branch -m [old branch-name] [new branch-name]`  | Rename a local branch                            |
| `git branch -d [branch-name]`                        | Delete a branch                                  |
| `git push origin --delete [branch-name]`             | Delete a remote branch                           |
| `git checkout -b [branch-name] origin/[branch-name]` | Clone a remote branch and switch to it           |
| `git checkout -b [branch-name]`                      | Create a new branch and switch to it             |
| `git checkout [branch-name]`                         | Switch to a branch                               |
| `git checkout -`                                     | Switch to the branch last checked out            |
| `git checkout -- [file]`                             | Discard changes to a file                        |
| `git merge [branch-name]`                            | Merge a branch into the active branch            |
| `git merge [source branch] [target branch]`          | Merge a branch into a target branch              |
| `git log`                                            | Show all commits in the current branch’s history |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Share-Update Repos

Retrieving updates from another repository and updating local repos.

| Command                            | Description                                                   |
| :--------------------------------- | :------------------------------------------------------------ |
| `git remote add origin [url]`      | Add a remote repository                                       |
| `git remote set-url origin [url]`  | Set a repository's origin branch to SSH                       |
| `git remote fetch`                 | Checks to see if there are any changes remote branch          |
| `git merge [branch]`               | Merge a remote branch into your current branch                |
| `git push -u origin [branch-name]` | Transmit a local branch to remote branch (save origin)        |
| `git push`                         | Transmit a local branch to remote branch (saved origin)       |
| `git push origin [branch-name]`    | Transmit a local branch to remote branch                      |
| `git pull origin [branch-name]`    | Fetch and merge any commits from remote branch (save origin)  |
| `git pull`                         | Fetch and merge any commits from remote branch (saved origin) |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Inspect-Compare

Examining logs, diffs and object information

| Command                      | Description                                                        |
| :--------------------------- | :----------------------------------------------------------------- |
| `git log`                    | Show the commit history for the currently active branch            |
| `git log --summary`          | Show the commit history for the currently active branch (detailed) |
| `git log --oneline`          | Show the commit history for the currently active branch (briefly)  |
| `git log --follow [file]`    | Show the commits that changed file, even across renames            |
| `git log branchB..branchA`   | Show the commits on branchA that are not on branchB                |
| `git diff branchB...branchA` | Show the diff of what is in branchA that is not in branchB         |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Tracking path changes

Versioning file removes and path changes.

| Command                             | Description                                                   |
| :---------------------------------- | :------------------------------------------------------------ |
| `git rm [file]`                     | Delete the file from project and stage the removal for commit |
| `git mv [existing-path] [new-path]` | Change an existing file path and stage the move               |
| `git log --stat -M`                 | show all commit logs with indication of any paths that moved  |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Rewrite History

Rewriting branches, updating commits and clearing history.

| Command                     | Description                                                    |
| :-------------------------- | :------------------------------------------------------------- |
| `git rebase [branch]`       | Apply any commits of current branch ahead of specified one     |
| `git reset --hard [commit]` | clear staging area, rewrite working tree from specified commit |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Temporary Commits

Temporarily store modified, tracked files in order to change branches.

| Command          | Description                                 |
| :--------------- | :------------------------------------------ |
| `git stash`      | Save modified and staged changes            |
| `git stash list` | List stack-order of stashed file changes    |
| `git stash pop`  | Write working from top of stash stack       |
| `git stash drop` | Discard the changes from top of stash stack |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Formulas

Workflow recipies.

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>
