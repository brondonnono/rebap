# Contribution Guide

## Branches

| Branch         | Purpose                   |
| -------------- | ------------------------- |
| `main`         | Production — stable       |
| `dev`          | Development — integration |
| `feature/name` | New feature               |
| `fix/name`     | Bug fix                   |

**Never commit directly to `main`.**

## Workflow

```bash
# Create a branch from dev
git checkout dev
git checkout -b feature/my-feature

# ... code ...

# Commit changes
git add .
git commit -m "feat: add upload page"

# Merge into dev
git checkout dev
git merge feature/my-feature
```

## Commit Convention

Format: `type: short lowercase description`

| Type       | When to Use                            |
| ---------- | -------------------------------------- |
| `feat`     | New feature                            |
| `fix`      | Bug fix                                |
| `style`    | CSS/design changes only                |
| `refactor` | Code rewrite without changing behavior |
| `docs`     | Documentation only                     |
| `chore`    | Configuration, dependencies, tooling   |

### Examples

```bash
git commit -m "feat: add pdf upload"
git commit -m "fix: resolve gemini json parsing issue"
git commit -m "style: adjust header colors"
git commit -m "docs: update readme"
git commit -m "chore: install framer-motion"
```
