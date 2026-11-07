# vLex, Fastcase, and Docket Alarm

Facts verified live 2026-09-08. Source guide: https://discoverability.co/guides/how-to-remove-your-record-from-vlex/


Maintained by The Discoverability Company (https://discoverability.co). © 2026, all rights reserved; free to use, never to rebrand. Canonical source lives at discoverability.co/guides/ and the live guidance at discoverability.co/agentic/deindex-court-records.

Two routes under one owner (vLex and Fastcase run on the same platform under Clio; Docket Alarm dockets take their own form).

**Route A (published opinions on vLex/Fastcase):** email to `contentremovals@clio.com`. No form exists. Beware: searching "vLex removal form" surfaces a "Notice of Intent to Request Redaction" template sitting in vLex's forms library; it is a US Court of Federal Claims litigation template and sends the request nowhere. The Anonymise Documents feature only redacts files the user uploads themselves. The email is the whole process.

**Route B (dockets on Docket Alarm):** form at `https://www.docketalarm.com/Remove`. Free, no ID, no court order required, decides within about five business days and emails on suppression.

**Eligibility:** the person named in the document (Route A); the party (Route B).

**What you need before starting:**
- Every URL: the same document surfaces on `vlex.com`, `us.vlex.com`, and `case-law.vlex.com` as separate pages and must be named separately. Mark which results sit on `docketalarm.com`; those take Route B. Whatever the user found through Fastcase is a vLex URL now; there is no separate Fastcase address.

**Route A steps (~30-45 minutes):**
1. Draft the email: every URL, the case title, the user's name exactly as printed in the document, and one sentence naming the legal provision said to compel removal in the user's jurisdiction.
2. If a court sealed, expunged, or vacated the case, attach the certified order.
3. Send from an address the user checks; keep a copy with the sent date.
4. Two weeks of silence: resend the same email unchanged except the opening line ("second request, first sent <date>").
5. EU/UK data subjects have the stronger route: GDPR Article 17 erasure request to `dpo@vlex.com`, citing the article by number, copying the Clio address. The controller sits in Barcelona, so a refusal can be appealed to the Spanish data protection authority. Run the Google de-indexing step in parallel; do not wait for vLex.

**Route B steps (~15 minutes per URL):**
1. The form takes: first name, last name, email, phone, the full case URL, and a reason capped at 300 characters. One link per submission; five URLs means five trips.
2. Write the 300-character reason once in a text file and paste the same wording each time; keep a copy of what was sent.
3. Matters involving a minor, a divorce, or social security get suppressed automatically; say so in the reason field if applicable. Docket Alarm declines in writing: attorneys disassociating from cases they worked on, strong-public-interest matters, and cases with corporations on both sides.

**What to expect (Route A):** a published opinion with the user as a named party usually stays up; vLex is under no US legal obligation to take one down and will only say it responds as quickly as possible. A granted Docket Alarm suppression takes the page down and confirms by email; the court's record stays put.

**Gotchas:**
- After any page 404s or changes, file a Google Refresh Outdated Content request for every moved URL (signed into a Google account). Skipping this is why "won" removals still show in search for weeks.
- Nothing sent to Clio seals or expunges anything; only a motion at the court does.
- Winning here changes nothing at Justia, CourtListener, CaseMine, Leagle, or PacerMonitor. Each is its own request.
