# Contributing to AI NutriScan

Thank you for your interest in contributing! We welcome contributions of all kinds — bug fixes, new features, documentation improvements, and more.

---

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [Development Workflow](#development-workflow)
- [Branching Strategy](#branching-strategy)
- [Commit Messages](#commit-messages)
- [Pull Request Guidelines](#pull-request-guidelines)
- [Reporting Bugs](#reporting-bugs)
- [Suggesting Features](#suggesting-features)

---

## Code of Conduct

Be respectful, inclusive, and constructive. We will not tolerate harassment of any kind. By participating, you agree to treat all contributors with professionalism and kindness.

---

## Getting Started

### Prerequisites

- Node.js v18 or higher
- npm v9 or higher (or pnpm v9+)
- Git

### Local Setup

```bash
# 1. Fork the repository on GitHub

# 2. Clone your fork
git clone https://github.com/<your-username>/ainutriscan.git
cd ainutriscan

# 3. Install dependencies
npm install

# 4. Set up environment variables
cp .env.example .env
# Edit .env with your local values

# 5. Start the development server
npm run dev
```

---

## Development Workflow

1. Check existing issues and PRs before starting work to avoid duplication.
2. Create a branch from `main` (see [Branching Strategy](#branching-strategy)).
3. Make your changes with clear, focused commits.
4. Run `npm run lint` and `npm run typecheck` before pushing.
5. Open a Pull Request against `main`.

---

## Branching Strategy

| Branch pattern | Purpose |
|----------------|---------|
| `feat/<name>` | New feature |
| `fix/<name>` | Bug fix |
| `docs/<name>` | Documentation only |
| `refactor/<name>` | Code refactor without behaviour change |
| `chore/<name>` | Tooling, dependencies, CI |

Example: `feat/offline-scan-history`

---

## Commit Messages

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(optional scope): <short description>

[optional body]

[optional footer]
```

**Types:** `feat`, `fix`, `docs`, `refactor`, `test`, `chore`, `perf`, `ci`

Examples:
```
feat(scanner): add multi-dish detection support
fix(auth): resolve token refresh race condition
docs: update API reference for /v1/scan endpoint
```

---

## Pull Request Guidelines

- Keep PRs focused — one feature or fix per PR.
- Fill out the PR template completely.
- Link to the relevant issue (e.g. `Closes #42`).
- Ensure all checks pass before requesting review.
- Add screenshots or screen recordings for UI changes.
- Be responsive to review feedback within a reasonable timeframe.

---

## Reporting Bugs

Please use [GitHub Issues](https://github.com/ainutriscan/ainutriscan/issues) and include:

- A clear, descriptive title
- Steps to reproduce the issue
- Expected vs actual behaviour
- Screenshots or logs if relevant
- Your environment (OS, Node version, app version)

For security vulnerabilities, do **not** open a public issue — see [SECURITY.md](SECURITY.md).

---

## Suggesting Features

Open a [GitHub Issue](https://github.com/ainutriscan/ainutriscan/issues) with the label `enhancement` and describe:

- The problem you are trying to solve
- Your proposed solution
- Any alternatives you considered
- Why this would benefit other users

---

Thank you for helping make AI NutriScan better for everyone. 🌿
