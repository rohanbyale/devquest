# 📝 Markdown — Complete Guide

> *Markdown is a lightweight markup language that converts plain text to formatted HTML. It's the language of GitHub READMEs, documentation, and developer communication.*

---

## 📋 Table of Contents

- [What is Markdown?](#what-is-markdown)
- [Headings](#headings)
- [Text Formatting](#text-formatting)
- [Lists](#lists)
- [Links & Images](#links--images)
- [Code](#code)
- [Tables](#tables)
- [Blockquotes](#blockquotes)
- [Horizontal Rules](#horizontal-rules)
- [GitHub Flavored Markdown](#github-flavored-markdown)
- [Best Practices](#best-practices)

---

## 🤔 What is Markdown?

Markdown was created by John Gruber in 2004. It lets you write using plain text that renders as formatted documents. GitHub uses "GitHub Flavored Markdown" (GFM) — a superset with extra features.

---

## # Headings

```markdown
# H1 — Page Title
## H2 — Major Section
### H3 — Subsection
#### H4 — Sub-subsection
##### H5 — Minor heading
###### H6 — Smallest heading
```

**Best Practice**: Use one H1 per document. Structure with H2 and H3.

---

## ✍️ Text Formatting

```markdown
**Bold text**
*Italic text*
***Bold and italic***
~~Strikethrough~~
`Inline code`
> Blockquote
```

Renders as: **Bold**, *Italic*, ***Both***, ~~Strikethrough~~, `code`

---

## 📋 Lists

### Unordered Lists

```markdown
- Item one
- Item two
  - Nested item
  - Another nested
- Item three
```

### Ordered Lists

```markdown
1. First item
2. Second item
3. Third item
```

### Task Lists (GitHub only)

```markdown
- [x] Completed task
- [ ] Incomplete task
- [ ] Another task
```

---

## 🔗 Links & Images

```markdown
[Link text](https://example.com)
[Link with title](https://example.com "Hover title")
[Relative link](../README.md)
[Reference link][ref-id]

[ref-id]: https://example.com

![Alt text](image.png)
![Alt text](image.png "Image title")
[![Badge](badge-url)](link-url)
```

---

## 💻 Code

### Inline Code

```markdown
Use `git status` to check your working directory.
```

### Fenced Code Blocks

````markdown
```bash
git clone https://github.com/user/repo.git
cd repo
```

```python
def hello():
    print("Hello, World!")
```

```javascript
const greet = (name) => `Hello, ${name}!`;
```
````

Supported languages: `bash`, `python`, `javascript`, `typescript`, `java`, `go`, `rust`, `yaml`, `json`, `markdown`, `html`, `css`, and many more.

---

## 📊 Tables

```markdown
| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Cell 1   | Cell 2   | Cell 3   |
| Cell 4   | Cell 5   | Cell 6   |
```

### Alignment

```markdown
| Left     | Center   | Right    |
|:---------|:--------:|---------:|
| aligned  | aligned  | aligned  |
```

---

## 💬 Blockquotes

```markdown
> Single blockquote

> Multi-line blockquote
> continues here

> Nested blockquote
>> Goes deeper
>>> Even deeper
```

---

## ➖ Horizontal Rules

```markdown
---
***
___
```

All produce a horizontal line.

---

## 🐙 GitHub Flavored Markdown

### Alerts (GitHub only)

```markdown
> [!NOTE]
> Useful information for the reader.

> [!TIP]
> Helpful advice.

> [!IMPORTANT]
> Crucial information.

> [!WARNING]
> Dangerous action warning.

> [!CAUTION]
> Risk of negative consequences.
```

### Collapsed Sections

```markdown
<details>
<summary>Click to expand</summary>

Hidden content here!

</details>
```

### Emoji

```markdown
:rocket: :fire: :tada: :white_check_mark: :x:
```

Renders: 🚀 🔥 🎉 ✅ ❌

### Mentions & References

```markdown
@username          — mention a user
#123               — reference an issue/PR
owner/repo#123     — cross-repo reference
SHA (abc1234)      — reference a commit
```

### Footnotes

```markdown
Here is a claim.[^1]

[^1]: Here is the footnote explanation.
```

---

## ✅ Best Practices

1. **One H1 per file** — multiple H1s confuse structure
2. **Blank lines around elements** — headings, lists, and code blocks need breathing room
3. **Consistent list markers** — pick `-` or `*` and stick with it
4. **Alt text for images** — always describe what the image shows
5. **Use relative links** — for files within the same repository
6. **Preview before committing** — GitHub's preview tab shows exactly how it renders
7. **Keep lines short** — ~80-120 characters for readability in raw form

---

## 📚 Further Reading

- [Markdown Guide](https://www.markdownguide.org) — Comprehensive reference
- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/)
- [Dillinger](https://dillinger.io) — Online Markdown editor with preview

---

*Next: [Pull Requests Guide →](PullRequests.md)*
