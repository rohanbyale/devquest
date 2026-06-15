# 🔀 Pull Requests — Complete Guide

> *A pull request is the heart of open source collaboration. Mastering PRs is mastering open source.*

---

## 📋 Table of Contents

- [What is a Pull Request?](#what-is-a-pull-request)
- [Before Opening a PR](#before-opening-a-pr)
- [Opening a Pull Request](#opening-a-pull-request)
- [Writing Great PR Descriptions](#writing-great-pr-descriptions)
- [The Review Process](#the-review-process)
- [Responding to Feedback](#responding-to-feedback)
- [Updating Your PR](#updating-your-pr)
- [Merge Types](#merge-types)
- [Reviewing Others' PRs](#reviewing-others-prs)
- [Common Mistakes](#common-mistakes)
- [PR Checklist](#pr-checklist)

---

## 🤔 What is a Pull Request?

A Pull Request (PR) is a proposal to merge changes from one branch into another. It's a formal request saying: *"Here are my changes — please review them and consider merging them."*

PRs enable:
- **Code review** — Others can inspect your changes
- **Discussion** — Comments and suggestions on specific lines
- **CI/CD** — Automated tests run before merging
- **Documentation** — A permanent record of why a change was made

---

## 🏁 Before Opening a PR

### 1. Understand the Project's Contribution Guidelines

Read `CONTRIBUTING.md` before doing anything else. It will tell you:
- Branch naming conventions
- Commit message format
- PR template requirements
- Which branch to target

### 2. Make Sure Your Branch is Up-to-Date

```bash
git fetch upstream
git rebase upstream/main
```

This prevents merge conflicts after you open the PR.

### 3. Test Your Changes

Even for documentation PRs, check that:
- All links work
- Formatting renders correctly
- No typos or errors

### 4. Keep It Small

One PR = one purpose. If you're fixing a bug AND adding a feature, open two PRs.

---

## 🚀 Opening a Pull Request

### On GitHub

1. Push your branch: `git push origin your-branch`
2. Visit the repository on GitHub
3. Click **"Compare & pull request"** (or go to Pull Requests → New)
4. Select the correct base branch (usually `main`)
5. Fill in the PR template
6. Click **"Create pull request"**

### Draft PRs

If your work is in progress, open a **Draft PR**:
- Click the dropdown arrow next to "Create pull request"
- Select "Create draft pull request"
- Converts reviewers from being notified until you're ready
- Mark as ready when done: **"Ready for review"**

---

## ✍️ Writing Great PR Descriptions

A great PR description answers three questions:
1. **What** changed?
2. **Why** was it changed?
3. **How** was it tested/verified?

### Example: Poor Description

```markdown
Fixed stuff.
```

### Example: Great Description

```markdown
## Description

Fixed a broken link in `RESOURCES/Git.md` that pointed to a 404 page.
Updated it to the correct URL at git-scm.com.

## Why

New contributors following the Git guide were hitting a dead end
when trying to learn about rebasing. This fix removes that friction.

## Changes Made

- Updated link on line 142 in `RESOURCES/Git.md`
- Verified the new URL is active and points to the correct section

## Testing

- [ ] Clicked the link in the preview — it loads correctly
- [ ] Checked for any other broken links in the same file

Closes #89
```

### PR Title Format

Use Conventional Commits:
```
feat: add JavaScript resources guide
fix: correct broken link in Git.md
docs: improve getting started instructions
chore: update contributors list
```

---

## 👁️ The Review Process

### What Happens After You Open a PR

```
PR Opened
    │
    ▼
Automated Checks (CI)
    │
    ├── ❌ Checks fail → Fix and push
    │
    ▼
Maintainer Reviews
    │
    ├── 💬 Changes requested → Make changes → Push
    ├── ❓ Questions → Answer in comments
    │
    ▼
PR Approved ✅
    │
    ▼
Merged 🎉
```

### Types of Reviews

| Review Type | Meaning | Action Required |
|-------------|---------|-----------------|
| 💬 Comment | Feedback without explicit approval | Address if needed |
| ✅ Approve | LGTM — ready to merge | Wait for merge |
| 🔄 Request Changes | Must be fixed before merge | Fix and push |

### Review Timeline

Most projects don't have SLAs. Be patient:
- Small projects: 1–7 days
- Large projects: 1–4 weeks
- Very active projects: hours

If you haven't heard back after 5–7 days, a polite ping is appropriate.

---

## 💬 Responding to Feedback

### The Right Mindset

Review comments are not personal. Every comment makes the project better. Reviewers are volunteering their time to help you improve.

### Responding to Comments

**Acknowledge**: Always reply to show you've read the comment.

```markdown
# Simple fix
Done! Fixed in the latest commit.

# Disagreement (polite)
Thanks for the feedback! I initially used X approach because [reason].
Would Y approach work better? Happy to change if so.

# Question about the feedback
Could you clarify what you mean by "inconsistent formatting" here?
I want to make sure I fix it correctly.
```

**Resolve threads**: After fixing, mark conversations as "Resolved" (but the reviewer usually does this).

### When You Disagree

1. Understand the reviewer's perspective first
2. State your case clearly and respectfully
3. Provide evidence or reasoning
4. Defer to the maintainer's final decision
5. Accept it gracefully even if you disagree

---

## 🔄 Updating Your PR

After making changes based on feedback:

```bash
# Make your changes
# ...

# Stage and commit
git add .
git commit -m "fix: address review feedback - correct formatting"

# Push to the same branch — PR updates automatically
git push origin your-branch
```

You don't need to close and reopen — GitHub automatically shows new commits.

### After a Rebase

If you need to rebase (to fix conflicts or stay up to date):

```bash
git fetch upstream
git rebase upstream/main
# Resolve any conflicts...
git push origin your-branch --force-with-lease
```

`--force-with-lease` is safer than `--force` — it fails if someone else pushed to your branch.

---

## 🔀 Merge Types

### Merge Commit

```
main:    A --- B --- C --- M
                     \   /
feature:          D - E
```

Preserves full branch history. Good for feature branches.

### Squash and Merge

```
main:    A --- B --- C --- [D+E]
```

All commits squashed into one. Good for messy commit histories.

### Rebase and Merge

```
main:    A --- B --- C --- D' --- E'
```

Replays commits onto main. Keeps linear history.

Most projects state their preference in CONTRIBUTING.md.

---

## 👀 Reviewing Others' PRs

Reviewing others' PRs is one of the most valuable contributions you can make.

### How to Review

1. Go to the PR's **"Files changed"** tab
2. Read the description first
3. Review changes top to bottom
4. Click `+` on any line to add a comment
5. Click **"Review changes"** to submit

### Review Comments — Do's and Don'ts

```markdown
# ❌ Vague and unhelpful
"This is wrong."
"Bad approach."

# ✅ Specific and constructive
"The link on line 42 appears to be broken — it returns a 404.
The correct URL should be https://example.com/correct-path"

# ❌ Demanding
"You need to fix this before I approve."

# ✅ Collaborative
"Could you update this to use the format shown in line 10?
That would keep it consistent with the rest of the file."
```

### Nit Comments

For minor style issues, prefix with `nit:` to signal it's optional:

```markdown
nit: could add a period at the end of this sentence.
```

---

## ⚠️ Common Mistakes

| Mistake | How to Avoid |
|---------|--------------|
| PRing directly to main on your fork | Always create a new branch |
| Not filling in the PR template | Templates exist for a reason — fill them in |
| Huge PRs with many changes | One change per PR |
| Ignoring CI failures | Fix failing checks before requesting review |
| Disappearing after opening a PR | Stay engaged and respond to feedback |
| Force pushing without warning | Give reviewers a heads-up |

---

## ✅ PR Checklist

Before submitting any PR:

```
Branch & Commits
 □ Working on a branch (not main)
 □ Branch name follows conventions
 □ Commits follow message format
 □ No unrelated changes mixed in

Content
 □ Changes do what the title says
 □ No leftover debug code or comments
 □ Links are working
 □ No typos or formatting issues

PR Description
 □ Title follows convention
 □ Description explains what AND why
 □ Related issues linked (Closes #X)
 □ Template filled in completely

Final Check
 □ CI checks are passing
 □ PR is targeted at the correct branch
 □ Reviewed your own "Files changed" tab
```

---

## 📚 Further Reading

- [GitHub PR Documentation](https://docs.github.com/en/pull-requests)
- [How to Write a Perfect Pull Request](https://github.blog/developer-skills/github/how-to-write-the-perfect-pull-request/)

---

*Next: [GitHub Achievements →](GitHubAchievements.md)*
