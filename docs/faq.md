# ❓ Frequently Asked Questions

Can't find your answer? [Open a Discussion](https://github.com/your-org/devquest/discussions)!

---

## 🔰 Getting Started

**Q: I've never contributed to open source. Is DevQuest for me?**

> Absolutely. DevQuest was built specifically for people at your stage. Levels 1 and 2 require zero coding skills — just a GitHub account and enthusiasm. Start with [Getting Started](getting-started.md).

**Q: Do I need to know how to code?**

> Not for the first two levels! Adding yourself to `CONTRIBUTORS.md` is editing a text file. Coding skills help for Level 4+ and Bonus Challenges, but even then, documentation contributions are always welcome.

**Q: What tools do I need?**

> A GitHub account, Git, and a text editor. See the [Getting Started Guide](getting-started.md) for installation instructions. Everything is free.

**Q: How long do the challenges take?**

> - Level 1: ~15 minutes
> - Level 2: ~30 minutes
> - Level 3: A few hours (waiting for review)
> - Level 4: 1–2 weeks
> - Level 5: Ongoing (60 days)
> - Bonus: Variable (1 day to several weeks)

---

## 🏅 XP & Ranking

**Q: How is XP tracked?**

> Currently, XP is tracked manually. After completing a challenge, open an issue titled `[XP Claim] YOUR_USERNAME - Challenge Name` with a link to your merged PR. A maintainer will verify and update the leaderboard.

> Automated XP tracking is on our [roadmap](roadmap.md)!

**Q: Can I skip levels?**

> Levels should be completed in order since each builds on the last. However, Bonus Challenges can be attempted any time after Level 2.

**Q: I completed a challenge but haven't received XP. What do I do?**

> Open an issue with the title `[XP Claim] YOUR_USERNAME - Challenge Name` and include a link to your merged PR. We'll process it within 48 hours.

**Q: Does contributing to repos other than DevQuest count for XP?**

> For Level 4 and Bonus Challenges, yes — contributions to external projects are required and count toward your XP claim. For Levels 1–3, contributions must be to DevQuest directly.

---

## 🔀 Pull Requests

**Q: My PR has been open for a week with no response. What should I do?**

> Leave a polite comment: *"Hi! Just checking in on this PR — happy to make any changes needed. Thanks for your time!"* Maintainers are volunteers; a gentle nudge after 5–7 days is perfectly reasonable.

**Q: A maintainer requested changes but I don't understand the feedback. What should I do?**

> Reply in the PR comments asking for clarification: *"Could you help me understand what you mean by X? I want to make sure I fix it correctly."* Asking is always the right move.

**Q: My PR has a merge conflict. What should I do?**

> ```bash
> git fetch upstream
> git rebase upstream/main
> # Resolve conflicts
> git push origin your-branch --force-with-lease
> ```
> See the [Git Guide](../RESOURCES/Git.md) for details on resolving conflicts.

**Q: I accidentally opened a PR to my fork instead of the main repo. How do I fix it?**

> Edit the base repository in your PR (click "Edit" at the top). Change it to `devquest-org/devquest` with base `main`. If that's not possible, close the PR and open a new one.

---

## 🐛 Technical Issues

**Q: I get "Permission denied" when pushing. What's wrong?**

> You're probably trying to push to the original repository instead of your fork. Make sure the remote URL contains YOUR username:
> ```bash
> git remote -v
> # Should show: origin https://github.com/YOUR_USERNAME/devquest.git
> ```
> If not: `git remote set-url origin https://github.com/YOUR_USERNAME/devquest.git`

**Q: I cloned the original repo, not my fork. What do I do?**

> ```bash
> # Option 1: Delete and re-clone your fork
> cd ..
> rm -rf devquest
> git clone https://github.com/YOUR_USERNAME/devquest.git
>
> # Option 2: Change the remote URL
> git remote set-url origin https://github.com/YOUR_USERNAME/devquest.git
> ```

**Q: My commits show the wrong email/name. How do I fix it?**

> ```bash
> git config --global user.name "Your Name"
> git config --global user.email "your@email.com"
> # Amend recent commits:
> git commit --amend --reset-author
> ```

**Q: The GitHub Actions check is failing on my PR. What do I do?**

> Click "Details" next to the failing check to see the error. Most lint failures are formatting issues — an extra space, a missing newline, etc. Fix the issue, commit, and push — the check will re-run automatically.

---

## 🌍 Community

**Q: Can I contribute in a language other than English?**

> Yes! We welcome translations. See [Bonus Challenge B5 — Translator](../CHALLENGES/Bonus-Challenges.md#b5--translator) for details. Create translated files with language code suffixes (e.g., `README.es.md`).

**Q: How can I become a maintainer?**

> Reach Level 5 (Community Contributor), consistently make quality contributions, and help new contributors. We'll reach out to active, trusted community members when we're looking for maintainers.

**Q: Can I suggest a new challenge?**

> Absolutely! Use the [Challenge Submission issue template](https://github.com/your-org/devquest/issues/new/choose) to propose your idea. Good challenge ideas are specific, achievable, educational, and build on previous levels.

**Q: Is there a Discord/Slack/chat?**

> A Discord server is on the [roadmap](roadmap.md)! For now, use GitHub Discussions for community conversations.

---

## 🤔 About DevQuest

**Q: Is DevQuest affiliated with GitHub?**

> No. DevQuest is an independent community project. We use GitHub as our platform, but we are not affiliated with, sponsored by, or endorsed by GitHub Inc.

**Q: Is DevQuest free?**

> Yes, 100% free. Always will be.

**Q: Can I use DevQuest in my classroom or bootcamp?**

> Yes! DevQuest is MIT licensed, which means you're free to use, fork, and adapt it for educational purposes. We'd love to hear how you're using it — share in GitHub Discussions!

**Q: How can I support DevQuest?**

> - ⭐ Star the repository
> - 🔀 Contribute (any level)
> - 📣 Share with friends and on social media
> - 💰 Sponsor the maintainers via GitHub Sponsors

---

*Still stuck? [Open a Discussion](https://github.com/your-org/devquest/discussions) and the community will help!*
