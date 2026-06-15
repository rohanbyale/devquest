# 🔥 Level 3 — First Merged PR

[![Difficulty](https://img.shields.io/badge/Difficulty-Intermediate-yellow?style=for-the-badge)](.)
[![XP Reward](https://img.shields.io/badge/XP%20Reward-300%20XP-orange?style=for-the-badge)](.)
[![Time](https://img.shields.io/badge/Time-1--2%20hours-blue?style=for-the-badge)](.)

> *"A merged PR is a conversation with the future. Someone in the future will use what you built today."*

---

## 🎯 Objective

Get a Pull Request **merged** into the DevQuest main branch. This is a major milestone — your code (or content) permanently becomes part of the project!

**Prerequisite**: Complete [Level 2 — First Pull Request](Level-2.md).

---

## 📋 Requirements

To complete Level 3, you must:

- [ ] Have an open PR from Level 2 (or open a new, improved one)
- [ ] **Address** all review feedback from maintainers
- [ ] **Pass** all automated checks (markdown lint, etc.)
- [ ] Have your PR **approved** by at least one maintainer
- [ ] Have your PR **merged** into `main`

---

## 📖 Step-by-Step Instructions

### 1. Check Your PR Status

Visit your open PR. Look for:
- 🟢 **Green checks** — automated tests pass
- 💬 **Review comments** — maintainer feedback to address
- ✅ **Approved** — a maintainer approved your changes
- 🔀 **Merged** — your PR was merged!

### 2. Address Any Feedback

If a maintainer requested changes:

```bash
# Make the requested changes locally
git checkout add/your-username

# Edit the files
# ...

# Stage and commit
git add .
git commit -m "fix: address review feedback"

# Push the update
git push origin add/your-username
```

Your PR will automatically update with the new commits.

### 3. Handle Merge Conflicts

If your branch is behind `main`, you may need to update it:

```bash
# Add the upstream remote (if you haven't already)
git remote add upstream https://github.com/devquest-org/devquest.git

# Fetch latest changes
git fetch upstream

# Rebase your branch onto the latest main
git rebase upstream/main

# Push with force (necessary after rebase)
git push origin add/your-username --force-with-lease
```

### 4. Be Patient & Professional

Maintainers are volunteers. If you haven't heard back in 3–5 days, it's okay to leave a polite comment:

> *"Hi! Just checking in on this PR. Happy to make any changes needed. Thanks for your time!"*

---

## ✅ Verification

Level 3 is complete when your PR shows the purple **"Merged"** badge on GitHub. 🎉

Claim your XP by opening an issue: `[XP] Claim: YOUR_USERNAME - Level 3 Complete`

---

## 🎁 Rewards

- ⭐ **300 XP** — massive XP boost
- 🏅 **"Merged!" badge**
- 🥉 You may now unlock **Contributor** rank (200 total XP)
- Progress toward **Pull Shark** GitHub achievement (merge 2 PRs = Pull Shark, 16 = Gold)
- Your contribution is **permanently part of DevQuest**!

---

## 💡 Tips

> **Tip 1**: The most common reason PRs don't get merged is unclear descriptions. If your PR sits open for a while, consider adding more context to the description.

> **Tip 2**: Be gracious about feedback. Even if you disagree, start by trying to understand the reviewer's perspective.

> **Tip 3**: Small PRs get merged faster than large ones. If you're making multiple changes, split them into separate PRs.

> **Tip 4**: Check that the CI/CD checks all pass. A failing lint check is an easy fix!

> **Tip 5**: After your first PR is merged, check if you've unlocked the **Quickdraw** GitHub achievement on your profile!

---

## 🔍 Understanding the PR Review Process

```
Open PR
   │
   ▼
Automated Checks Run
   │
   ├── ❌ Checks Fail → Fix Issues → Push Update
   │
   ▼
Maintainer Reviews
   │
   ├── 💬 Changes Requested → Address Feedback → Push Update
   │
   ▼
PR Approved
   │
   ▼
Merged! 🎉
```

---

## 📚 Resources

- [🔀 Pull Requests Guide](../RESOURCES/PullRequests.md) — Deep dive into PR workflows
- [🔧 Git Guide](../RESOURCES/Git.md) — Rebasing and conflict resolution
- [🏆 GitHub Achievements](../RESOURCES/GitHubAchievements.md) — Track your achievement progress

---

## 🎓 What You Learned

By completing Level 3, you can:
- Navigate the PR review cycle
- Resolve merge conflicts
- Respond professionally to code review
- Use git rebase
- Understand CI/CD automation

---

## ➡️ What's Next?

You're officially an open source contributor. Time to explore the wider ecosystem!

**[Level 4 → Open Source Explorer](Level-4.md)**

---

<div align="center">

*Your name is now permanently in the history of an open source project. That's something to be proud of!* 🌟

[⬅️ Level 2](Level-2.md) | [🏠 Back to Main](../README.md#-challenge-system) | [➡️ Level 4](Level-4.md)

</div>
