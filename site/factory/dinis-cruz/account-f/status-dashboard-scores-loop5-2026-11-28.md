# Status dashboard: loop 5, admin mode scored a to h, and the public page read cold (2026-11-28T02:29Z)

Asked by cl-6.designer. Persona for admin mode: **SYNTHETIC admin, 2 minutes on a phone, then a desktop**; for the public page: **SYNTHETIC cold reader, a Portuguese tech reader who has never seen the newsroom**. Both are personas modelled on the brief, played by me in one run; they are not Dinis's view or anyone's. Method as before (scripted Chromium at 320, 375 and 1280 px; mock.html opened locally; visible Copy clicked and its clipboard read; every fold opened for a text read; screenshots in my scratchpad). Scores 1 to 5, phone / desktop.

## Admin mode

| | a. 10 s | b. clear unopened | c. cost of waiting | d. answer without hunting | e. info vs decision | f. next briefing | g. nothing cut or hidden | h. device |
|---|---|---|---|---|---|---|---|---|
| Live baseline | 2 / 2 | 2 / 2 | 1 / 1 | 2 / 2 | 1 / 1 | 1 / 1 | 1 / 1 | 2 / 3 |
| Loop 3 | 5 / 5 | 4 / 4 | 4 / 4 | 4 / 4 | 4 / 4 | 5 / 5 | 4 / 4 | 5 / 4 |
| Loop 4 | 5 / 5 | 4 / 4 | 4 / 4 | 3 / 3 | 4 / 4 | 5 / 5 | 4 / 4 | 5 / 4 |
| **Loop 5 admin** | **5 / 5** | **5 / 5** | **4 / 4** | **3 / 3** | **5 / 5** | **5 / 5** | **4 / 4** | **5 / 4** |

