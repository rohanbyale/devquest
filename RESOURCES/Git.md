# 🔧 Git — Complete Guide

> *Git is a distributed version control system that tracks changes in your code. Mastering it is the single most valuable skill for any developer.*

---

## 📋 Table of Contents

- [What is Git?](#what-is-git)
- [Installation](#installation)
- [Core Concepts](#core-concepts)
- [Essential Commands](#essential-commands)
- [Branching](#branching)
- [Remote Repositories](#remote-repositories)
- [Undoing Mistakes](#undoing-mistakes)
- [Advanced Topics](#advanced-topics)
- [Best Practices](#best-practices)
- [Cheat Sheet](#cheat-sheet)

---

## 🤔 What is Git?

Git is a tool that tracks every change you make to your files. Think of it like a time machine for your code — you can go back to any point in history, create parallel universes (branches), and merge different timelines together.

### Why Git Matters

- **Safety**: Never lose work again
- **Collaboration**: Multiple people can work on the same project simultaneously
- **History**: See who changed what, when, and why
- **Experimentation**: Try ideas in branches without breaking anything

---

## ⚙️ Installation

### macOS

```bash
# Option 1: Homebrew (recommended)
brew install git

# Option 2: Xcode Command Line Tools
xcode-select --install
```

### Windows

Download and install from [git-scm.com](https://git-scm.com/download/win). Use **Git Bash** as your terminal.

### Linux (Ubuntu/Debian)

```bash
sudo apt update
sudo apt install git
```

### Verify Installation

```bash
git --version
# git version 2.43.0
```

### First-Time Setup

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global core.editor "code --wait"  # Use VS Code as editor
git config --global init.defaultBranch main     # Default branch name
```

---

## 🧠 Core Concepts

### The Three Areas

```
Working Directory  →  Staging Area  →  Repository
   (your files)       (git add)       (git commit)
```

- **Working Directory**: Where you edit files
- **Staging Area** (Index): Where you prepare commits
- **Repository**: Where commits are permanently stored

### File States

```
Untracked → Staged → Committed → Modified → Staged → Committed...
```

- **Untracked**: New file Git doesn't know about
- **Staged**: Ready to be committed
- **Committed**: Saved in Git history
- **Modified**: Changed since last commit

---

## 📝 Essential Commands

### Starting a Repository

```bash
# Create a new repository
git init

# Clone an existing repository
git clone https://github.com/username/repo.git

# Clone into a specific folder
git clone https://github.com/username/repo.git my-folder
```

### Checking Status

```bash
# See current state of your working directory
git status

# Short status
git status -s

# See what changed (unstaged)
git diff

# See staged changes
git diff --staged
```

### Staging & Committing

```bash
# Stage a specific file
git add filename.md

# Stage all changes
git add .

# Stage parts of a file interactively
git add -p filename.md

# Commit staged changes
git commit -m "feat: add new feature"

# Stage and commit tracked files in one step
git commit -am "fix: quick fix"
```

### Viewing History

```bash
# View commit history
git log

# Compact one-line history
git log --oneline

# History with graph
git log --oneline --graph --all

# History of a specific file
git log --follow filename.md

# Show a specific commit
git show abc1234
```

---

## 🌿 Branching

Branches let you work on features or fixes in isolation.

### Basic Branch Operations

```bash
# List all branches
git branch

# Create a new branch
git branch feature-name

# Switch to a branch
git checkout feature-name

# Create and switch in one command (modern)
git switch -c feature-name

# Create and switch (classic)
git checkout -b feature-name

# Delete a branch (after merge)
git branch -d feature-name

# Force delete (unmerged)
git branch -D feature-name

# Rename a branch
git branch -m old-name new-name
```

### Merging

```bash
# Switch to the destination branch
git checkout main

# Merge another branch into current
git merge feature-name

# Merge with a commit message
git merge feature-name --no-ff -m "Merge feature-name into main"
```

### Rebasing

```bash
# Rebase current branch onto main
git rebase main

# Interactive rebase (last 3 commits)
git rebase -i HEAD~3

# Continue rebase after resolving conflicts
git rebase --continue

# Abort a rebase
git rebase --abort
```

---

## 🌐 Remote Repositories

### Managing Remotes

```bash
# View remotes
git remote -v

# Add a remote
git remote add origin https://github.com/username/repo.git

# Add upstream (original repo when you've forked)
git remote add upstream https://github.com/original-owner/repo.git

# Remove a remote
git remote remove origin

# Change remote URL
git remote set-url origin https://github.com/new-url/repo.git
```

### Pushing & Pulling

```bash
# Push current branch to remote
git push origin branch-name

# Push and set upstream tracking
git push -u origin branch-name

# Pull (fetch + merge)
git pull origin main

# Fetch without merging
git fetch origin

# Fetch all remotes
git fetch --all

# Pull with rebase instead of merge
git pull --rebase origin main
```

### Syncing a Fork

```bash
# Fetch upstream changes
git fetch upstream

# Merge upstream/main into your local main
git checkout main
git merge upstream/main

# Push to keep your fork updated
git push origin main
```

---

## ↩️ Undoing Mistakes

### Before Committing

```bash
# Undo changes to a file (restore to last commit)
git checkout -- filename.md

# Unstage a file (keep changes)
git reset HEAD filename.md

# Discard ALL unstaged changes (⚠️ irreversible)
git checkout -- .
```

### After Committing

```bash
# Amend last commit (message or staged files)
git commit --amend

# Undo last commit, keep changes staged
git reset --soft HEAD~1

# Undo last commit, keep changes unstaged
git reset HEAD~1

# Undo last commit, discard changes (⚠️ irreversible)
git reset --hard HEAD~1

# Create a new commit that reverts a specific commit
git revert abc1234
```

### Emergency Recovery

```bash
# See history of HEAD movements (including deleted branches)
git reflog

# Recover a deleted commit
git checkout abc1234
```

---

## 🔬 Advanced Topics

### Stashing

```bash
# Save work-in-progress without committing
git stash

# Stash with a description
git stash push -m "WIP: half-done feature"

# List all stashes
git stash list

# Apply most recent stash (keep stash)
git stash apply

# Apply and remove stash
git stash pop

# Apply a specific stash
git stash apply stash@{2}

# Delete a stash
git stash drop stash@{0}
```

### Tags

```bash
# List tags
git tag

# Create a lightweight tag
git tag v1.0.0

# Create an annotated tag
git tag -a v1.0.0 -m "Release version 1.0.0"

# Push tags to remote
git push origin --tags
```

### Cherry-picking

```bash
# Apply a specific commit to the current branch
git cherry-pick abc1234
```

---

## ✅ Best Practices

### Commit Messages

Follow the Conventional Commits format:

```
type(scope): short description

[optional body explaining WHY]

[optional footer with references]
```

Types: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`

### Branch Naming

```
feature/user-authentication
fix/broken-login-link
docs/improve-readme
chore/update-dependencies
```

### The Golden Rules

1. **Commit often**: Small, frequent commits are easier to review and revert
2. **Never force push to shared branches**: It rewrites history for everyone
3. **Write meaningful commit messages**: Your future self will thank you
4. **Keep branches short-lived**: Merge or delete branches quickly
5. **Review before committing**: `git diff --staged` before every commit

---

## 📋 Cheat Sheet

```bash
# Setup
git config --global user.name "Name"
git config --global user.email "email"

# Start
git init
git clone <url>

# Stage & Commit
git add .
git commit -m "message"
git commit -am "message"

# Branch
git checkout -b branch-name
git merge branch-name
git branch -d branch-name

# Remote
git remote add origin <url>
git push origin branch-name
git pull origin main
git fetch upstream

# Undo
git reset HEAD~1
git revert <commit>
git stash / git stash pop

# History
git log --oneline --graph
git diff
git status
```

---

## 📚 Further Reading

- [Official Git Documentation](https://git-scm.com/doc)
- [Pro Git Book (free)](https://git-scm.com/book)
- [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)
- [Learn Git Branching (Interactive)](https://learngitbranching.js.org)

---

*Next: [GitHub Guide →](GitHub.md)*
