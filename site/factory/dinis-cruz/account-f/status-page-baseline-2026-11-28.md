# /newsroom/status/ baseline, loop 0 (2026-11-28T02:18Z)

Asked by cl-6.conductor at Dinis's request. Persona: **SYNTHETIC operator, 2 minutes on a phone, wants to know what to decide**. It is a persona modelled on the brief, played by me in one run: it is not Dinis's own view and says nothing for him. Method: scripted Chromium at 390 x 844 px, page text, positions and a full-page screenshot (kept in my scratchpad), page built 2026-11-28 02:00 UTC. Scores 1 (fails) to 5 (works).

The page: 14,442 px tall (17.1 phone screens), about 2,200 words, no sideways scroll.

| Question | Score | Evidence |
|---|---|---|
| Find the top decision in under 10 seconds | **2** | The first screen is the title, share buttons, a tab row and a three-line intro. "Waits on Dinis" starts at 787 px, at the fold, with the sticky bottom bar over it; the first decision is about 1.2 screens down. Nothing says "this is the top one"; urgency ("now", "high", "next", "today") is a bullet after each item, and the order is not strictly by it ("today" comes after "next"). |
| Understand each item without internal ids | **2** | The first line of each item is plain ("Publishing is blocked: the journalist has no website attached"), then ids and paths break in: "questions.json a7914b5", "P11", "content/about/**", "sha256:0d045a0b55734ac7", "cl-6.abp and cl-6.decisions". About 14 such ids and hashes in the page text. |
| Copy the full answer line | **2** | The "line that answers it" is quoted and mostly whole, but there is no copy control, and the text around it is cut with an ellipsis: "It may create…" and "your choice: turn the box off, or keep it with honest wording,…" (cut mid-sentence). Six cut-offs found in total, three of them in decisions. |
| Know when he is next briefed | **1** | Only past times: "Built 2026-11-28 02:00 UTC", "read: 2026-11-28T01:57Z". No next briefing time, and the times are in machine format. |
| What should go, and what is missing | see below | |

## What should go
- "Every agent" (about 4,000 px), "Other teams" and "The data" sit between the decisions and the footer: the operator in 2 minutes does not need them first. Fold them under one line each.
- The same issue appears twice: the /talk/ box problem is in both "From the briefing" and "Open questions".
- Raw hashes, file names, ids and ISO timestamps in the decision text; keep them behind a "details" fold.
- The three-line intro and the share buttons above the first decision.

## What is missing
- A count and a clock at the top: "N waiting for you, M today; next briefing HH:MM".
- The top decision first, marked, with its one-line answer and a copy button.
- Urgency as a label that sorts the list, visible for the 20 folded items too ("20 more" hides their urgency).
- Plain headings (no "Open questions" next to "From the briefing"); who asked and since when is there, good.

Next: re-run on each design loop the designer sends.
