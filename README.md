# Git Commands Overview

## Git Clone
The `git clone` command is used to download the source code from a remote repository (like GitHub, Bitbucket, or GitLab).

### Using Git Clone Command:
```bash
git clone <https://url-of-the-repository>
```
When you clone a repo, the code is automatically downloaded to your local machine.

## Git Status
This command shows which files are modified, untracked, or staged.

```bash
git status
```

## Git Add
Every time you create, delete, or modify a file, you must stage it using git add.

```bash
git add <file-name>
```
To add all modified files:

```bash
git add -A
```
> Note: `git add` only stages changes. It does not save them permanently or push them anywhere.

## Git Commit
Think of the Git Commit command like a checkpoint in your development process.

Commit all staged changes:

```bash
git commit
```
Commit all tracked files directly:

```bash
git commit -a
```
Commit with a message:

```bash
git commit -am "<commit-message>"
```
> Note: Commits are stored only in your local repository until you push them.

## Git Push
Push your committed changes to the remote repository:

```bash
git push <remote> <branch-name>
```
> Only committed changes will be pushed.

## Git Pull
Download and merge the latest changes from the remote repo into your local branch:

```bash
git pull <remote> <branch-name>
```
## Git Branch
Branches allow you to work on different features independently.

### Create a new branch:
```bash
git branch <branch-name>
```
### Switch to an existing branch:
```bash
git checkout <branch-name>
```
### Create and switch to a new branch:
```bash
git switch -c <branch-name>
```
### List all branches:
```bash
git branch
```
## Git Merge
Merge another branch into your current branch:

```bash
git merge <branch-name>
```
## Git Log
View commit history:

```bash
git log
```
## Git Remote
View connected remote repositories:

```bash
git remote -v
```
## Git Stash
Temporarily save uncommitted changes:

```bash
git stash
```
Restore them later:

```bash
git stash pop
```
## Git Reset (Use Carefully!)
Undo commits or remove changes.

Undo last commit but keep changes:

```bash
git reset --soft HEAD~1
```
Undo last commit AND delete changes permanently:

```bash
git reset --hard HEAD~1
```
⚠️ Be careful: `--hard` removes changes permanently.
