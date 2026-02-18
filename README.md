
## SSH

```bash
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

## Initial Setup

```bash
git init  # Initializes a new local Git repository.
```

```bash
git remote add origin <url>  # Connects your local repository to a remote repository.
```

## Working with Changes

```bash
git status  # Checks the current state of your repository.
```

```bash
git add .  # Adds all current changes to the index for commit.
```

```bash
git reset <item-name>  # Removes item from the current staged changes for commit.
```

```bash
git diff  # Shows the differences between unstaged files and the index.
```

```bash
git commit -m "commit name"  # Records the changes in the repository with a commit message.
```

## Branching and Merging

```bash
git branch -M main  # Renames the current branch to "main".
```

```bash
git branch  # Lists all local branches.
```

```bash
git branch <branch-name>  # Creates a new branch.
```

```bash
git switch <branch-name>  # Switches to the specified branch.
```

```bash
git switch -c <branch-name>  # Creates and switches to the specified branch.
```

```bash
git merge <branch-name>  # Merges the specified branch into the current branch.
```

```bash
git merge --squash <branch-name>  # Merges the specified branch into the current branch without commit history.
```

```bash
git cherry-pick <commit-hash>  # Takes the last commit from the branch you want to the current branch.
```

```bash
git branch -D <branch-name>  # Deletes the specified branch.
```

```bash
git push origin :<branch-name>  # Removes the specified branch from the remote repository.
```

## Collaboration

```bash
git push -u origin main  # Sends local commits to the remote repository (main) for the first time.
```

```bash
git pull --rebase # Pulls and merges changes from the remote repository to the local repository.
```

## Logs and History

```bash
git log  # Shows the commit history.
```

```bash
git log --oneline  # Shows the commit history with one line per commit.
```

```bash
git log --graph  # Shows the commit history in a graphical format.
```

```bash
git show  # Shows information about a specific commit.
```

```bash
git log <branch-name>  # Shows the commit history of a specific branch.
```

## Reverting Changes

```bash
git revert <commit-code>  # Reverts a specific commit by creating a new commit.
```

```bash
git reset --hard HEAD  # Reverts the working directory and index to the state of the last commit.
```

## Stash

```bash
git stash  # Saves temporary changes that are not ready for commit.
```

```bash
git stash pop  # Applies and removes the last stash entry.
```

```bash
git stash drop  # Removes the last stash entry.
```

```bash
git stash clear  # Clears all stash entries.
```

```bash
git stash push -m "stash name"  # Saves temporary changes with an associated message.
```

## Worktree

```bash
git worktree add ../<folder-name> <branch-name> # Creates a new folder and automatically checks out the branch

```

```bash
git worktree remove ../feature-x # Removes the worktree without deleting the branch
```

```bash
git worktree list # Lists all active worktrees
```

## Tags

```bash
git tag <tag-name>  # Creates a lightweight tag at the current version.
```

```bash
git tag <tag-name> <commit-code>  # Creates a tag associated with a specific commit.
```

```bash
git tag  # Lists all tags in the repository.
```

```bash
git push origin <tag-name>  # Sends a specific tag to the remote repository.
```

```bash
git push origin --tags  # Sends all local tags to the remote repository.
```

```bash
git tag -d <tag-name>  # Deletes a tag locally.
```

```bash
git push --delete origin <tag-name>  # Removes a tag from the remote repository.
```

```bash
git tag -a <tag-name> -m "tag message"  # Creates an annotated tag with an associated message.
```

```bash
git tag -v <tag-name>  # Verifies the signature of an annotated tag.
```
