# Status dashboard: scores, baseline, loop 1 and loop 2 (2026-11-28T02:23Z)

Asked by cl-6.designer. Persona: **SYNTHETIC admin, 2 minutes on a phone, then a desktop; a persona modelled on the brief, played by me in one run, not Dinis's view and not said for him.** Method as before: scripted Chromium; the live page /newsroom/status/ (v0.1.2412), loop 1 and loop 2 mock.html opened locally at 320, 375 and 1280 px; Copy clicked and its clipboard read; page text, positions, screenshots in my scratchpad. Scores 1 (fails) to 5 (works), phone / desktop where they differ. Same points as before plus the designer's extras.

| Point | Live baseline | Loop 1 | Loop 2 |
|---|---|---|---|
| Top decision in 10 s | 2 / 2 | 5 / 5 | 5 / 5 |
| Items without internal ids | 2 / 2 | 2 / 2 | 3 / 3 |
| Copy the full answer line | 2 / 2 | 4 / 4 | 4 / 4 |
| Know when next briefed | 1 / 1 | 2 / 2 (revised from 3) | 2 / 2 |
| Nothing cut or hidden | 1 / 1 | 4 / 4 | 4 / 4 |
| Consequence of waiting | 1 / 1 | 3 / 3 | 4 / 4 |
| Information versus decision | 1 / 1 | 3 / 3 | 3 / 3 |
| Phone at 320 px | not measured | not measured | 5 |

I revised loop 1's "next briefed" from 3 to 2: its time was an example, not an answer; loop 2 says plainly "not reported yet", which is more honest but still no answer, so both are 2. It becomes 5 when cl-6.maestro supplies the time.

Measures: loop 2 is 3.1 phone screens at 375 px (4.6 at 320 px, 2.6 at 1280 px), 423 words, no sideways scroll at 320, 375 or 1280, no ellipsis anywhere, 3 Copy buttons, and the Copy copies the whole line. These match the designer's.

## What got better in loop 2
A one-line state at the top; three Now cards instead of five, each with a concrete "If you wait" ("Every comment readers write is lost", "The publication stays frozen"); the titles are mostly plain tasks ("Restart the news..."); the 29 questions are all on the page (nothing behind "N more"); an Answered band; "next briefing: not reported yet" instead of a made-up time.

## Where Dinis still gets lost
1. **Card 2's answer box (the most important one) still holds a session id, "P11 h", two file paths, "add_repo" and a fallback sentence.** He cannot say that in one breath. The answer should be only "yes, start a journalist session with PrompTugal__News__Website as its source", the place ("in cl-6.maestro's session") in its own line with a link: the data fields `where` and `where_url` the designer asked cl-6.decisions for. Card 3 also shows a session id.
2. **Card 1 puts two answers in one Copy box and shows no recommendation.** The copy gives both lines; he must delete one and does not know which the team advises. One box per option, with the recommended one marked (the `options` field).
3. **The Decide soon rows are 11 titles with dates and nothing to rank them by.** All carry the same shape, no consequence until opened, and some are topics not asks ("What is /app/ now?", "How does the reading meter charge?"), one still has an id ("Fix the sign-in key storage (S17)"). I did not test whether a row opens into the full card.
4. **The state line alarms and does not guide.** "17 agents blocked . 6 data sources with a problem" sits next to "3 need you now": a reader asks why 17 blocked agents give 3 decisions. It reads as trouble with nothing to do. Link each count to what it needs, or say "17 agents blocked: 3 of them on you".
5. **The page contradicts its own notice.** It says "anything about keys, money or private people is not shown here", yet a row says "Let eight sections publish their keys" and another "Fix the sign-in key storage (S17)". The public: true flag is not on the data yet; until it is, the notice is untrue. (Public or private is for the conductor, cl-6.decisions and cl-6.security.)
6. **"Answered (1): Who owns content" shows a title only**: he cannot tell what was answered or when. Add the answer and the time.
7. **"What changed since you last looked" is still an EXAMPLE box, and "last briefed / next briefing" are "not reported yet".** Honest, but until cl-6.maestro's feed exists, e and f cannot score above 3 and 2.
8. Not tested: whether the Can wait fold lists titles when opened; whether the row's Details holds the answer and a Copy button.

## What should be on the page
The state line (with each count linked to what it needs), the Now cards with a one-line answer, the recommended option marked, a ranked Soon list with a consequence in each row, Answered with the answer, a real "what changed" and the briefing times. **What should not:** session ids, paths, policy codes and "add_repo" in the answer; anything the notice says is not shown; the unexplained 17 and 6.

Re-run on loop 3.
