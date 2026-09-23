# Contributing

This is the default contributing guide for public repositories under the **GeeksikhSecurity** GitHub organization. An individual repository's own `CONTRIBUTING.md`, if present, takes precedence over this one.

## Before You Start

- Check open issues and pull requests to avoid duplicate work.
- For anything non-trivial, open an issue first to discuss the approach before submitting a PR.

## Secure Development Practices

Contributions are expected to follow the practices in this organization's [SECURITY.md](./SECURITY.md):

- No hardcoded credentials, tokens, or secrets in code, commits, or commit history.
- Prefer environment variables / secret managers for any required configuration.
- New dependencies should be justified in the PR description (what it's for, why it's needed).
- Keep pull requests small and scoped to one concern — this makes review faster and defects easier to isolate.

## Submitting a Pull Request

1. Fork the repository and create a branch from the default branch.
2. Make your change, with tests where the project has a test suite.
3. Open a PR describing **what** changed and **why**.
4. A maintainer will review; expect requested changes before merge on security-relevant code paths.

## Reporting Bugs vs. Reporting Vulnerabilities

These are handled through **different channels** — please use the right one:

- **Non-security bugs, defects, or feature requests** → open a public [GitHub Issue](../../issues) on the affected repository. Include steps to reproduce, expected vs. actual behavior, and environment details.
- **Security vulnerabilities** → do **not** open a public issue. Follow the private reporting process in [SECURITY.md](./SECURITY.md) instead.

## Code of Conduct

Be respectful and constructive. Maintainers may close issues or PRs that are off-topic, abusive, or not aligned with the project's goals.
