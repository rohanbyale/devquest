# 💎 Bonus Challenges

[![Difficulty](https://img.shields.io/badge/Difficulty-Variable-purple?style=for-the-badge)](.)
[![XP Reward](https://img.shields.io/badge/XP%20Reward-200%20XP%20each-orange?style=for-the-badge)](.)

> *"True growth happens outside your comfort zone. These challenges will push you further."*

Bonus Challenges can be attempted **at any time** after completing Level 2. They award **200 XP each** and count toward your total rank score.

---

## 💎 Challenge List

| # | Challenge | XP | Difficulty |
|---|-----------|-----|------------|
| B1 | [🐛 Bug Hunter](#b1--bug-hunter) | 200 | 🟡 Intermediate |
| B2 | [👁️ PR Reviewer](#b2-️-pr-reviewer) | 200 | 🟡 Intermediate |
| B3 | [🤝 Beginner Helper](#b3--beginner-helper) | 200 | 🟢 Any level |
| B4 | [📚 Documentation Champion](#b4--documentation-champion) | 200 | 🟡 Intermediate |
| B5 | [🌐 Translator](#b5--translator) | 200 | 🟡 Intermediate |
| B6 | [🔭 Issue Archaeologist](#b6--issue-archaeologist) | 200 | 🔴 Advanced |
| B7 | [⭐ Star Curator](#b7--star-curator) | 200 | 🟢 Beginner |
| B8 | [🎓 Knowledge Sharer](#b8--knowledge-sharer) | 200 | 🔴 Advanced |

---

## B1 🐛 Bug Hunter

**Objective**: Find and report a real, reproducible bug in DevQuest.

### Requirements
- [ ] Find a legitimate bug (broken link, formatting issue, incorrect info, workflow failure)
- [ ] Open a detailed bug report using the [bug report template](.github/ISSUE_TEMPLATE/bug_report.yml)
- [ ] Include reproduction steps and screenshots
- [ ] Bug must be confirmed by a maintainer

### What Counts
- Broken links
- Incorrect information in guides
- Formatting issues that make content unreadable
- GitHub Actions failures
- Template errors

### Tips
- Read every file carefully — there are likely issues waiting to be found
- Try the workflows yourself; if something doesn't work as described, it's a bug
- Check all links in the Resources folder

### Reward
- ✅ **200 XP** on confirmed bug
- 🏅 **"Bug Hunter" badge**

---

## B2 👁️ PR Reviewer

**Objective**: Review **5 Pull Requests** with high-quality, constructive feedback.

### Requirements
- [ ] Review 5 different open PRs in DevQuest
- [ ] Each review must include specific, actionable feedback (not just "LGTM")
- [ ] At least 3 of your reviews must be "Request Changes" or "Approve" type (not just Comment)
- [ ] No reviews on your own PRs

### What Makes a Good Review

```markdown
✅ Good Review:
"The entry on line 47 needs to be moved — alphabetically, 'sarah' comes before
'tom', so your entry should be above @tomsmith's. Also, the XP column should say
'50 XP' not just '50'. Otherwise this looks great — nice work on your first PR!"

❌ Poor Review:
"Looks good!"
```

### Tips
- Check the Files Changed tab carefully
- Look at the contributor table for ordering issues
- Verify all links work
- Check commit message format

### Reward
- ✅ **200 XP** after 5 quality reviews
- 🏅 **"Reviewer" badge**
- Progress toward **Galaxy Brain** GitHub achievement

---

## B3 🤝 Beginner Helper

**Objective**: Help **3 newcomers** successfully complete their first PR.

### Requirements
- [ ] Find 3 newcomers struggling with their PR (check open PRs and issues)
- [ ] Leave helpful, step-by-step guidance in comments
- [ ] Guide them to success without doing it for them
- [ ] All 3 of those newcomers must get their PRs merged

### How to Find Newcomers

- Look for PRs with no review activity
- Check issues with questions from new users
- Look for PRs that have been open for 3+ days without merge

### Sample Helpful Comment

```markdown
Hey @newcomer! 👋 Welcome to DevQuest!

I noticed your PR needs a small fix — your entry in CONTRIBUTORS.md
appears to be slightly out of alphabetical order. The contributor above
yours starts with 'j' (james) and below starts with 'm' (mike), so your
entry with 'k' is correct there ✅

However, I noticed the XP column says just "XP" instead of "50 XP".
Quick fix: change that cell to "50 XP".

Let me know if you have any questions — happy to help! 🎉
```

### Reward
- ✅ **200 XP**
- 🏅 **"Helper" badge**
- Counts toward Level 5 requirements

---

## B4 📚 Documentation Champion

**Objective**: Write or significantly improve a learning resource in the `RESOURCES/` folder.

### Requirements
- [ ] Write a new guide OR significantly expand an existing one (500+ words added)
- [ ] Include practical examples and code snippets
- [ ] Add a table of contents if the guide is long
- [ ] Get the PR merged by a maintainer

### Ideas for New Guides

- `RESOURCES/GitHub-Actions.md` — Introduction to GitHub Actions
- `RESOURCES/VSCode.md` — Using VS Code for open source
- `RESOURCES/Terminal.md` — Command line basics
- `RESOURCES/Python-OS.md` — Contributing to Python open source projects
- `RESOURCES/JavaScript-OS.md` — Contributing to JavaScript projects

### Quality Bar

Your guide should:
- Be readable by a complete beginner
- Include real, working examples
- Have clear headings and structure
- Link to external resources for further reading

### Reward
- ✅ **200 XP**
- 🏅 **"Doc Champion" badge**

---

## B5 🌐 Translator

**Objective**: Translate a DevQuest file into another language.

### Requirements
- [ ] Choose a file to translate (start with README.md or a challenge file)
- [ ] Create a new file with language code suffix: e.g., `README.zh.md`, `README.es.md`
- [ ] Translate accurately — use a native speaker review if possible
- [ ] Submit PR with the translated file

### Supported Languages (add yours!)

| Language | Code | Status |
|----------|------|--------|
| Spanish | `es` | 🔜 Wanted |
| French | `fr` | 🔜 Wanted |
| Portuguese | `pt` | 🔜 Wanted |
| German | `de` | 🔜 Wanted |
| Chinese (Simplified) | `zh` | 🔜 Wanted |
| Japanese | `ja` | 🔜 Wanted |
| Hindi | `hi` | 🔜 Wanted |
| Arabic | `ar` | 🔜 Wanted |

### Tips
- Translate the meaning, not just the words — idiomatic phrasing matters
- Keep code examples in English
- Keep commands and technical terms in English
- Don't translate username examples

### Reward
- ✅ **200 XP**
- 🏅 **"Globetrotter" badge**

---

## B6 🔭 Issue Archaeologist

**Objective**: Triage and close **10 stale issues** by providing solutions or confirming they're fixed.

### Requirements
- [ ] Find 10 open issues that are outdated, already fixed, or unclear
- [ ] For each: comment explaining the status and ask if the issue is still valid
- [ ] Help close issues by fixing the underlying problem (if possible)
- [ ] Work with maintainers to close or update issues

### Types of Issues to Look For

- Issues that reference outdated content now fixed
- Duplicate issues
- Issues with no response from the reporter in 30+ days
- Issues that have been resolved by other PRs but not closed

### Template Comment

```markdown
Hi @reporter! 👋 Thanks for opening this issue.

I wanted to check in — is this still an issue for you? I believe this may have
been addressed in PR #XX. If you can confirm it's fixed, we can close this issue.

If the problem persists, please let us know and we'll take another look! 🙏
```

### Reward
- ✅ **200 XP**
- 🏅 **"Archaeologist" badge**

---

## B7 ⭐ Star Curator

**Objective**: Create a curated list of 20+ open source projects with descriptions for beginners.

### Requirements
- [ ] Create `RESOURCES/CuratedProjects.md`
- [ ] List 20+ beginner-friendly open source projects
- [ ] Each project needs: name, link, language, difficulty, why it's great
- [ ] Group projects by category or language
- [ ] Get the PR merged

### Template

```markdown
| Project | Language | Difficulty | Why It's Great |
|---------|----------|------------|----------------|
| [first-contributions](https://github.com/firstcontributions/first-contributions) | Markdown | 🟢 Beginner | Made for first-timers |
```

### Categories to Cover
- JavaScript/Node.js projects
- Python projects
- Documentation projects
- Tools and utilities
- Frameworks

### Reward
- ✅ **200 XP**
- 🏅 **"Curator" badge**

---

## B8 🎓 Knowledge Sharer

**Objective**: Write and publish a blog post or tutorial about your DevQuest journey.

### Requirements
- [ ] Write a 500+ word post on any platform (DEV.to, Hashnode, Medium, personal blog)
- [ ] Include your DevQuest experience and what you learned
- [ ] Link back to the DevQuest repository
- [ ] Share the link in a DevQuest issue or discussion

### Post Ideas
- *"How I Made My First Open Source Contribution in 30 Minutes"*
- *"DevQuest: The Gamified Path to Open Source"*
- *"What I Learned from My First 5 Pull Requests"*
- *"From Zero to Open Source Contributor: My DevQuest Story"*

### Reward
- ✅ **200 XP**
- 🏅 **"Knowledge Sharer" badge**
- Your post linked in the DevQuest README (if quality is high)

---

## 📋 Claiming Bonus Challenge XP

For each completed bonus challenge:

1. Open an issue titled: `[XP Claim] Bonus B# Complete - YOUR_USERNAME`
2. Include links to evidence (PRs, issues, external posts)
3. A maintainer will verify and award XP

---

<div align="center">

*Bonus challenges are where legends are made. How many can you complete?* 💎

[🏠 Back to Main](../README.md#-challenge-system) | [⬅️ Level 5](Level-5.md)

</div>
