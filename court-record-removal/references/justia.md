# Justia

Facts verified live 2026-09-08. Source guide: https://discoverability.co/guides/how-to-remove-your-record-from-justia/

**Route:** form at `https://support.justia.com`, category for blocking a Justia link from search engines (it names court dockets, judicial opinions, trademarks and patents; that is how you know it is the right one). Free, four fields, no ID, no case number, no lawyer.

**Eligibility:** the person named on the pages.

**What you need:** every Justia URL ranking on the user's name. Search the full name in quotes, then name plus case caption; copy whole links, never case numbers.

**Steps (~15 minutes):**
1. Show the user the trade first: Justia's block list is a public file, so if the user's full name sits inside the URL being blocked, that name becomes visible in `robots.txt` (a docket means `https://dockets.justia.com/robots.txt`). Decide before filing.
2. Fill the form: paste every URL, one per line, into the links field. In the required Comments box: the pages carry the user's name and they are requesting the search engine block. Name and email, then Send Request. No fee, no paid expedite.
3. Send once. Silence is a normal outcome and is not a cue to resend.

**What to expect:** a search-engine block on the page, not deletion. Their policy says so in writing: the page keeps its address, anyone holding the link still reaches it. No response time is published, and Justia states it cannot control how long links take to leave the search engines after the block goes on.

**Gotchas:**
- Verify rather than assume: an empty robots.txt file is not proof of failure, and a block that went on once can come off later. Re-check the URL and the name search at a few weeks and a few months.
- Deletion is a courthouse product: Justia itself points to contacting the court or hiring an attorney to petition to seal. An expungement order does not automatically bind Justia; send it once obtained, then verify.
- If the court will not seal it, no legal lever is left: the work shifts to suppression (what ranks above it).
- No FCRA dispute here; that letter belongs to a background-check company selling a report.
- If CourtListener, UniCourt, or the court's own portal outrank Justia on the user's name, blocking Justia alone moves nothing anyone will notice. Work the whole first page, not one result.
