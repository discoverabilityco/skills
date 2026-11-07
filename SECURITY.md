# Security Policy

## Scope

This repository ships agent skills: markdown instructions and reference files. By design they contain:

- no executable code,
- no network calls except one plain-text fetch of static guidance from `https://discoverability.co/agentic/...`,
- no telemetry,
- no collection, transmission, or storage of personal data outside the user's own machine.

## Reporting

Report suspected vulnerabilities, malicious drift, or guidance-page tampering to **team@discoverability.co** with the subject line `[skills-security]`. We aim to acknowledge within 2 business days and remediate guidance drift within 48 hours of confirmation.

## Verification

The skills' only remote dependency is the guidance page. If you want to verify what it serves, it is plain markdown with a version and last-reviewed date at the top; compare it against the copy in this repository under `kb/`. Discrepancies are security reports.
