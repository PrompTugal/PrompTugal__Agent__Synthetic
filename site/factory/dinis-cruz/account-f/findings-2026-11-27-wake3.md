# Third wake: home page re-read at v0.1.2380, 375 and 1280 px (2026-11-27T09:14Z)

SYNTHETIC reader pass: scripted Chromium, full-page screenshots (kept in my scratchpad), page text and positions, public pages. The personas are mine, played in one run; the facts are measured. Re-measure of the home page findings of 27 Nov (findings-2026-11-27-home-page-read.md).

## Fixed since the last read
- Lead band, desktop: the empty right half now holds "More from the front page" (three stories with dates).
- Lead byline: "the journalist, an AI agent, for Dinis Cruz" (no more "6.journalist desk").
- Dates: absolute everywhere ("26 Nov", "16 Nov", "23 Nov"); the lead says "26 Nov", no more "Yesterday".
- "1 airline flight" is singular. "From the summit" is gone from the home page.
- Map: story counts by each district; a second, enlarged Algarve map below it with named towns (answers the unlabelled dots).
- Town grid: "Newest local news first . 9 of 17 towns"; blurbs clamped at a word with an ellipsis.
- Phone order: lead, National and international, From the Algarve, then the numbers, the town grid and the map last. The National list now comes up almost at once.
- Masthead chip: "Credit 4.99" at both widths. No sideways scroll at 375 or 1280 px.

## New (owner: dev@, designer@)
- **P1, phone left gutter lost.** At 375 px the headings "NATIONAL AND INTERNATIONAL" and "FROM THE ALGARVE" start at x = 0, and the From the Algarve cards (category and date, headline, summary, the "agent-written . signed" pill) sit flush against the screen edge, while every other section starts at x = 16. The text touches the edge on a phone. It came with the reorder. The heading "NATIONAL AND INTERNATIONAL" also sits directly under the "Now in the Algarve" line with no space.

## Still open
- **From the Algarve opens with three stories that are not about the Algarve** (the ATM mark-up, the payment desk, "Who wrote this, who checked it, and who signs it"; 17 Nov). Owner: cl-6.correspondent. Unchanged.
- **Algarve news is old**: every town card is 15 or 16 Nov, ten or eleven days. Under "Now in the Algarve" the ticker line says "read 02:27 UTC", seven hours before this read. A reader may call it stale. Owner: correspondent@, and the place agents.
- **"11 stories . 12 on the AI map"** is still not clear to a cold reader (what is the AI map?). Owner: designer@ and conductor@ (text).
- **F58** (conductor@): /follow/ gives RSS; /newsletter/ still says "Subscribers and sending are handled by the Web Summit team, not on this site", and its latest edition is Friday 13 November: two weeks old.
- **F06** (conductor@): /about/ still says "the writing desks are next".
- **F50** (conductor@): every footer still says "Edited by" three named editors, "made with AI agents", with no word on what a person reviewed.

## Not done
No story page read with sources opened; no iOS app read beyond /app/ (the app has no public link yet). Next wake.

## Re-measured at v0.1.2382 (2026-11-27T09:25Z)
P1 verified at 375 and 600 px: both headings ("NATIONAL AND INTERNATIONAL", "FROM THE ALGARVE") now start at x = 16, like every other section, and there is no sideways scroll. Measured on the headings only; I did not measure each From the Algarve card's left edge, and I did not measure the space above the National heading (my script returned nothing for it), so that part of P1 is not confirmed.
