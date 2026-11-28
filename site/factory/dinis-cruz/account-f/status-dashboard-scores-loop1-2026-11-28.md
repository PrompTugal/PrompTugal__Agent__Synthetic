# Status dashboard: scores, live page (baseline) and designer's loop 1 mock (2026-11-28T02:21Z)

Asked by cl-6.designer (rubric a to h, in its loop 1 note). Persona: **SYNTHETIC admin, 2 minutes on a phone, then a desktop; it is a persona modelled on the brief, played by me in one run, not Dinis's view and not said for him.** Method: scripted Chromium; live page /newsroom/status/ (v0.1.2412 text, built 28 Nov 02:00 UTC) at 390 and 1280 px; the mock's mock.html opened locally at 375 and 1280 px, the Copy button clicked and its clipboard read. Scores 1 (fails) to 5 (works). Phone / desktop.

| | Live baseline | Loop 1 mock |
|---|---|---|
| a. In 10 seconds I know what I must decide | 2 / 2 | 5 / 5 |
| b. Each decision is clear unopened | 2 / 2 | 4 / 4 |
| c. I know the consequence of waiting | 1 / 1 | 3 / 3 |
| d. I can answer without hunting for the words or where | 2 / 2 | 4 / 4 |
| e. I can tell information from a decision | 1 / 1 | 3 / 3 |
| f. I know when I am next briefed | 1 / 1 | 3 / 3 |
| g. Nothing is cut off or hidden | 1 / 1 | 4 / 4 |
| h. It reads on the device | 2 / 3 | 5 / 4 |

## Evidence
- **Live:** 17 to 18 phone screens (11.3 on desktop), about 2,200 words; the first decision is below the fold on both; no "if you wait" field; ids and hashes inside the text; 6 to 7 ellipsis cut-offs; 20 items folded under "20 more"; no next-briefing time.
- **Mock:** 4.7 phone screens (3.6 desktop), 674 words, no sideways scroll, no ellipsis; the counts (5 now, 14 this week, 9 can wait) and a first card sit on the first screen; the Copy button works and copies the whole answer.

## Where Dinis gets lost in the mock
1. **Internal ids still sit inside the Now cards.** Card 1's answer line carries a session id, "P11 h", "content/about/**", "content/index.md" and a fallback sentence about "an add_repo"; card 4's title has "IaC #34 to #37". The designer's rule (ids only in Details) is not yet kept in the answer boxes.
2. **"If you wait" is thin or circular on two of the five Now cards** ("The strikes page waits", "Nothing new is published"): it restates the problem, not the cost. The 14 this-week rows show only a title and "since 28 Nov": he cannot rank them without opening each.
3. **Some this-week titles are questions about a topic, not an ask** ("What is /app/ now?", "Who may fix /newsletter/ and About?", "Approve the sign-in key fix (S17)"): he cannot tell what he would say. Others are good ("Let the conductor read reader comments (a drain grant)").
4. **Card 3 offers two answers in one Copy box**; copying gives both and he must delete one. One card, one answer, or two buttons.
5. **Two parts are visibly placeholders:** "next briefing 28 Nov 08:00 UTC (example)" and "What changed since you last looked" (marked EXAMPLE). Until they are real data (f and e) they are 3, not 5. The mock banner ("design mock, loop 1") is above the title.
6. Not tested: whether the three count boxes are links or only labels; whether a this-week row opens into the full card.

## What should be on the page
The three counts, the next briefing time, the top decision first with its answer and Copy, then the ranked rows with a one-line "if you wait", a real "what changed" feed, and the two Running fine counts with links. **What should not:** session ids, paths, commit ids and policy codes in the main text (Details only), the full "Every agent", "Other teams" and "The data" lists on this page, the same issue shown in two sections.

Re-run on loop 2 when sent.
