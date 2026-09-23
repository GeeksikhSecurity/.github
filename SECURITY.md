# Security Policy

This is the default security policy for public, open-source repositories maintained under the **GeeksikhSecurity** GitHub organization by Gurvinder Singh (SecurityLeader.ai / Sayva Consulting). It applies to any repository in this organization that does not publish its own `SECURITY.md`, which would take precedence over this one.

This policy is published voluntarily, in line with the [EU Cyber Resilience Act (CRA) guidance for open source maintainers](https://best.openssf.org/CRA-Brief-Guide-for-OSS-Developers). See the disclaimer at the bottom.

## 1. Secure Development Practices

- Changes to `main`/default branches go through pull request review before merge; branch protection is enabled on actively maintained repositories.
- Dependencies are tracked via each repository's manifest (e.g. `package.json`, `requirements.txt`, `pyproject.toml`) and updated on a best-effort basis as vulnerabilities are disclosed upstream.
- Secrets and credentials are never committed; repositories use environment variables and secret managers for any required configuration.
- Where applicable, static analysis and dependency scanning are run before release.

## 2. How Project Risk Is Handled

Each repository is maintained on a best-effort, volunteer basis. Risk is assessed by the maintainer at triage time based on: exploitability, whether the affected code path is reachable by default configuration, and whether the project is under active maintenance. There is no formal SLA; see Section 5 for support expectations.

## 3. Reporting a Vulnerability

**Preferred channel:** [GitHub Security Advisories](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing/privately-reporting-a-security-vulnerability) — open a private security advisory directly on the affected repository ("Security" tab → "Report a vulnerability"). This keeps the report private until a fix is coordinated.

**Alternate contact:** security@geeksikh.com

Please do **not** open a public GitHub issue for a suspected security vulnerability. Public bug reports should go through the process in `CONTRIBUTING.md` instead (see the distinction there).

When reporting, please include: affected repository and version/commit, a description of the issue, and steps to reproduce if available.

## 4. Vulnerability Handling Process

1. **Acknowledge** — best-effort acknowledgment of a received report (target: within 5 business days).
2. **Triage** — assess severity and reproducibility.
3. **Remediate** — develop and test a fix on a private branch where coordinated disclosure is warranted.
4. **Patch & release** — publish a fixed version/tag and a corresponding entry in the repository's release notes or `CHANGELOG.md`.
5. **Disclose** — coordinated public disclosure once a fix is available, with credit to the reporter unless anonymity is requested.

## 5. Supported Versions / End-of-Life

Unless a repository states otherwise in its own documentation, only the latest release/`main` branch is supported. There is no guaranteed support window or end-of-life date — this reflects the volunteer, non-commercial nature of these projects. If a repository is archived or no longer maintained, this will be noted in its README.

## Voluntary Practice — Not a Regulatory Status

*This project voluntarily documents its security practices. This information is provided "as is," without warranties or guarantees. See the project's license for more details.*

*The maintainers and contributors:*
- *have no obligations under the EU CRA,*
- *are not Manufacturers, Importers, or Economic Operators,*
- *assume no financial, contractual, or legal liability,*
- *and do not provide CRA compliance assurances.*

*Anyone incorporating this software into commercial products remains solely responsible for such products, including regulatory compliance, risk assessment, and vulnerability management.*
