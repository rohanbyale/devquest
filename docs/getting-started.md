# 🚀 Getting Started with DevQuest

Welcome! This guide will get you from zero to your first open source contribution in under 30 minutes.

---

## Prerequisites

You'll need:

- [ ] A [GitHub account](https://github.com/signup) (free)
- [ ] [Git installed](https://git-scm.com/downloads) on your computer
- [ ] A text editor ([VS Code](https://code.visualstudio.com) recommended)
- [ ] A terminal (Terminal on Mac/Linux, Git Bash on Windows)

That's it — no coding experience required for the first two levels!

---

## Step 1: Set Up Git (5 minutes)

If you've never used Git before, configure it first:

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

Verify it worked:

```bash
git config --list
# Should show your name and email
```

---

## Step 2: Star This Repository ⭐

Go to the [DevQuest repository](https://github.com/your-org/devquest) and click the **Star** button. This helps others find the project and earns you good karma! 😄

---

## Step 3: Fork the Repository

Click **Fork** in the top right of the DevQuest page.

Select your account as the destination. GitHub will create a copy at:
`https://github.com/YOUR_USERNAME/devquest`

---

## Step 4: Clone Your Fork

```bash
# Replace YOUR_USERNAME with your actual GitHub username
git clone https://github.com/YOUR_USERNAME/devquest.git

# Navigate into the folder
cd devquest
```

You should now see all the DevQuest files on your computer.

---

## Step 5: Create Your Branch

```bash
git checkout -b add/your-github-username
```

Replace `your-github-username` with your actual username. Example: `git checkout -b add/octocat`

---

## Step 6: Add Yourself to CONTRIBUTORS.md

Open `CONTRIBUTORS.md` in your text editor and add your row to the contributors table.

Find this section:

```markdown
| GitHub Profile | Rank | Highest Level | XP | Joined |
```

Add your row in alphabetical order by username:

```markdown
| [your-username](https://github.com/your-username) | 🔰 Rookie | Level 1 | 50 XP | June 2025 |
```

Save the file.

---

## Step 7: Commit and Push

```bash
# Stage your change
git add CONTRIBUTORS.md

# Commit it
git commit -m "feat: add your-username to contributors"

# Push to GitHub
git push origin add/your-github-username
```

---

## Step 8: Open Your First Pull Request

1. Go to your fork on GitHub: `https://github.com/YOUR_USERNAME/devquest`
2. You'll see a yellow banner — click **"Compare & pull request"**
3. Fill in the PR description
4. Click **"Create pull request"**

🎉 **Congratulations! You just opened your first pull request!**

---

## What Happens Next?

1. A maintainer will review your PR (usually within 1–3 days)
2. They may leave feedback — respond to it kindly
3. Once approved, your PR gets merged
4. You earn XP and your name appears in the project forever!

---

## Stuck?

Check these resources:
- [Git Guide](../RESOURCES/Git.md) — Git commands explained
- [GitHub Guide](../RESOURCES/GitHub.md) — GitHub walkthrough
- [FAQ](faq.md) — Common questions answered
- [Open an Issue](https://github.com/your-org/devquest/issues/new) — Ask for help

---

## Next Steps

After your first merged PR, explore the full challenge system:

| Level | What You'll Do |
|-------|---------------|
| [Level 1](../CHALLENGES/Level-1.md) | Fork & clone the repo |
| [Level 2](../CHALLENGES/Level-2.md) | Open your first PR |
| [Level 3](../CHALLENGES/Level-3.md) | Get your PR merged |
| [Level 4](../CHALLENGES/Level-4.md) | Contribute to external projects |
| [Level 5](../CHALLENGES/Level-5.md) | Mentor others |
| [Bonus](../CHALLENGES/Bonus-Challenges.md) | Extra XP challenges |

---

*You've got this. Every expert was once a beginner.* 💪
