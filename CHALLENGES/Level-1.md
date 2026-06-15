# ⚔️ Level 1 — First Fork

[![Difficulty](https://img.shields.io/badge/Difficulty-Beginner-brightgreen?style=for-the-badge)](.)
[![XP Reward](https://img.shields.io/badge/XP%20Reward-50%20XP-orange?style=for-the-badge)](.)
[![Time](https://img.shields.io/badge/Time-15%20mins-blue?style=for-the-badge)](.)

> *"Every great journey begins with a single step — and every great open source journey begins with a fork."*

---

## 🎯 Objective

Fork the DevQuest repository and add yourself to the `CONTRIBUTORS.md` file. This is your first step into the world of open source contribution!

---

## 📋 Requirements

To complete Level 1, you must:

- [ ] **Fork** this repository to your GitHub account
- [ ] **Clone** your fork to your local machine
- [ ] **Create** a new branch named `add/your-github-username`
- [ ] **Add** your entry to `CONTRIBUTORS.md`
- [ ] **Commit** your change with the message: `feat: add YOUR_USERNAME to contributors`
- [ ] **Push** your branch to GitHub

---

## 📖 Step-by-Step Instructions

### 1. Fork the Repository

Click the **Fork** button in the top-right corner of the DevQuest repository page. Select your account as the destination.

### 2. Clone Your Fork

Open your terminal and run:

```bash
git clone https://github.com/rohanbyale/devquest.git
cd devquest
```

Replace `YOUR_USERNAME` with your actual GitHub username.

### 3. Create a Branch

```bash
git checkout -b add/your-github-username
```

Example: `git checkout -b add/octocat`

### 4. Add Yourself to CONTRIBUTORS.md

Open `CONTRIBUTORS.md` in any text editor and add your row to the contributors table:

```markdown
| [your-username](https://github.com/your-username) | 🔰 Rookie | Level 1 | 50 XP | Month YYYY |
```

Keep the table sorted alphabetically by username.

### 5. Commit Your Change

```bash
git add CONTRIBUTORS.md
git commit -m "feat: add your-username to contributors"
```

### 6. Push Your Branch

```bash
git push origin add/your-github-username
```

---

## ✅ Verification

After pushing, go to GitHub. You should see a banner saying **"Compare & pull request"**. Click it — but don't open the PR yet! That's Level 2! 😄

For Level 1 verification, a maintainer simply checks that you've:
- Successfully forked the repo
- Created the correct branch
- Made the correct edit to `CONTRIBUTORS.md`

---

## 🎁 Rewards

Upon completing this level you earn:

- ⭐ **50 XP** toward your rank
- 🏅 **"First Fork" badge** (add it to your DevQuest contributor entry)
- 📋 Your name in the contributors list

---

## 💡 Tips

> **Tip 1**: If you get a "permission denied" error when pushing, make sure you cloned *your fork* and not the original repository. The URL should contain YOUR username.

> **Tip 2**: Not sure what branch you're on? Run `git branch` — the current branch has an asterisk `*` next to it.

> **Tip 3**: Made a typo in your commit message? Run `git commit --amend` before pushing to fix it.

> **Tip 4**: Want to see your changes before committing? Run `git diff` to see what's changed.

---

## 📚 Resources

If you're stuck, these guides will help:

- [🔧 Git Guide](../RESOURCES/Git.md) — Everything you need to know about Git
- [🐙 GitHub Guide](../RESOURCES/GitHub.md) — Navigating GitHub like a pro
- [🚀 Getting Started](../docs/getting-started.md) — DevQuest beginner guide

---

## ➡️ What's Next?

Ready for the next step?

**[Level 2 → First Pull Request](Level-2.md)**

---

<div align="center">

*You've got this! The hardest part is starting.* 💪

[🏠 Back to Main Challenges](../README.md#-challenge-system) | [➡️ Level 2](Level-2.md)

</div>
