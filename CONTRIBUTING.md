# Contributing

## Sumary

- [Development Workflow](#development-workflow-guidelines)
- [Pull Request Guidelines](#pull-request-guidelines)
- [Migration Guidelines](#migration-guidelines)
- [Code Standards](#code-standards)
- [Recommended Labels](#recommended-labels)


## Development Workflow Guidelines

This project follows the **GitHub Flow** workflow, a lightweight branching strategy focused on continuous integration and Pull Requests.

> Always use English for technical naming, branch names, commits, variables, and documentation.

---

### Workflow Overview

1. Update your local `main` branch
2. Create a new branch
3. Push the branch to the remote repository
4. Make changes and create commits
5. Synchronize your branch with `main`
6. Open a Pull Request
7. Wait for review and approval
8. Merge the Pull Request
9. Remove merged branches

---

### 1. Update your local `main` branch

Before starting a new feature or fix, update your local `main` branch:

```bash
git checkout main
git pull origin main
```

---

### 2. Create a new branch

Create a descriptive branch from `main`:

```bash
git checkout -b feature/short-description
```

#### Branch naming conventions

```text
feature/short-description
fix/short-description
docs/short-description
refactor/short-description
test/short-description
chore/short-description
```
---

### 3. Push the branch to the remote repository

```bash
git push -u origin feature/short-description
```

---

### 4. Make changes and create commits

Use clear and standardized commit messages.

#### Commit pattern

```text
:emoji: type: short description
```

#### Examples

```bash
git commit -m ":tada: initial commit"
```

```bash
git commit -m ":sparkles: feat: add authentication routes" -m "Add login, logout and session validation routes"
```

```bash
git commit -m ":bug: fix: resolve login validation issue"
```

```bash
git commit -m ":recycle: refactor: improve authentication middleware"
```

```bash
git commit -m ":test_tube: test: add authentication tests"
```

```bash
git commit -m ":books: docs: update installation instructions"
```

```bash
git commit -m ":art: style: improve code formatting"
```

### 5. After committing your changes, push them to the remote repository:

```bash
git push
```

---

### 6. Synchronize your branch with `main`

Before opening a Pull Request, synchronize your branch with the latest `main` updates:

```bash
git checkout main
git pull origin main

git checkout your-branch-name
git merge main
```

Resolve any merge conflicts before continuing.

---

### 7. Open a Pull Request

When your changes are ready:

1. Open a Pull Request
2. Add a clear description
3. Link related issues if applicable
4. Wait for review
5. Make requested adjustments if necessary
6. Ensure tests are passing
7. Merge through GitHub after approval

> Pull Requests should be merged only after review and approval.

---

### 8. Update your local `main` branch

After the Pull Request is merged:

```bash
git checkout main
git pull origin main
```

---

### 9. Remove merged branches

After merging, remove the local branch to keep the repository clean:

```bash
git branch -d your-branch-name
```

Optionally, remove the remote branch as well:

```bash
git push origin --delete your-branch-name
```

---

## Pull Request Guidelines

- Always create a Pull Request
- Keep Pull Requests small and focused
- Write clear descriptions
- Link related issues whenever possible
- Resolve conflicts before requesting review
- Avoid mixing unrelated changes in the same Pull Request

---

## Migration Guidelines

- Never edit old migrations after they have been shared
- Create a new migration for every database change
- Keep migrations atomic and descriptive

### Examples of valid migrations

- Table creation
- Column addition
- Field updates
- Relationship changes

---

## Code Standards

- Write clean and readable code
- Avoid duplicated logic
- Follow the project architecture
- Use meaningful naming
- Keep methods and classes focused
- Never commit secrets or `.env` files
- Use English for technical naming

---

## Recommended Labels

Each issue should ideally contain:

- one type label
- one area label
- one priority label

### Examples

```text
bug + backend + priority:high
```

```text
enhancement + frontend + priority:medium
```

```text
refactor + infra + priority:low
```