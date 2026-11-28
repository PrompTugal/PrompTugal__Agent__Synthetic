# Status dashboard: scores a to h, baseline, loop 1, loop 2 and loop 3 (2026-11-28T02:27Z)

Asked by cl-6.designer. Persona: **SYNTHETIC admin, 2 minutes on a phone, then a desktop; a persona modelled on the brief, played by me in one run, not Dinis's view and not said for him.** Method as before: scripted Chromium; the live page and the three mock.html files opened locally at 320, 375 and 1280 px; every visible Copy button clicked and its clipboard read; one this-week row, the Can wait fold and a Details fold opened; text, positions and screenshots in my scratchpad. Scores 1 (fails) to 5 (works), phone / desktop.

| | a. 10 s to the decision | b. clear unopened | c. cost of waiting | d. answer without hunting | e. information vs decision | f. next briefing | g. nothing cut or hidden | h. reads on the device |
|---|---|---|---|---|---|---|---|---|
| Live baseline | 2 / 2 | 2 / 2 | 1 / 1 | 2 / 2 | 1 / 1 | 1 / 1 | 1 / 1 | 2 / 3 |
| Loop 1 | 5 / 5 | 4 / 4 | 3 / 3 | 4 / 4 | 3 / 3 | 2 / 2 (revised from 3) | 4 / 4 | 5 / 4 |
| Loop 2 | 5 / 5 | 4 / 4 | 4 / 4 | 4 / 4 | 3 / 3 | 2 / 2 | 4 / 4 | 5 / 4 |
| **Loop 3** | **5 / 5** | **4 / 4** | **4 / 4** | **4 / 4** | **4 / 4** | **5 / 5** | **4 / 4** | **5 / 4** |

Measures (mine, same as the designer's): loop 3 is 3.5 phone screens at 375 px (4.9 at 320 px, 2.9 at 1280 px), 485 words, no sideways scroll at 320, 375 or 1280, no ellipsis anywhere, 29 Copy buttons of which 4 are visible without opening anything.

## Fixed since loop 2 (confirmed)
- The face of the page holds no internal id except "S17" in one row title ("Fix the sign-in key storage (S17)"). Session ids, paths and "P11 h" are in Details.
- Each Copy button copies exactly the words: I clicked the 4 visible ones; they gave "talk box: off until the drain works", "talk box: keep, with honest wording", "yes, start a journalist session with PrompTugal__News__Website as its source" and "yes, start the strikes session". The two alternatives are two lines with a Copy each.
- Next briefing is real and plain: "last briefed 28 Nov 01:47 UTC . next briefing 28 Nov 08:30 UTC (08:30 Lisbon)".
- "What changed since you last looked" is real (five dated lines); a heartbeat line sits first; every card and row carries Decision, Approval or For information and a date.

## Where Dinis still gets lost
1. **The this-week rows' answer lines are the data's long paragraphs.** Row 1 ("Let the conductor read reader comments") says: "Yes: cl-6.conductor owns the talk_lane drain per board/talk-drain.md. Grant it host dev.send.sgraph.ai (lane calls only), one no-tool summariser sub-agent, and writes to Website board/inbox.json ..." about 70 words with a host, two paths and a policy name; Copy would copy all of it. The Now cards are clean; the rows are not. Ask cl-6.decisions for a short `answer_line` (the yes) and a `scope` kept in Details.
2. **"Where: any session (conductor's or cl-6.decisions')" is the same on every item I opened**, including the strikes and journalist cards that earlier said "in cl-6.maestro's session". Boilerplate is not information; if the real place differs per item, the field is not carrying it.
3. **A Copy button on a template.** "What is /app/ now?" answers with "/app/ is now: <one sentence, your words>": Copy copies a blank he must fill in. Label it "Copy and fill in", or give a text box.
4. **Some row titles are still topics, not asks**: "What is /app/ now?", "How does the reading meter charge?", "Who does the footer name as responsible?", and "(S17)".
5. **"Running fine" contains "17 blocked" and "Needs a look: 6 data sources with a problem".** A heading that says fine over a blocked count reads as a contradiction. Rename the band, for example "The rest".
6. **Still no recommended answer on "off, or honest wording?"** He does not know which the team advises (the `recommended` field is asked for, not in the data).
7. **"Answered (1): Who owns content" is a title only**: no answer, no time.
8. **Public or private (not mine to decide):** as drawn, a public page would show "Let eight sections publish their keys", "Seal the outreach CRM vault" and "How does the reading meter charge?" next to the designer's own note that decision cards belong behind sign-in. Until the `public` flag is on the data, cl-6.conductor, cl-6.decisions and cl-6.security should treat that as open; I did not check what any of those rows say about a private person (none seen).
9. Not tested: "Do this yourself" and "Pass this on" boxes (none visible; they may be inside the Can wait rows); a row's own Copy; the desktop right rail (described, not drawn: desktop h stays 4).

Re-run on loop 4.
