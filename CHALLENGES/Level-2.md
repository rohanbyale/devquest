# 🛡️ Level 2 — First Pull Request

[![Difficulty](https://img.shields.io/badge/Difficulty-Beginner-brightgreen?style=for-the-badge)](.)
[![XP Reward](https://img.shields.io/badge/XP%20Reward-150%20XP-orange?style=for-the-badge)](.)
[![Time](https://img.shields.io/badge/Time-30%20mins-blue?style=for-the-badge)](.)

> *"A pull request is an act of courage — you're saying 'here is my work, please look at it.' That takes guts."*

---

## 🎯 Objective

Open your first Pull Request on the DevQuest repository. You'll submit the changes you made in Level 1 (or any improvement you'd like to contribute) as an official PR.

**Prerequisite**: Complete [Level 1 — First Fork](Level-1.md) first.

---

## 📋 Requirements

To complete Level 2, you must:

- [ ] Have completed Level 1 (your branch exists with changes)
- [ ] **Open** a Pull Request from your fork to the `main` branch of DevQuest
- [ ] **Fill in** the PR template completely
- [ ] **Use** a proper PR title: `feat: add YOUR_USERNAME to contributors`
- [ ] **Wait** for at least one review comment or approval
- [ ] **Respond** to any feedback (if given)

---

## 📖 Step-by-Step Instructions

### 1. Navigate to GitHub

Go to your forked repository: `https://github.com/rohanbyale/devquest.git`

### 2. Open the Pull Request

You should see a yellow banner saying **"Compare & pull request"**. Click it!

If you don't see the banner:
1. Click the **"Pull requests"** tab
2. Click **"New pull request"**
3. Set **base repository** to `devquest/devquest` and **base** to `main`
4. Set **head repository** to `YOUR_USERNAME/devquest` and **compare** to `add/your-username`

### 3. Fill in the PR Template

You'll see a template automatically. Fill it in properly:

```markdown
## Description
Added my username to the CONTRIBUTORS.md file as part of the Level 1 & 2 DevQuest challenge.

## Type of Change
- [x] New contributor entry

## Checklist
- [x] My changes follow the style guidelines
- [x] I have added myself in alphabetical order
- [x] My entry uses the correct format
```

### 4. Write a Good PR Title

Use the Conventional Commits format:
```
feat: add octocat to contributors
```

### 5. Submit the PR

Click **"Create pull request"** — congratulations, you've opened your first PR! 🎉

### 6. Wait and Engage

A maintainer will review your PR. They might:
- ✅ Approve and merge it
- 💬 Leave a comment requesting changes
- ❓ Ask a question

Respond respectfully and promptly!

---

## ✅ Verification

Level 2 is complete when:
- Your PR is open and visible on the DevQuest repository
- The PR has a proper title, description, and filled template
- You have responded to any review feedback

---

## 🎁 Rewards

- ⭐ **150 XP** (100 XP + 50 XP bonus for Level 1)
- 🏅 **"First PR" badge**
- 🥉 You're on your way to **Contributor** rank!
- **Quickdraw** GitHub achievement progress (merge within 5 mins of opening your first issue)

---

## 💡 Tips

> **Tip 1**: A good PR description is as important as the code itself. Take time to explain *what* you changed and *why*.

> **Tip 2**: Don't be nervous about review comments — they're not criticism, they're collaboration! Every comment makes the project better.

> **Tip 3**: If your PR has conflicts with the base branch, run:
> ```bash
> git fetch upstream
> git rebase upstream/main
> git push --force-with-lease
> ```

> **Tip 4**: Check the PR "Files changed" tab to verify your changes look correct before submitting.

> **Tip 5**: If you accidentally opened a PR to the wrong branch, you can change the base branch using the "Edit" button at the top of your PR.

---

## 📚 Resources

- [🔀 Pull Requests Guide](../RESOURCES/PullRequests.md) — Everything about PRs
- [🐙 GitHub Guide](../RESOURCES/GitHub.md) — GitHub workflow explained
- [🔧 Git Guide](../RESOURCES/Git.md) — Git commands reference

---

## 🎓 What You Learned

By completing Level 2, you now know how to:
- Open a Pull Request
- Write a clear PR description
- Respond to review feedback
- Work with the GitHub PR interface

---

## ➡️ What's Next?

Get your PR merged to unlock Level 3!

**[Level 3 → First Merged PR](Level-3.md)**

---

<div align="center">

*The open source community is waiting for your contribution!* 🌍

[⬅️ Level 1](Level-1.md) | [🏠 Back to Main](../README.md#-challenge-system) | [➡️ Level 3](Level-3.md)

</div>
