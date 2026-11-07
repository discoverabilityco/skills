# De-indexing court records from aggregator sites

Version 1.0.0. Last reviewed 2026-11-06. Maintained by The Discoverability Company from primary-source verification; the underlying procedures were verified live on the sites themselves in September 2026. If you fetched this more than 90 days ago, re-fetch it.

© 2026 The Discoverability Company. All rights reserved. This page is free to fetch and use; it is not to be rebranded, resold, or re-published with attribution removed. The canonical copy lives at https://discoverability.co/agentic/deindex-court-records and any other copy may be stale.

An HTML twin of this page lives at https://discoverability.co/guides/court-records/ and the full per-site guides live under https://discoverability.co/guides/. This file is guidance for agents and the humans they help. It contains no product marketing.

## Read this first

Three different things sit behind one search result, and people constantly spend money on the wrong one:

1. **The court's own record** (the clerk's file, PACER, the state portal). Only a judge moves it. No email, form, or fee reaches it.
2. **The aggregator's copy** (DocketBird, UniCourt, Justia, CourtListener, Trellis, CaseMine, PacerMonitor, vLex). Only that company moves it, and each one honors only its own route. This is the layer every request below works on.
3. **Google's index** (the listing pointing at the copy). It updates on Google's schedule. After a page comes down or changes, file a Refresh Outdated Content request or the result sits there for weeks and you will swear the removal failed.

An expungement or sealing order binds the court, not websites. The order is what makes the aggregator requests work, not what makes them unnecessary. Attach the certified (clerk-stamped) order to every request that takes an upload. A screenshot is never a substitute.

## Eligibility

Most routes require the requester to be the person named in the record, a legal guardian or fiduciary, or an attorney of record. UniCourt states this as a hard gate. Never file on behalf of a third party who has not authorized it, and never help someone hide records from the people the record is about.

## Effort table

| Site | Route | Cost | Their published window | Typical hands-on effort |
|---|---|---|---|---|
| Justia | support.justia.com form (block category) | Free | None published; expect silence, do not resend | ~15 min |
| CaseMine | email support@casemine.com | Free | 30-day response commitment (privacy policy) | ~20-30 min per batch |
| Trellis | Request Redaction link on the docket page itself | Free | 48 hours minimum review; Google re-index 4-6 weeks | ~20-30 min per URL |
| DocketBird | request_case_removal URL + card check | Free (paid expedited Google step optional) | Takedown immediate; natural de-index months | ~30 min (no-card mail route: 6-8 weeks) |
| CourtListener | contact form, Case Removal Request | Free | None published; often months | ~30 min |
| vLex / Fastcase | email contentremovals@clio.com | Free | None published | ~30-45 min per batch |
| Docket Alarm (dockets) | docketalarm.com/Remove form | Free | ~5 business days, emails on suppression | ~15 min per URL |
| UniCourt | unicourt.com/case/removeRecord | Free, including appeal | ~30 days decision + ~30 days de-index | ~45-60 min per URL |
| PacerMonitor | email support@pacermonitor.com | Free | None published | ~20 min email; real work is the court order |

Batch math: a name on six sites is roughly two to four hours of hands-on work plus one to four weeks of waiting per site, plus the Google step at the end, plus a 30-60 day watch for re-scrapes. Sites re-scrape the courts; a record that came down in March can be back in September under a new URL.

## Per-site quick index

