# 🐙 GitHub — Complete Guide

> *GitHub is where over 100 million developers collaborate. It's Git + social network + CI/CD platform + project management all in one.*

---

## 📋 Table of Contents

- [What is GitHub?](#what-is-github)
- [Account Setup](#account-setup)
- [Repository Basics](#repository-basics)
- [Issues](#issues)
- [Pull Requests](#pull-requests)
- [GitHub Actions](#github-actions)
- [GitHub Discussions](#github-discussions)
- [GitHub Pages](#github-pages)
- [Useful Features](#useful-features)
- [Keyboard Shortcuts](#keyboard-shortcuts)

---

## 🤔 What is GitHub?

GitHub is a cloud-based platform that hosts Git repositories. It adds:

- **Web interface** to view and edit code
- **Pull Requests** for code review and collaboration
- **Issues** for bug tracking and feature requests
- **Actions** for CI/CD automation
- **Discussions** for community conversations
- **Pages** for free website hosting

---

## 👤 Account Setup

### Profile Optimization

A strong GitHub profile attracts collaborators and employers:

```
✅ Professional photo or avatar
✅ Clear bio (who you are + what you build)
✅ Location and website
✅ Pinned repositories (your best work)
✅ README profile (special repo: username/username)
```

### Creating a Profile README

Create a repo named exactly `YOUR_USERNAME` (e.g., `octocat/octocat`). Add a `README.md` — it appears on your profile!

```markdown
# Hi, I'm [Your Name] 👋

🔭 Currently working on: [Project]
🌱 Learning: [Technology]
💬 Ask me about: [Topics]
📫 Reach me: [Email/Social]
```

### SSH Keys (Recommended)

```bash
# Generate SSH key
ssh-keygen -t ed25519 -C "your_email@example.com"

# Copy public key
cat ~/.ssh/id_ed25519.pub

# Add to GitHub: Settings → SSH Keys → New SSH Key
# Test connection
ssh -T git@github.com
```

---

## 📁 Repository Basics

### Creating a Repository

1. Click **+** → **New repository**
2. Choose a clear, lowercase, hyphenated name
3. Add a description
4. Initialize with README, .gitignore, License
5. Click **Create repository**

### Repository Files to Include

| File | Purpose |
|------|---------|
| `README.md` | Project overview and documentation |
| `CONTRIBUTING.md` | How to contribute |
| `LICENSE` | Legal permissions |
| `CODE_OF_CONDUCT.md` | Community standards |
| `.gitignore` | Files Git should ignore |
| `CHANGELOG.md` | Version history |

### Forking

Forking creates your own copy of someone else's repository:

1. Click the **Fork** button (top right)
2. Select your account
3. Clone YOUR fork (not the original)

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/original-repo.git

# Add original as upstream
git remote add upstream https://github.com/original-owner/original-repo.git
```

---

## 🐛 Issues

Issues are how you report bugs, request features, and track work.

### Writing a Good Issue

**Bug reports** should include:
- Clear title describing the problem
- Steps to reproduce
- Expected vs actual behavior
- Environment (OS, browser, version)
- Screenshots if visual

**Feature requests** should include:
- What you want to achieve (not just how)
- Why this would be valuable
- Any potential implementation ideas

### Issue Labels

Common labels you'll see:

| Label | Meaning |
|-------|---------|
| `bug` | Something isn't working |
| `enhancement` | New feature or improvement |
| `good first issue` | Great for newcomers |
| `help wanted` | Extra attention needed |
| `documentation` | Docs improvements |
| `wontfix` | Will not be addressed |
| `duplicate` | Already exists |

### Referencing Issues

In commit messages or PRs, use:
- `Fixes #123` — closes the issue when PR merges
- `Closes #123` — same as above
- `Resolves #123` — same as above
- `See #123` — references without closing

---

## 🔀 Pull Requests

See the full [Pull Requests Guide](PullRequests.md) for detail.

### Quick PR Workflow

```
Fork → Clone → Branch → Change → Commit → Push → PR → Review → Merge
```

### PR Best Practices

- **One thing per PR** — focus helps reviewers
- **Clear description** — explain what AND why
- **Small diffs** — easier to review
- **Tests** — include them if the project requires
- **Link issues** — use `Closes #123`

---

## ⚙️ GitHub Actions

GitHub Actions automates workflows triggered by repository events.

### Example: Run Tests on Push

```yaml
# .github/workflows/test.yml
name: Run Tests

on:
  push:
    branches: [main]
  pull_request:
    branches: [main]

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Run tests
        run: |
          npm install
          npm test
```

### Common Triggers

```yaml
on:
  push:              # On push to branches
  pull_request:      # On PR events
  schedule:          # Cron schedule
    - cron: '0 9 * * 1'  # Every Monday at 9am
  workflow_dispatch: # Manual trigger
  issues:            # On issue events
```

### Useful Actions

| Action | Use |
|--------|-----|
| `actions/checkout` | Check out code |
| `actions/setup-node` | Set up Node.js |
| `actions/cache` | Cache dependencies |
| `peter-evans/create-or-update-comment` | Comment on PRs |
| `actions/first-interaction` | Welcome new contributors |

---

## 💬 GitHub Discussions

Discussions are community forums within repositories.

### Categories

- **Q&A** — Questions and answers
- **Ideas** — Feature brainstorming
- **Show and Tell** — Share what you built
- **General** — Anything else

### When to Use Discussions vs Issues

| Use Issues for | Use Discussions for |
|----------------|---------------------|
| Specific bugs | General questions |
| Feature requests (decided) | Ideas and brainstorming |
| Tasks with clear completion | Community conversations |

---

## 🌐 GitHub Pages

Host a free website directly from your repository.

### Quick Setup

1. Go to **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: `main` / `docs` folder
4. Your site will be at: `username.github.io/repo-name`

### Jekyll Support

GitHub Pages natively supports Jekyll for static sites. Create a `_config.yml`:

```yaml
title: My Project
description: A great project
theme: minima
```

---

## 🛠️ Useful Features

### Code Review

- **Inline comments**: Click line numbers in Files Changed tab
- **Suggestions**: Use ```suggestion blocks to propose exact changes
- **Review types**: Comment / Approve / Request Changes

### GitHub CLI

```bash
# Install
brew install gh  # macOS

# Authenticate
gh auth login

# Create PR from terminal
gh pr create --title "My PR" --body "Description"

# View PRs
gh pr list

# Check out a PR
gh pr checkout 123
```

### GitHub Codespaces

Run a full VS Code environment in your browser — no local setup needed!

1. Open any repository
2. Press `.` (period) to open VS Code in the browser
3. Or click **Code** → **Codespaces** → **New codespace**

### Saved Replies

Save common responses to reuse in comments:
Settings → Saved replies → Add saved reply

### Notifications

Manage notifications effectively:
- **Watch**: Get all notifications
- **Participating**: Only when @mentioned or involved
- **Ignore**: No notifications

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `?` | Show keyboard shortcuts |
| `t` | File finder |
| `s` | Focus search |
| `g n` | Go to notifications |
| `g i` | Go to issues |
| `g p` | Go to pull requests |
| `g c` | Go to code |
| `.` | Open in VS Code (web) |
| `⌘ K` | Command palette |

---

## 📚 Further Reading

- [GitHub Docs](https://docs.github.com)
- [GitHub Skills](https://skills.github.com) — Interactive courses
- [GitHub Blog](https://github.blog)
- [GitHub CLI Manual](https://cli.github.com/manual/)

---

*Next: [Open Source Guide →](OpenSource.md)*
