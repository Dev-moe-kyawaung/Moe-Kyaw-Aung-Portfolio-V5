# Contributing to Moe-Kyaw-Aung-portfolio-V5

Thank you for your interest in contributing! 🎉  
This document explains how to contribute effectively and respectfully.

---

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Getting Started](#getting-started)
- [Development Workflow](#development-workflow)
- [Commit Convention](#commit-convention)
- [Pull Request Process](#pull-request-process)
- [Style Guide](#style-guide)
- [Reporting Bugs](#reporting-bugs)
- [Suggesting Features](#suggesting-features)

---

## 🤝 Code of Conduct

This project follows a simple rule: **be kind and respectful**.  
Any form of harassment, discrimination, or toxic behaviour will not be tolerated.

---

## 🛠️ How Can I Contribute?

There are many ways to contribute beyond writing code:

- 🐛 **Report bugs** via [GitHub Issues](../../issues/new?template=bug_report.md)
- 💡 **Suggest features** via [GitHub Issues](../../issues/new?template=feature_request.md)
- 📝 **Improve documentation** — fix typos, clarify instructions
- 🎨 **Improve design** — accessibility, responsiveness, animations
- ⚡ **Improve performance** — faster animations, better loading
- ✅ **Review pull requests** from other contributors

---

## 🚀 Getting Started

### Prerequisites

No build tools required. You only need:

- A modern web browser (Chrome 90+, Firefox 88+, Safari 14+)
- A code editor (VS Code recommended)
- Git

### Fork & Clone

```bash
# 1. Fork the repository (click "Fork" on GitHub)

# 2. Clone your fork
git clone https://github.com/YOUR-USERNAME/Moe-Kyaw-Aung-portfolio-V5.git

# 3. Navigate to the project
cd Moe-Kyaw-Aung-portfolio-V5

# 4. Open the file in your browser
open moe-kyaw-aung-portfolio-v5.html
```

### Set Up Upstream

```bash
# Add the original repo as upstream
git remote add upstream https://github.com/Dev-moe-kyawaung/Moe-Kyaw-Aung-portfolio-V5.git

# Verify remotes
git remote -v
```

---

## 🔄 Development Workflow

```bash
# 1. Sync your fork with upstream
git fetch upstream
git checkout main
git merge upstream/main

# 2. Create a feature branch
git checkout -b feature/your-feature-name
# or for bug fixes:
git checkout -b fix/short-description

# 3. Make your changes
# Edit moe-kyaw-aung-portfolio-v5.html (and other files as needed)

# 4. Test in multiple browsers
# Chrome, Firefox, Safari, Edge — mobile and desktop

# 5. Commit your changes
git add .
git commit -m "feat: add your feature description"

# 6. Push to your fork
git push origin feature/your-feature-name

# 7. Open a Pull Request on GitHub
```

---

## 💬 Commit Convention

This project uses [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <short description>

[optional body]

[optional footer]
```

### Types

| Type | When to use |
|---|---|
| `feat` | A new feature or section |
| `fix` | A bug fix |
| `docs` | Documentation changes only |
| `style` | CSS/formatting changes (no logic change) |
| `refactor` | Code restructuring (no feature/bug change) |
| `perf` | Performance improvements |
| `a11y` | Accessibility improvements |
| `chore` | Build process, CI, dependency updates |

### Examples

```bash
git commit -m "feat: add PWA service worker support"
git commit -m "fix: lightbox keyboard navigation on mobile"
git commit -m "docs: update customization guide in docs/"
git commit -m "style: improve skill bar animation timing"
git commit -m "a11y: add aria-labels to social link buttons"
git commit -m "perf: lazy load certificate images with loading=lazy"
```

---

## 🔀 Pull Request Process

1. **Branch** from `main` with a descriptive name
2. **Test** your changes across Chrome, Firefox, and mobile
3. **Follow** the PR template (it will appear automatically)
4. **Link** any related issues using `Closes #123` in the PR body
5. **One concern per PR** — keep PRs focused and small
6. **Wait** for review — feedback will come within 48–72 hours

### PR Checklist

- [ ] Tested in Chrome, Firefox, Safari (desktop)
- [ ] Tested on mobile viewport (375px width minimum)
- [ ] Dark mode works correctly
- [ ] Accessibility: keyboard navigation still works
- [ ] No console errors
- [ ] HTML is valid (use [validator.w3.org](https://validator.w3.org/))
- [ ] CSS custom properties used (no hardcoded colors)
- [ ] Code is commented for complex logic

---

## 🎨 Style Guide

### HTML
- Use semantic HTML5 elements (`<section>`, `<article>`, `<nav>`, `<aside>`)
- Every image must have a descriptive `alt` attribute
- Use `aria-label` on icon-only buttons
- 2-space indentation

### CSS
- Always use CSS custom properties (`var(--primary)`) — never hardcode colors
- Follow the existing BEM-lite class naming (e.g. `.gc`, `.sec-title`, `.btn-p`)
- Mobile-first is preferred for new sections
- Comment non-obvious styles

### JavaScript
- ES6+ syntax (const, let, arrow functions, template literals)
- No external libraries — keep it vanilla
- Use `IntersectionObserver` instead of scroll event listeners where possible
- Comment complex logic blocks

---

## 🐛 Reporting Bugs

Use the [Bug Report template](../../issues/new?template=bug_report.md).

Please include:
- Browser and version
- Device type (desktop/tablet/mobile)
- OS and version
- Steps to reproduce
- Expected vs actual behaviour
- Screenshot or screen recording (if possible)

---

## 💡 Suggesting Features

Use the [Feature Request template](../../issues/new?template=feature_request.md).

Good feature requests include:
- Clear problem statement ("I want to be able to...")
- Proposed solution (even rough is fine)
- Why it benefits users of this portfolio

---

## ❓ Questions?

If you have questions that are not bugs or features, open a [Discussion](../../discussions) instead of an issue.

You can also reach the author directly:
- 📧 moekyawaung@fastmail.com
- 💼 [LinkedIn](https://www.linkedin.com/in/moe-kyaw-aung-2653093a1)

---

*Thank you for contributing! Your help makes this project better for everyone.* 🙏
