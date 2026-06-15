# 🤝 Contributing to DevQuest

First off — **thank you** for considering contributing to DevQuest! 🎉

Every contribution, no matter how small, makes this project better for thousands of developers starting their open source journey. This document explains how you can get involved.

---

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Your First Contribution](#your-first-contribution)
- [Pull Request Process](#pull-request-process)
- [Commit Message Guidelines](#commit-message-guidelines)
- [Style Guide](#style-guide)
- [Community](#community)

---

## 📜 Code of Conduct

This project follows our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you agree to uphold it. Please report unacceptable behavior to the maintainers.

---

## 💡 How Can I Contribute?

### 🐛 Report Bugs

Found something broken? Open an issue using our [Bug Report template](.github/ISSUE_TEMPLATE/bug_report.yml).

Include:
- What you expected to happen
- What actually happened
- Steps to reproduce
- Screenshots if helpful

### 💬 Suggest Features

Have an idea? Open an issue using our [Feature Request template](.github/ISSUE_TEMPLATE/feature_request.yml).

### 📝 Improve Documentation

Our docs can always be better! Fix typos, clarify instructions, add examples, or translate content.

### ✅ Complete Challenges

The most fun contribution — work through the [challenge system](CHALLENGES/) and add yourself to the leaderboard.

### 👀 Review Pull Requests

Experienced contributors can help by reviewing open pull requests, leaving constructive feedback, and helping maintainers triage.

### ⭐ Star & Share

Star this repo and share it with friends. It costs nothing and helps others discover DevQuest.

---

## 🚀 Your First Contribution

Never contributed to open source before? Start here!

### Step 1: Fork the Repository

Click the **Fork** button at the top right of this page. This creates a copy of DevQuest in your GitHub account.

### Step 2: Clone Your Fork

```bash
git clone https://github.com/YOUR_USERNAME/devquest.git
cd devquest
```

### Step 3: Create a Branch

Always work in a new branch — never directly on `main`.

```bash
git checkout -b type/your-description
# Examples:
# git checkout -b feat/add-python-challenge
# git checkout -b fix/typo-in-readme
# git checkout -b docs/improve-git-guide
```

### Step 4: Make Your Changes

Edit files, add content, fix bugs — whatever your contribution is.

### Step 5: Commit Your Changes

```bash
git add .
git commit -m "feat: describe what you did"
```

See [Commit Message Guidelines](#commit-message-guidelines) below.

### Step 6: Push & Open a PR

```bash
git push origin your-branch-name
```

Then go to GitHub and click **"Compare & pull request"**. Fill in the PR template and submit!

---

## 🔀 Pull Request Process

1. **Fill in the PR template** completely — don't skip sections
2. **Link to related issues** using `Closes #123`
3. **Keep PRs focused** — one feature or fix per PR
4. **Respond to feedback** — maintainers may request changes
5. **Be patient** — reviews take time; we're all volunteers

### PR Requirements

- [ ] PR title follows the format: `type: short description`
- [ ] PR description explains *what* and *why*
- [ ] All markdown files are valid
- [ ] No broken links introduced
- [ ] Changes are in scope of the PR description

---

## 📝 Commit Message Guidelines

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
type(scope): short description

[optional body]
[optional footer]
```

### Types

| Type | Use When |
|------|----------|
| `feat` | Adding new content or features |
| `fix` | Fixing bugs, typos, or broken links |
| `docs` | Documentation-only changes |
| `chore` | Maintenance, dependencies |
| `refactor` | Restructuring without changing content |
| `style` | Formatting, whitespace |

### Examples

```bash
feat: add Level 3 challenge for first merged PR
fix: correct broken link in Git.md
docs: improve getting started instructions
chore: update contributor list
```

---

## 🎨 Style Guide

### Markdown

- Use ATX-style headings (`##` not underlines)
- Use `-` for unordered lists (not `*` or `+`)
- Leave one blank line before and after headings
- Use fenced code blocks with language identifiers

```markdown
```bash
echo "Hello, World!"
```
```

- Keep line length under 120 characters
- Use relative links for internal files

### Emojis

Emojis are encouraged in documentation but use them purposefully. Each section heading should have a relevant emoji. Don't overload paragraphs.

### Tone

- Friendly, encouraging, and inclusive
- Second person ("you") when addressing the reader
- Active voice where possible
- Avoid jargon without explanation

---

## 🌍 Community

- **Discussions**: Use GitHub Discussions for questions and ideas
- **Issues**: Bug reports and feature requests only
- **Pull Requests**: Code and content contributions

### Getting Help

Stuck? Here's how to get help:
1. Check the [FAQ](docs/faq.md)
2. Search existing [Issues](https://github.com/your-org/devquest/issues)
3. Open a [Discussion](https://github.com/your-org/devquest/discussions)
4. Ask in your PR — maintainers are happy to help

---

## 🏆 Recognition

Every contributor is added to [CONTRIBUTORS.md](CONTRIBUTORS.md) and the monthly leaderboard. Top contributors earn special mentions in our README Hall of Fame.

Thank you for making DevQuest awesome! 🗡️✨
