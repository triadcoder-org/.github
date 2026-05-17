# Contributing Guidelines

## Development workflow

The organization follows the GitHub Flow workflow.

---

## Branch naming

Use descriptive branch names.

### Patterns

```text
feature/short-description
fix/short-description
docs/short-description
refactor/short-description
test/short-description
chore/short-description
```

---

## Commit conventions

Use clear and standardized commits.

### Pattern

```text
:emoji: type: short description
```

### Examples

```bash
git commit -m ":sparkles: feat: add authentication routes"
```

```bash
git commit -m ":bug: fix: resolve login validation"
```

```bash
git commit -m ":recycle: refactor: improve auth middleware"
```

```bash
git commit -m ":books: docs: update installation instructions"
```

---

## Pull Requests

- Always open a Pull Request
- Keep Pull Requests small and focused
- Link related issues whenever possible
- Wait for review before merging
- Resolve conflicts before requesting review

---

## Migrations

- Never edit old migrations after sharing them
- Create a new migration for each database change
- Keep migrations atomic and descriptive

---

## Code standards

- Write clean and readable code
- Avoid duplicated logic
- Follow project architecture
- Never commit secrets or .env files
- Use English for technical naming

---

## Recommended labels

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