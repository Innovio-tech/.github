# Security policy

This policy covers every repository of the Innovio-tech organisation unless a repository has
its own `SECURITY.md`.

## Reporting a vulnerability

**Do not open a GitHub issue, discussion or pull request for a vulnerability.**

Report it privately to the Innovio engineering team through GitHub's private vulnerability
reporting (the repository's **Security** tab → **Report a vulnerability**) where it is enabled,
or through the company's approved private channel. Include, where you can:

- the product and component, version, commit or image tag, and environment;
- a description, steps to reproduce, and the impact you expect;
- logs or screenshots **with secrets and personal data removed**;
- a suggested fix, if you have one.

We confirm receipt, assess the impact, fix it in private, release the fix, rotate any exposed
credential, and only then disclose, unless disclosure is agreed earlier.

## Supported versions

Security fixes go to the version running in production. Development branches and unreleased
builds are not supported versions.

## Never share

Passwords, tokens, API keys, private keys, database credentials, production secrets, personal
data or production customer data, in any issue, pull request, log, screenshot or document. A
secret that was exposed is compromised: rotate it first; deleting it in a later commit is not
enough.

## Personal data breaches

A breach of personal data is reported to the supervisory authority within 72 hours of
becoming aware of it (Moldova Law 195/2024; GDPR where it applies), following the product's
incident runbook.

## Baseline

The security rules every product follows are in
[engineering-standards/standards/security.md](https://github.com/Innovio-tech/engineering-standards/blob/main/standards/security.md);
each product's own controls and targets are in its `docs/security/`.
