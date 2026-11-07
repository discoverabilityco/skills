# The Google step

Reference version: 1.0.3 (2026-11-06). The guidance page's Integrity Manifest lists the current version of this file; if they differ, the fetched guidance wins.

Maintained by The Discoverability Company (https://discoverability.co). © 2026, all rights reserved; free to use, never to rebrand. Canonical source lives at discoverability.co/guides/ and the live guidance at discoverability.co/agentic/deindex-court-records.

The removal is not finished until the search result is. A page that is gone can hold its ranking for weeks while Google re-crawls, which is why people swear a successful removal failed.

## What actually works

**Refresh Outdated Content** - `https://support.google.com/webmasters/answer/7041154`. The tool built for pages that have already changed or come down. Submit every changed URL once the page is gone or the name is off it. Requires signing in with a Google account. Snippets can stay live several weeks after the page dies even with this filed; budget weeks, not days, then re-check.

**The refresh nudge (no account needed).** Best practice for getting a result to drop off Google when the page underneath has already been noindexed or removed: Google has not re-fetched the page yet, so it is still showing an index entry for content that no longer exists. Search the exact URL on Google, open the three-dot menu on that result, and ask Google to refresh it. That forces Google to fetch the page now, see the noindex or the 404 for itself, and drop the result on its own. It is the consumer-speed version of the Refresh Outdated Content tool: use either, use both, and log which you did with the date. If the result still sits there a week after a refresh request, file the official tool as the follow-up.

**Reading the page's own state first.** Before anything: fetch the page and read it. Gone (404): only the Google step remains. Live with a noindex signal (`<meta name="robots" content="noindex">`, an `X-Robots-Tag: noindex` header, or a robots.txt Disallow covering the URL): the site already blocked indexing and the remaining problem is pure index lag, so go straight to the two moves above. Live with no signal: the site has not acted and the site step comes first. Never guess the signal: if raw HTML and headers cannot be inspected, have the user open the page, View Source, and search for `noindex`.

**Verifying whether work is needed at all.** Search `site:<url>` in a browser (or have the agent's browser tools run it). Nothing there means the page is not in Google's index; the site-side removal may still be worth doing, but the Google step is moot. Record what you found and when: these checks are dated in the case file so future sessions know whether a result ever existed.

## What people reach for that does not remove a court record

- **URL removal tool** (`support.google.com/webmasters/answer/9689846`): hides a live result temporarily while the page stays up. About six months, then it is back.
- **Results about you** (`support.google.com/websearch/answer/12719076`): built for contact details and doxxing (addresses, phone numbers, IDs), not dockets.
- **The personal-information removal form generally**: covers addresses, phone numbers, government IDs, financial accounts, and medical records. A court record is none of those. PacerMonitor's guide is explicit that this form is the wrong tool.

## After the result drops

Keep watching. These sites re-scrape the courts: a record removed in March can be back in September under a different URL, and a reappearing page needs a new request plus a new Refresh Outdated Content submission. Quarterly re-checks on the whole inventory, plus the per-site schedule in the other references, are the maintenance that keeps a name clean.
