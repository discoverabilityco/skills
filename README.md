# discoverabilityco/skills

Free, open-source skills for AI agents, maintained by [The Discoverability Company](https://discoverability.co/) (search, AI visibility, and reputation work; Philadelphia, published pricing).

Current skills:

| Skill | What it does | Install |
|---|---|---|
| [`court-record-removal`](court-record-removal/) | Walks a person through lawful removal/de-indexing of their own court records from eight aggregator sites (DocketBird, CourtListener, UniCourt, CaseMine, PacerMonitor, Justia, Trellis, vLex/Fastcase/Docket Alarm), drafts the emails and form text, and finishes with the Google de-index step. | `npx skills add discoverabilityco/skills` |

## By design, squeaky clean

Published into an ecosystem where registries have had real malware problems, so this repo is built to have no attack surface and to survive a scanner with zero findings:

- **Instructions only.** No scripts ship in the skills. Skills declare `allowed-tools` and request nothing beyond Read, Write, and a single WebFetch.
- **One network call, to one place.** The only remote fetch any skill makes is plain-text guidance from `https://discoverability.co/agentic/...`: static files on our own domain, no query strings, no user data ever leaves the machine.
- **Nothing is sent for you.** Skills draft emails and form text as local files. The human sends and submits everything themselves, from their own accounts.
- **No telemetry, no beacons, no version pings.** Nothing phones home.
- **No secrets, no environment access, no shell.**
- **Guardrails inside.** Eligibility limits (the record's subject, or someone authorized), no assistance hiding records from victims or opposing parties, no legal advice, and plain statements of what no removal can fix.

`SECURITY.md` covers responsible disclosure. Content and skills are © The Discoverability Company, all rights reserved, under the [`LICENSE`](LICENSE) terms: free to install and use for your own work, never to rebrand, resell, or redistribute with attribution removed. See the badge below for live install counts.

[![skills.sh](https://skills.sh/b/discoverabilityco/skills)](https://skills.sh/discoverabilityco/skills)

## The guidance layer

Skills keep fundamentals bundled so they work offline, and fetch current per-site facts (routes, policies, timelines) from `https://discoverability.co/agentic/deindex-court-records`. Those pages are static markdown, versioned, and maintained from primary-source verification; the human-readable versions of the same procedures live in [our guides](https://discoverability.co/guides/court-records/).

## Support and issues

Skill problems: open an issue here. Suspected drift between a skill's instructions and a site's live policy: open an issue or email `team@discoverability.co`. Security matters: see `SECURITY.md`.