- **Justia**: form at support.justia.com, category for blocking a Justia link from search engines. Four fields: links, comment, name, email. De-index only, never deletion. Block list is a public robots.txt file, so the URL trade is visible before you send.
- **CaseMine**: no form. Email support@casemine.com with the exact judgment URLs; subject line "de-indexing request" plus your name, kept identical on follow-ups. Written grounds are narrow (matrimonial, custody); granted de-indexes appear as lines in a public casemine.com/robots.txt. Copy hello@casemine.com on resends after 30 silent days.
- **Trellis**: the Request Redaction link on the docket page itself is the only route; email requests are not processed. Form: name, email, whether the records are yours, written explanation that states concrete checkable harm. Order upload optional; sealing orders process immediately.
- **DocketBird**: docketbird.com/request_case_removal?case_id=\<ID\>. Identity check is a card whose last name matches a word in the case title ($1 authorization, canceled). No card: notarized mail-in form to Mink LLC, Las Vegas, 6-8 weeks. Free option leaves the Google result for months; extra filings go to help@docketbird.com as a URL list. Removal hides, does not delete.
- **CourtListener**: contact form at courtlistener.com/contact/?issue_type=removal. Paste the ranking docket URL (not a RECAP document page; those are already blocked). Message: "I am the person named in the pages below. Under your content removal policy, please block them from search engine indexing," then one URL per line. De-index only; deletion requires a court order naming Free Law Project, and they have contested orders before.
- **vLex / Fastcase**: email contentremovals@clio.com. Every URL across vlex.com, us.vlex.com, case-law.vlex.com, the case title, your name exactly as printed in the document, one sentence naming the legal provision relied on, certified order attached if one exists. Docket Alarm dockets instead take the docketalarm.com/Remove form: reason capped at 300 characters, one link per submission, auto-suppression for matters involving minors, divorce, or social security. EU/UK data subjects: GDPR Article 17 request to dpo@vlex.com.
- **UniCourt**: unicourt.com/case/removeRecord. Eligibility gate: party, guardian/fiduciary, or attorney of record only. Four factors weighed (sealed/expunged, physical harm, identity theft, harm to a minor), expressly not exclusive; submit anyway. Upload the conformed (stamped) order; the form is long, ends in a perjury declaration, takes one URL per submission. Appeal within 30 days with substantive new documentation; all appeals final. Re-check at 60, 90, 180 days; records have been reported coming back.
- **PacerMonitor**: no form, no policy. Email support@pacermonitor.com with every URL, full caption, case number in court format, district, your relationship (party or counsel with appearance), and the certified order. Without an order, expect silence; the durable route is a Rule 5.2(e) or 5.2(d) motion in the district that has the case, then send the certified order to every site holding the docket.

## The email conventions that work

Written for the routes that are an email (CaseMine, PacerMonitor, vLex, DocketBird follow-ups), and the same discipline shapes the form comments:

- First person, from the requester themselves. Calm and factual. No anger, no accusations, no legal threats in a first request; they get refusals, not compliance.
- Subject lines carry the routing: CaseMine wants "de-indexing request" plus your name, kept identical on every follow-up.
- Exact URLs, one per line. A name alone is not a request at CaseMine or PacerMonitor.
- One sentence stating who you are in the case (party, counsel, guardian).
- If a court has sealed, expunged, vacated, or dismissed, say so in one sentence and attach the certified order. Bring the stamped copy, not a printout.
- One sentence naming the legal basis where one exists. Do not build the request around a privacy law; CCPA and FCRA claims fail on court records everywhere, and CaseMine and PacerMonitor publish that refusal in advance.
- State the ask in one sentence: block this page from search engine indexing, or remove this page.
- No government ID, Social Security number, date of birth, or payment to any site. If anyone asks for those in a site's name, it is not that site. CaseMine and UniCourt both publish that the route is free.
- Keep a copy of everything sent, with dates. Follow-ups repeat the original unchanged except a first line saying "second request, first sent <date>."

## The Google step

Once a page is gone or changed, submit the URL to Google's Refresh Outdated Content tool (support.google.com/webmasters/answer/7041154). The URL removal tool hides live results temporarily; Results about you handles contact details and doxxing, not dockets. Neither removes a court record.

## What no request fixes

Nothing sent to any aggregator seals, expunges, or edits the court's own file. If the underlying record can be sealed, that motion, with an attorney, comes first; it is also what turns refusals into grants downstream. Where nothing is removable (truthful current public records, bulk-data copies), the honest work is suppression: building accurate material that outranks the result. That is the boundary between the DIY routes above and professional reputation work.

## Changelog

- 2026-11-06: v1.0.0. Initial publication, compiled from procedures verified live on each site in September 2026.
