# Security Policy

## Reporting vulnerabilities

If you discover a security vulnerability, contact the Triadcoder team privately.

Do not create public issues for security vulnerabilities.

---

## Security best practices

- Never commit secrets
- Never commit `.env` files
- Use environment variables
- Enable 2FA on GitHub accounts
- Keep dependencies updated
- Review Pull Requests carefully
- Use strong passwords
- Keep local environments secure

---

## Access control

- Repository access should follow least privilege principles
- Sensitive repositories should remain private
- Only organization owners can manage critical permissions

---

## Dependency management

- Keep dependencies updated regularly
- Remove unused packages
- Review package vulnerabilities before upgrades

---

## Pull Request review

Before merging:

- Review code carefully
- Check for exposed credentials
- Validate environment variable usage
- Verify sensitive data is not committed
- Confirm no debug code remains

---

## Sensitive files

The following files should never be committed:

```text
.env
.env.*
*.pem
*.key
credentials.json
auth.json
```

---

## Recommended practices

- Use branch protection rules
- Use Pull Requests for all changes
- Avoid direct commits to `main`
- Use least privilege permissions
- Enable GitHub security alerts