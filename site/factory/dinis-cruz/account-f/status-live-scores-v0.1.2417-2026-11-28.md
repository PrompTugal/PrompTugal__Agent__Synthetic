# Live /newsroom/status/ at v0.1.2417: round 2 scored (2026-11-28T03:28Z)

Asked by cl-6.conductor. Personas as before: **SYNTHETIC admin (the operator), 2 minutes on a phone, then a desktop**, and a **SYNTHETIC cold reader**; personas modelled on the brief, played by me in one run, not Dinis's view and not said for him. Method as before: scripted Chromium on the live page at 320, 375, 768, 1024, 1099, 1100, 1280, 1440 and 1920 px, page text and positions, screenshots in my scratchpad (not in the repository). Scores 1 (fails) to 5 (works), phone / desktop. Public mode only (the admin mode is not built).

## The operator (a to h)
| | Baseline | v0.1.2414 | **v0.1.2417** |
|---|---|---|---|
| a. 10 s to the decision | 2 / 2 | 3 / 3 | **4 / 5** |
| b. clear unopened | 2 / 2 | 4 / 4 | **4 / 4** |
| c. cost of waiting | 1 / 1 | 4 / 4 | **4 / 4** |
| d. answer without hunting | 2 / 2 | 2 / 2 | **3 / 3** |
| e. info vs decision | 1 / 1 | 3 / 3 | **4 / 4** |
| f. next briefing | 1 / 1 | 1 / 1 | **1 / 1** |
| g. nothing cut or hidden | 1 / 1 | 3 / 3 | **4 / 4** |
| h. device | 2 / 3 | 3 / 4 | **4 / 5** |

Measures: **5.6 phone screens at 375 px (8.0 at 320, 4.2 at 1280, 3.7 at 1440), about 650 words** (v0.1.2414: 8.8 screens, 1,066 words; baseline 17 to 18 screens, 2,200 words); no sideways scroll at 320, 375, 768, 1024, 1099, 1100, 1280, 1440 or 1920 px; no ellipsis (the two cut-offs in the data list are gone); 15 folds, all closed by default; no claude.ai link, no session id, no key; only "Copy link" as a Copy.

- **a (4 / 5):** on a phone the counts block is at 719 px and "Waiting on Dinis" at 987 px, the first card at 1,091 px (1.3 screens): one scroll. On a desktop at 1280 px the waiting list is at 678 px, above the fold, next to the rail: 5.
- **d (3):** "Dinis answers in cl-6.decisions' session." now sits under the three cards. He knows where; by design he still does not see the words here.
- **e (4):** the counts are labelled and in one place ("117 articles published; the newest is dated 26 Nov", "43 agents: 0 working, 26 idle, 17 blocked", "30 datasets: 23 fresh, 1 archive, 6 with a source problem"). "17 blocked" still has no line on what it means for him.
- **f (1):** no next briefing on the public page; "Built 2026-11-28 03:00 UTC . agents read 02:32 . data read 02:32" only.
- **g (4):** the agents, other teams and datasets are folds closed by default with a labelled one-line count ("Every agent, by desk", "Agents of other teams (4)", "Every dataset, with its source and date"); nothing is cut. The six source problems are no longer visible until the data fold is opened.

## The right rail (the check the mocks could not give)
At **1100 px and wider** there is an aside ("The newsroom today": the counts) in a 280 px column on the right, beside "Waiting on Dinis", which then starts at 678 px. At **1099 px and below** the aside drops above the content as a full-width block and "Waiting on Dinis" starts at 896 to 916 px (768 and 1024 px). The break at exactly 1100 px is as described. The rail holds counts only: no next briefing (public mode).

## The cold reader
| Question | v0.1.2414 | **v0.1.2417** | Evidence |
|---|---|---|---|
| Does it say what the newsroom is? | 4 | **4** | "How the newsroom is doing, in public: who does what, what is waiting, and how fresh the data is. Run by AI agents, operated by Dinis Cruz." One plain line (shorter than before). |
| What is waiting, can I follow it? | 4 | **4** | Three cards with "If it waits"; the rule is now "Only decisions marked public are shown."; "session" and "writing agent" still unexplained, no "since". |
| Anything that should not be public? | 3 (lead) | **3 (lead)** | Card 3 still names the unpublished address in full: "The London strikes page (strikes.london.place.agent.promptugal.news) is ready but not published yet." Unchanged from v0.1.2414; for cl-6.security. Nothing else I see. |
| Reads on a phone? | 3 | **4** | 5.6 screens, no sideways scroll; the waiting list one scroll down. |

## What still loses the reader or the operator
1. **The unpublished address in card 3** (cl-6.security's call, not mine; unchanged).
2. **No next briefing and no answer words on the public page** (f 1, d 3): by design in public mode; the page now says where he answers, not when he is briefed.
3. **"17 blocked" and "0 working" are bare**: nothing says whether that is normal for a quiet night.
4. **The 20-item newsroom tab row still comes before the content** (about 450 px on a phone).
5. **The "Talk to us" form is on a page that says "Comments are not being read yet"**, honest but odd beside a Send button.

Owners: cl-6.security (1), cl-6.conductor and cl-6.decisions (2), cl-6.dev (3, 4), cl-6.designer for the whole.
