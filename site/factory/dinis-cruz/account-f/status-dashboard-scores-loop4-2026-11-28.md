# Status dashboard: scores a to h, loop 4 beside baseline and loops 1 to 3 (2026-11-28T02:28Z)

Asked by cl-6.designer (loop 4 supersedes loop 3). Persona: **SYNTHETIC admin, 2 minutes on a phone, then a desktop; a persona modelled on the brief, played by me in one run, not Dinis's view and not said for him.** Method as before: scripted Chromium; the mock.html files opened locally at 320, 375 and 1280 px; every visible Copy clicked and its clipboard read; all folds opened for a text read of every answer line; text, positions, screenshots in my scratchpad. Scores 1 (fails) to 5 (works), phone / desktop.

| | a. 10 s | b. clear unopened | c. cost of waiting | d. answer without hunting | e. info vs decision | f. next briefing | g. nothing cut or hidden | h. device |
|---|---|---|---|---|---|---|---|---|
| Live baseline | 2 / 2 | 2 / 2 | 1 / 1 | 2 / 2 | 1 / 1 | 1 / 1 | 1 / 1 | 2 / 3 |
| Loop 1 | 5 / 5 | 4 / 4 | 3 / 3 | 4 / 4 | 3 / 3 | 2 / 2 | 4 / 4 | 5 / 4 |
| Loop 2 | 5 / 5 | 4 / 4 | 4 / 4 | 4 / 4 | 3 / 3 | 2 / 2 | 4 / 4 | 5 / 4 |
| Loop 3 | 5 / 5 | 4 / 4 | 4 / 4 | 4 / 4 | 4 / 4 | 5 / 5 | 4 / 4 | 5 / 4 |
| **Loop 4** | **5 / 5** | **4 / 4** | **4 / 4** | **3 / 3** | **4 / 4** | **5 / 5** | **4 / 4** | **5 / 4** |

Measures (match the designer's): 3.7 phone screens at 375 px (5.3 at 320, 3.1 at 1280), 540 words, no sideways scroll at 320, 375 or 1280, no ellipsis, 35 Copy buttons (4 visible), 34 questions (3 now, 14 this week, 16 can wait, 1 answered).

## Why d went down from 4 to 3: a regression
**The clipboard now holds more than the words.** Clicking the visible Copy on the second and third Now cards gives "yes, start a journalist session with PrompTugal__News__Website as its source Recommended by cl-6.maestro" and "yes, start the strikes session Recommended by cl-6.maestro". The "Recommended by" line that sits inside the answer box is copied with the words; in loop 3 the copy was exact. He would paste "Recommended by cl-6.maestro" into the session. The two lines of card 1 still copy cleanly (no recommendation there).

## Fixed or better since loop 3 (confirmed)
- "Where" now names the place and links to it for most items (cl-6.maestro's session, cl-6.abp's session, GitHub, cl-6.signals, cl-6.places and others); card 1 still says "any session (conductor's or cl-6.decisions')".
- Recommended answers shown on three cards by cl-6.maestro and one by cl-6.observability, and none where it is Dinis's own call (card 1): the page does not steer him there.
- Long rows are shorter: 27 answer blocks, longest 55 words (was about 70), 2 over 30 words. The longest, the conductor's drain grant, still carries a host, two file paths and a "who does what".
- Next briefing and what changed stay real; the face holds only "S17" as an id.

## Where Dinis still gets lost
1. **The copied text has "Recommended by ..." in it** (above).
2. **Five answer lines are templates with a blank** ("my key fingerprint is SHA256:<yours>", "push work/cl-6.<agent>", "/app/ is now: <one sentence, your words>", "yes to <agent> fixing the /newsletter...", "footer: <your wording>"): Copy gives text he must edit, and nothing on the button says so. Label "Copy and fill in".
3. **"Facts checked 28 Nov 02:24 UTC" appears 33 times, all with the same time.** That looks like the file's update time, not a check of each question's facts; on a card it reads as someone checked these facts at that time. Show it once at the top ("decisions list updated"), or per question only when it differs.
4. **"Running fine" still holds "17 blocked" and "Needs a look: 6 data sources with a problem".** The heading contradicts the line; rename ("The rest"), or move the blocked count under the Decide band.
5. **"Answered (1): Who owns content" is still a title only**: no answer, no time.
6. **Rows still need a tap to be understood** (title, tag and date only until opened); some titles are topics ("What is /app/ now?", "How does the reading meter charge?").
7. **Public or private** (conductor, cl-6.decisions, cl-6.security): unchanged from my loop 3 note; every question is `public: false` in the file, so a page that honours it shows no decisions until /admin/ exists.
8. Not tested: "Do this yourself" and "Pass this on" boxes (none visible); a row's own Copy; the desktop right rail (described, not drawn: desktop h stays 4).

Re-run on loop 5.
