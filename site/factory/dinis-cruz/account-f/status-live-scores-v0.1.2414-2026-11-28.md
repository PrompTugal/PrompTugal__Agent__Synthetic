# Live /newsroom/status/ at v0.1.2414: public mode scored (2026-11-28T02:52Z)

Asked by cl-6.conductor. Personas as before: **SYNTHETIC admin (the operator), 2 minutes on a phone, then a desktop** and a **SYNTHETIC cold reader**; personas modelled on the brief, played by me in one run, not Dinis's view and not said for him. Method as for the baseline: scripted Chromium at 320, 375, 1280 and 1440 px on the live page, page text, positions, screenshots in my scratchpad (not in the repository). Scores 1 (fails) to 5 (works), phone / desktop. This is the **public** mode only; the admin mode is not built yet.

## The operator on the public page (a to h)
| | Live before (baseline) | Live public mode, v0.1.2414 |
|---|---|---|
| a. 10 s to the decision | 2 / 2 | 3 / 3 |
| b. clear unopened | 2 / 2 | 4 / 4 |
| c. cost of waiting | 1 / 1 | 4 / 4 |
| d. answer without hunting | 2 / 2 | 2 / 2 |
| e. info vs decision | 1 / 1 | 3 / 3 |
| f. next briefing | 1 / 1 | 1 / 1 |
| g. nothing cut or hidden | 1 / 1 | 3 / 3 |
| h. device | 2 / 3 | 3 / 4 |

Measures: **8.8 phone screens at 375 px (12.3 at 320, 6.7 at 1280, 5.9 at 1440), about 1,070 words**, no sideways scroll at any width. The baseline was 17 to 18 phone screens and about 2,200 words; the designer's public mock is 1.3 screens and 170 words.

- **a (3):** "Waiting on Dinis" starts 1,102 px down on a phone (1.4 screens) and 959 px on a 1280 desktop (just below the fold), after the title, share buttons, a 20-item tab row and an intro paragraph. Three plain cards follow. Better than the baseline; not on the first screen.
- **b, c (4):** each item is a plain ask with a one-line summary and "If it waits: ..." ("The publication stays frozen."). "Journalist session" and "restart the news" are still insider words.
- **d (2):** by design the answers are not on the public page ("The answers, and the rest, are not on this page"), so the operator cannot answer here; and the page does not say where he should go instead (a pointer to his full list). That is the gap, not the rule.
- **e (3):** "The newsroom today" gives plain counts (117 articles, the newest dated 26 Nov; 43 agents: 0 working, 26 idle, 17 blocked; 30 datasets: 23 fresh, 6 with a problem), then the waiting list, then the agents and the data. "17 blocked" has no line saying what it means for him.
- **f (1):** no next briefing, by design on the public page; "Built 2026-11-28 02:00 UTC . agents read 02:32 . data read 02:32" only.
- **g (3):** the three cards are whole; two cut-offs remain in "The data" ("Câmara Municipal de Lagos (cm-lagos.p...", "Teatro das...").
- **h (3 / 4):** no sideways scroll; the first 1.4 screens are page furniture before the decisions.

## The cold reader on the public page
| Question | Score | Evidence |
|---|---|---|
| Does it say what the newsroom is? | 4 | "PrompTugal.news is run by AI agents and operated by Dinis Cruz. This page says how it is doing: whether the news is moving, what is waiting on Dinis that is safe to show, what the agents do and how fresh the data is." Plain and honest. |
| Does it say what is waiting, and can I follow it? | 4 | "Waiting on Dinis" with its rule stated ("Only the decisions the decisions agent has marked public appear here"), three cards. "Session" and "writing agent" are not explained; no "since". |
| Anything that should not be public? | 3 (lead) | **Card 3 on the live page names an unpublished address in full ("The London strikes page (strikes.london.place.agent.promptugal.news) is ready but not published yet").** The mock said only "The London strikes page is ready"; the live card adds the hostname. For cl-6.security to rule on. Nothing else I see: no key, token, vault, session id or link to claude.ai (0 claude.ai links), no money, no answer line. |
| Reads on a phone? | 3 | 8.8 screens, no sideways scroll; the three cards sit 1.4 screens down. |

Other things the cold reader meets:
- **The live page is the old long page with the waiting list inserted**, not the designer's 1.3-screen public mode: agents by desk, "Other teams", a "Talk to us" form (with "Comments are not being read yet. We are fixing this." above a Send button), and about 2,400 px of datasets. The agent and data parts match the designer's contract; the page is about six times longer than the mock.
- **"The data" cards show a bare number next to "source problem"** (6, 72, 750, 615, 21, 145) with no unit: a cold reader cannot tell if it is hours, rows or days. Owner: the data agent and dev.
- "Other teams" lists the last-commit time of four other teams' agents: public, and plain.
- The 20-item newsroom tab row (OVERVIEW ... RELEASES) comes before the content on a phone and scrolls sideways within itself.

## Checks I could not run on the mocks
- **Desktop right rail: not present.** At 1280 and 1440 px the page is one column; there is no aside or rail with the counts and the next briefing the designer described. For the public mode that is not needed; for the admin mode it is still not drawn.
- A row's own Copy and "Do this yourself" / "Pass this on": not applicable on the public page (no Copy box, no answer lines: the only Copy is "Copy link" in the share row).

## Owners
cl-6.security: the hostname in card 3. cl-6.dev: the order and length of the live page, the cut-offs, the bare numbers. cl-6.decisions and the conductor: a pointer from the public page to where the operator answers. cl-6.designer: the live page against its public mode (1.3 screens).
