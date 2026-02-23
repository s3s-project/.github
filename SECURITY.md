# Security Policy

All repositories under <https://github.com/s3s-project> take security seriously.

This document describes how to report security vulnerabilities, and which reporting channel to choose based on severity.

## Reporting a Vulnerability

You may use any of the following methods. If you start with a public report and later realize the issue is more severe or contains sensitive details, **stop sharing details publicly** and escalate to a private channel (email or a draft security advisory).

### 1. Public GitHub Issue (low severity / non-sensitive)

Use this option when **public discussion is safe**, for example:

- Documentation or configuration hardening suggestions
- Minor information leaks without real-world impact
- Issues that do **not** include exploit details, credentials, tokens, private keys, or user data

Create an issue in the **affected repository** and include the details in “What to include”.

**If you are unsure about the severity, ALWAYS default to a private channel.** If at any point you need to share proof-of-concept code, exploit details, or sensitive data, switch to a private channel.

### 2. Email Maintainers (medium severity / needs limited privacy)

Use this option when the report should **not** be fully public, but you cannot (or prefer not to) use GitHub Security Advisories.

- Send an email to the maintainers of the affected repository.
- If you cannot find a maintainer email in the repository metadata (README, website, package/crate metadata, etc.), please use method 3 instead.

### 3. GitHub Security Advisory (high/critical severity / private)

Use this option for **high-impact vulnerabilities** or anything that may be exploited:

- Remote code execution (RCE), command injection
- Authentication/authorization bypass
- Sensitive data exposure (secrets, credentials, user data)
- Supply-chain risks (malicious artifacts, dependency confusion, etc.)
- Reports with proof-of-concept exploits

In the affected repository, open a **draft security advisory** and discuss it privately:

- Go to the repository’s **Security** tab
- Choose **Advisories** → **Report a vulnerability**
- Create a draft advisory and share details there

If the repository does not have Security Advisories enabled, fall back to method 2.

## What to Include

To help us triage quickly, please include:

- A clear description of the vulnerability and its security impact
- Affected repository and affected component/module
- Affected versions/branches and the environment (OS, architecture, config)
- Reproduction steps or a minimal proof-of-concept (only via private channels for medium+ severity)
- Any relevant logs, stack traces, or screenshots (redact sensitive data)
- Suggested mitigations or patches (optional)

## Coordinated Disclosure

We aim to:

- Acknowledge receipt within a reasonable timeframe
- Work with you on impact assessment, fixes, and release planning
- Credit reporters where appropriate (if you want)

Please avoid disclosing high/critical vulnerabilities publicly until a fix is available.