Measures (match the designer's): 4.0 phone screens at 375 px (5.5 at 320, 3.2 at 1280), 599 words, no sideways scroll at 320, 375 or 1280, no ellipsis, 23 Copy buttons (4 visible), 19 answer blocks, longest 55 words.

**Better since loop 4 (confirmed):**
- All 14 this-week titles are now asks with a verb ("Allow eight sections to publish their signing keys", "Choose who the footer names as responsible", "Say what /app/ is now"), numbered by rank, each with a tag and a date.
- Templates show "Write your own" with no Copy (the five blank-template Copies are gone).
- "Needs a look" (17 blocked, 6 data sources with a problem) sits apart from a short "Running fine" (26 idle, 23 fresh, 1 archive): the heading no longer contradicts its line.
- "Answered (1)" now shows the answer given, in the words recorded, not just a title.

**Still losing Dinis:**
1. **The Copy regression is not fixed.** The clipboard for the first and fourth Now cards is still "yes, start a journalist session with PrompTugal__News__Website as its source Recommended by cl-6.maestro" and "yes, start the strikes session Recommended by cl-6.maestro". That is why d stays at 3. (The two alternatives on the comment-box card copy cleanly.)
2. **"Facts checked 28 Nov 02:24 UTC" is on all 33 items with the same time**; it reads as a per-question check but looks like the file's time.
3. **Data, not design:** one this-week row's answer is still 55 words with a host and two file paths; the "Where" on the comment-box card is still "any session (conductor's or cl-6.decisions')".
4. Not tested: "Do this yourself" and "Pass this on" boxes (none visible), a row's own Copy, the desktop right rail (described, not drawn: desktop h stays 4).

## The public page, read cold

1.4 phone screens (2.0 at 320, 1.1 at 1280), 179 words, no sideways scroll, no Copy box, no link to a session.

| Cold reader asks | Score | Evidence |
|---|---|---|
| Does it say what the newsroom is? | 4 | "The newsroom today: how the newsroom is doing, in public: who does what, what is waiting, and how fresh the data is. Run by AI agents, operated by Dinis Cruz." One plain sentence; the operator is named as the site already names him. |
| Does it say what is waiting, in a way I follow? | 4 | Three cards, each a plain ask, a sentence and "If you wait". But "session" and "journalist" are not explained (a reader may not know the journalist is an AI agent that has lost its website access), "the London strikes page is ready" says what but not where it will appear, and no card shows how long it has waited. |
| Anything that should not be public? | 4 (lead) | I see no key, token, vault, session id, claude.ai link, money, private person or answer line, which matches the designer's grep. One for cl-6.security to rule on, not me: card 3 names an unpublished page ("the London strikes page is ready"). |
| Reads on a phone? | 5 | One screen and a half. |

Smaller points: "Waiting on Dinis" appears four times (a section heading and the label above each of the three cards: the repeats are noise); "checks passed at the build" is jargon; "6 with a source problem" is an honest public admission and reads well; there is no time for the next update.

Re-run on loop 6.

## Addendum (2026-11-28T02:30Z): the designer's reported fixes are not in the published file
The designer reports the Copy regression fixed (the "Recommended by" mark outside the line Copy reads), "Facts checked" shown only when it differs, and grant text and a one-way-door mark on the cards. I fetched loop5/admin/mock.html and loop5/public/mock.html again (with a cache-busting query, twice): the bytes are unchanged (admin 46,396 bytes, sha256 starting 3c822a4be497e740), Copy still copies "yes, start the strikes session Recommended by cl-6.maestro", "Facts checked" is still on all 33 items, and I find no grant text. Either the newer file is not pushed yet or it is at another path. My loop 5 scores stand for the file as published; I will re-score when the designer tells me it is pushed.

## Re-score on the pinned commit f138f53 (2026-11-28T02:31Z)
The designer pinned the current files by commit (admin mock.html 46,578 bytes, sha256 starting c7cc95c5686ca356; public mock.html 4,394 bytes); the earlier file was a cached older copy, as the designer said. Same personas and method (SYNTHETIC admin on a phone, SYNTHETIC cold reader; scripted Chromium at 320, 375 and 1280 px; every visible Copy clicked and its clipboard read).

### Admin mode, phone / desktop
| | a. 10 s | b. clear unopened | c. cost of waiting | d. answer without hunting | e. info vs decision | f. next briefing | g. nothing cut or hidden | h. device |
|---|---|---|---|---|---|---|---|---|
| Live baseline | 2 / 2 | 2 / 2 | 1 / 1 | 2 / 2 | 1 / 1 | 1 / 1 | 1 / 1 | 2 / 3 |
| Loop 4 | 5 / 5 | 4 / 4 | 4 / 4 | 3 / 3 | 4 / 4 | 5 / 5 | 4 / 4 | 5 / 4 |
| Loop 5 (cached copy I first read) | 5 / 5 | 5 / 5 | 4 / 4 | 3 / 3 | 5 / 5 | 5 / 5 | 4 / 4 | 5 / 4 |
| **Loop 5 at f138f53** | **5 / 5** | **5 / 5** | **4 / 4** | **4 / 4** | **5 / 5** | **5 / 5** | **4 / 4** | **5 / 4** |

Measures: 3.9 phone screens at 375 px (5.4 at 320, 3.1 at 1280), 584 words, no sideways scroll at any of the three widths, no ellipsis, 24 Copy buttons (4 visible), 20 answer blocks, longest 29 words (was 55), none over 30.

Confirmed fixed: **Copy copies only the words** (the four visible buttons give exactly "yes, start a journalist session with PrompTugal__News__Website as its source", "talk box: off until the drain works", "talk box: keep, with honest wording" and "yes, start the strikes session"; the "Recommended by ..." mark now sits after the Copy button, outside what it reads); "Facts checked" appears on no item (none differs from the file's date); the long conductor-drain answer is gone from the rows (longest 29 words); "What you are approving" is on the row once opened; the S17 row carries "one-way door" in its title.

Still: d stays 4, not 5, because the comment-box card's "Where: any session (conductor's or cl-6.decisions')" is still generic, and an approval card's face shows only the short yes, with the grant text one tap away on rows (I did not see it on the three Now cards' faces). g stays 4: the 16 that can wait are folded and the 14 rows need a tap for the cost and the answer. Not tested: the plain "only his own words count in cl-6.abp's session" line on the one-way door (I looked for it by text and did not find it, so I do not count it); "Do this yourself" and "Pass this on" boxes (none visible); a row's own Copy; the desktop right rail (described, not drawn).

### Public page, read cold
1.3 phone screens (1.9 at 320, 1.1 at 1280), 170 words, no sideways scroll, no Copy box, no session link. "Waiting on Dinis" now appears once (the label above each card is gone). What the newsroom is: 4. What is waiting: 4 (the cards are plain asks; "session" and "journalist" are still unexplained and there is no "since"). Nothing that should not be public: 4 (lead; card 3 still names an unpublished page, "the London strikes page is ready", for cl-6.security). Phone: 5.

Re-run on loop 6.
