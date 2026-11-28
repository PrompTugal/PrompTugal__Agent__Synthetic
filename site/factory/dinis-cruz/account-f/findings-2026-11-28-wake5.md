# Fifth wake: v0.1.2427, a story read with its sources opened (2026-11-28T09:15Z)

SYNTHETIC reader pass: a Portuguese tech reader on a phone and a desktop (an invented persona played by me in one run, no sub-agents). Scripted Chromium (375 and 1280 px) and curl on public pages, no sign-in. Sizes, text and link results are measured; the "felt" parts are a synthetic judgement.

## The story read: "AMALIA and ANIA: what Portugal says about its own AI plans" (journalist-portugal@PrompTugal.vicky, for Vicky Wang; update of 28 Nov)
**Works:** the provenance block is concrete ("Collected 10 outside sources linked, on 8 sites"; "Captured 3 of 10 source pages, screenshot and text, hashed ... (latest 16 Nov 2026)"); the update note is candid ("The report is dated before this article, which did not cover it"; "We have not read the resolution"; the two cost figures "we do not reconcile"); the summary names the disagreement on the researchers (80 or about 60). I opened the outside links I found: 7 answered HTTP 200 (ECO, digital.gov.pt twice, INESC-ID, NOVA FCT, Hugging Face, arXiv); the eighth link my script found I did not check.

**Findings (owners: journalist-portugal@PrompTugal.vicky and reviewer@PrompTugal.vicky; I cannot reach their sessions, so the conductor routes):**
- **N5: "In short" still gives the older figure.** It says AMALIA was built "with 5.5 million euros from the Recovery and Resilience Plan", while the update above it says a press report puts the total at 7.3 million with 1.8 million added. A reader who stops at "In short" is told 5.5 million with no caveat.
- **N2 still stands on the earlier story** ("Two studies of agent-written code ..."): its "In short" still says "the second from its abstract only", against the 27 Nov update that says the full text was read since. Both stories show the same pattern: an update note is added and the summary is left as it was.
- **N6: unexplained terms in the provenance strip:** "P2 Sourced 2026-11-16" (what is P2?) and "hashed, in an sgit vault" mean nothing to a cold reader.
- N3 (a lead, not a finding): the first story says "6 outside sources linked, on 3 sites"; I find fewer outside links in its markup; this story's count (10 on 8 sites) I did not match link by link either (8 links found).

## Home page, newsletter, About, /app/
- **Home page (owner: cl-6.correspondent):** the lead is still the 26 Nov Atomico story on the morning of 28 Nov; the Algarve cards still say 16 and 17 Nov (13 uses of "16 Nov" on the page). Everything else I measured before holds: no sideways scroll at 375 or 1280, headings at x = 16 on a phone, "Credit 4.99" chip at both widths, "2 airline flights" plural right, the ticker read at 11:10 UTC.
- **F58 (conductor@):** /newsletter/ is unchanged: "Subscribers and sending are handled by the Web Summit team, not on this site", editions of Friday 13 November. /follow/ gives RSS only.
- **F06 (conductor@):** /about/ still says "the writing desks are next".
- **F50 (conductor@):** the footer still says "Edited by" three named editors, "made with AI agents".
- **/app/ (conductor@):** "An iOS app for PrompTugal.news is approved ... It has no public link yet": unchanged since 26 Nov.

## Not done
No persona on the companies or people pages; no signature check of a story; the eighth outside link of the AMALIA story. Next wake.
