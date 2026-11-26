# First wake: reader pass at v0.1.2306 (2026-11-26T11:27Z)

SYNTHETIC reader pass, scripted Chromium at 390 px (phone) and 1280 px (desktop), public pages only, geo lookups blocked, no sign-in. It is a measurement, not a persona's full read: I did not open a story page (my link finder returned the articles index; a second attempt timed out), so no story-level provenance finding is made.

## Measured
- No sideways scroll at 390 px on the front page, /newsletter/, /about/ and /companies/. (Good for the iOS app, which reuses these pages.)
- F56 fixed: the front page no longer shows "N items" in the days strip. F15 and F60 not present on the front page.
- F58 still stands: /newsletter/ says "Subscribers and sending are handled by the Web Summit team, not on this site".
- F06 still stands: /about/ says "the writing desks are next".
- F57 (dev.pages@): the search box on /companies/ now has a placeholder ("Search companies, people, events") but no aria-label: a screen reader still has no name for it. Placeholder part fixed, label part open.
- F50: the footer reads "Edited by Dinis Cruz, Indi Gupte and Vicky Wang, made with AI agents." (checked on the articles index only; the story-page line "No person read" not re-checked).
- New (N1, for dev@ and conductor@, to confirm on a story page): the desktop masthead shows "Pay for what you read · £4.99" while /account/ says "Nothing is charged": the F01 wording problem may be back in a different place. I did not capture its context, so treat it as a lead, not a finding.
- The masthead has an "App" link: the iOS app's entry on the site. Where it leads and what it says is the next thing to read.

## Not done
No story read, no persona run, no screenshot. Next wake: one persona on a story page and on what the "App" link says.
