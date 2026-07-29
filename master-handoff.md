# Master hand-off — the one session chain (all projects)

**This folder (Projects → App-Docs) is the single home for cross-project
docs — Patrick's decision, session #71 (2026-07-09): everything in one
folder, backed up and version-controlled (this folder is a git repo;
Patrick does all commits).**

**KEEP THIS FILE TRIM (Patrick, #97).** Only the CURRENT state is
written out in full. The session history lives in
`MysteryCluesTracker/docs/build-history.md`, whose own section headings
carry the session number, the date and a summary of what happened. At
the session-end refresh, rewrite "Where things stand" in place, add the
closing session as one line under "Session history", and drop any line
there that no longer bears on live work — never let per-session
paragraphs accumulate here. Git holds every old version of this file.

## How a session starts

1. Patrick connects **Projects → App-Docs** (this folder) and says read
   the master hand-off.
2. Claude reads this file, then `Publishing-Strategy.docx` (the north
   star: strategy, standing rules, the four products, the learning
   tracker) if the session is publishing/business-side.
3. Claude connects whichever project folder the session's goal lives in
   and reads THAT project's own docs (each app keeps its own material).
4. Patrick names ONE goal; scope it together; Claude waits for his
   "go", asked as CLAUDE.md rule 8 requires — a sentence naming the
   actions and what they act on.

Patrick's opener line: "#NN — name. Read CLAUDE.md and the hand-off,
then tell me where things stand."

## Standing rules

How Claude conducts itself lives in `App-Docs/CLAUDE.md`, which
arrives at the start of every session before anything is read. It is
not repeated here.

## The build-and-test commit rhythm (standing — never trimmed at a refresh)

When a session's work needs a device test, Patrick splits it into two
commits at two different times. First the code commit, before the
build: Patrick commits the code so the build captures the right state,
then triggers it and tests on the phone. Then the docs commit, after
the test: once the phone run confirms the work, Patrick tells Claude
the result, Claude refreshes the project's docs, and Patrick commits
them separately — often in a later session.

What this means at a session start: the previous session's code should
already be committed, but the docs may lag. If the docs still say
"awaiting build or device test," confirm with Patrick how the test
went before assuming the work shipped clean.

## The products (all to be published — decided #71)

1. **Mystery Tracker — web** — live at elyfont.com, Beta. Project:
   `Projects/MysteryTracker` (its own docs: docs/session-start.md,
   docs/handoff.md, ROADMAP.md).
2. **Mystery Clues Track Sheet** (mobile; renamed #78) — PWA in a bare
   Xcode+WKWebView wrapper, App Store, FREE. **← THE ACTIVE EFFORT.**
   Project: `Projects/MysteryCluesTracker` — read
   `docs/upgrade-scope.md` FIRST; it holds every decision.
3. **A Place To Remember (Memory) — iPhone** — Alpha, mostly built.
   Project: `Projects/elderlyassistant` (its own docs: docs/handoff.md,
   pending.txt, parked-items.md, session-start.md). Store prep after
   the Mystery rehearsal; Android eventually (#72).
4. **Memory — web** — DROPPED (#72). elyfont.com gets a pointer to the
   App Store listing only.

## Where things stand (updated 2026-07-29, session #149 — Appendix D finished, the script and docx agree at 417, and #150 takes the two coverage gaps)

**THE APP IS WITH APPLE.** Build **1.0 (2)**, status **Waiting for
Review**, release setting **MANUAL** — so an approval waits for
Patrick rather than putting the app on the store by itself. No word
from Apple as of #143. Nothing in App Store Connect lives in a repo,
so this is the only record.

**#149 FINISHED APPENDIX D.** The docx regenerated and
machine-verified row-for-row — 417 steps, §31 at 27, the
end-of-testing banner (zero mismatches, all 481 rows compared);
the #148 settled accusation family pasted word for word (four
functions in; `accuseYes`, `accuseRight` and `wrongAccTap` out,
entries and map rows both); the four stale descriptions
(`checkStars`, `undoTurn`, `logTurn`, `logOut`) brought current
from fresh code reads and Patrick's approval; all 31 coverage-map
rows citing §22 or §31 re-derived against the current sections;
`clearCellNote`'s row completed (19.4, 19.7, 19.8, 19.9); the
stray "ink" removed; and renderLog and copyLog corrected to
"seven living entry kinds" — the take-back entry can no longer be
written. Every edit went through `build-mcts-test.js`, the docx
regenerated and re-verified after each one. The test-doc catch-up
that led the agenda since the code rebuilds is DONE. Full detail:
build-history.md #149.

**TWO COVERAGE GAPS — #150's GOAL (Patrick's call, #149).** The
re-derivation showed the rebuilt §31 has no close-and-reopen
step, so no step anywhere proves an accusation ending surviving a
kill-and-relaunch (§27 still proves the quit ending's survival);
and gameOverGuard's frozen-screen proof now rests on §27's quit
road alone. Filling both is the next session's goal.

**THE OPENER-NOTE RULE (Patrick, #149).** Every session-end
opener note now begins with Patrick's scripted line — the #148
note had dropped it and this session opened on a stumble because
of it. The requirement is written into "At session end" below.

**THE LOG-AFTER-GAME-OVER IDEA IS CLOSED (Patrick, #149).** He
rethought the parked NICE-TO-HAVE, checked his phone, and the Log
button already stays active at game over — steps 31.18 and 31.27
prove the use. Nothing to build; the entry is out of pending.

**A WORKING NOTE.** Patrick said plainly that he could not track the
renumbering in his head, and a plain numbered list of the section's
Do cells fixed it at once. When a section's numbers shift under him,
print the list without being asked.

Still open (pending.txt numbering): the two coverage gaps
(pending 4) are **#150's goal**. The
mistouching (pending 1) is part built and **Patrick
has parked the remainder** (#141) — the phone's Touch Accommodations
settings, a visible pressed state and taller rows are not to be
raised again until he calls for them; reclaiming the never-used
seats' width is the same fix as the narrow-width screens
(pending 5). Also live: the Feedback-modal bug question (pending 2),
the web-spec evaluation (pending 3), the stale comment tail at line
810 (pending 6), and the step-by-step pipeline document Patrick asked
for at #140 and parked into NICE-TO-HAVE.

Standing habits and notes: after any HTML change, re-copy into the
wrapper's www/ and verify the copy matches exactly. Old/saved games
don't exist and don't matter — no migration concerns, ever (#75).
The free script doubles as the paid tier's future answer key (#90).
The paid-tier design/build (upgrade-scope.md "Decided — session #76")
waits until the free product is finished. The App Store listing name
question is settled and the name is registered (#129) — see
MysteryCluesTracker/docs/pending.txt and ROADMAP.md.

## Session history

The full history lives in `MysteryCluesTracker/docs/build-history.md`.
Every section heading there carries its session number, its date and a
one-line summary of what happened — so the list of headings IS the
index. Read those when something needs finding, rather than keeping a
copy here.

Kept here only while they still bear on live work:

- #148 (2026-07-28): APPENDIX D'S LINE NUMBERS SWEPT AND THE THREE ENDINGS BUILT — every function entry's line number brought current ("as of #148"; 109 pairs machine-checked, zero mismatches); the accusation family rewritten from the #133 code and settled in chat, preserved in build-history #148 for #149's paste; §31 extended 18 → 27 steps with the you-lost, Ann-won and glowing-win endings and the page-wide "— THE END OF TESTING —" banner (document 408 → 417; the docx NOT regenerated, by Patrick's ruling); the review-and-test-together rule written into the styling doc; two ideas parked in NICE-TO-HAVE (capitalizing the game-over lines; the Log copied to the clipboard at game over); the stale You-form note dropped.

- #149 (2026-07-29): APPENDIX D FINISHED — the docx regenerated to 417 and verified row-for-row; the settled accusation family pasted (accuseYes, accuseRight, wrongAccTap out); checkStars, undoTurn, logTurn and logOut brought current; all 31 coverage-map §22/§31 rows re-derived; clearCellNote completed and the "ink" removed; renderLog and copyLog corrected to seven living entry kinds; two coverage gaps found (an accusation ending surviving close-and-reopen; the frozen screen after an accusation ending) and set as #150's goal; the opener-note rule added to "At session end"; the Log-after-game-over NICE-TO-HAVE closed by Patrick's phone check.

## Next session's goal (#150, from #149)

**FILL THE TWO COVERAGE GAPS — the test document's known holes
(#149's find, Patrick's call).**

1. An ending surviving close-and-reopen: no step proves an
   accusation ending survives a kill-and-relaunch (§27 proves the
   quit ending's survival; the rebuilt §31 proves none).
2. The frozen screen after an accusation ending: gameOverGuard is
   proved only on §27's quit road — no step taps the frozen
   screen after an accusation ending.

Both likely land as a few steps in §31's ending games, born the
§22 way: drafted in chat from the real code paths, Patrick
phone-runs the draft as he reads it, then the paste into
`docs/build-mcts-test.js`, the docx regenerated and verified
row-for-row.

**What may take the agenda instead.** Apple's answer on build
1.0 (2) may arrive and set its own — the release is MANUAL, so an
approval waits for Patrick. **The mistouching remainder is PARKED
by Patrick (#141)** and is not to be raised until he calls for it.
Also available: the Feedback-modal bug question (pending 2), the
web-spec evaluation (pending 3), the narrow-width screens
(pending 5), the one-sentence stale comment at line 810
(pending 6), and the step-by-step pipeline document.

The opener note is handed to Patrick in chat at session end —
not stored here (Patrick, #124).

## Loose ends

- Memory's #69 badge-reorder commit/build/phone-check may still be
  pending — confirm with Patrick.
- The elyfont.com home card mis-describes the web app (says
  book-reading; it's a board-game companion).
- The 266-step web test procedure as a tickable web page remains a
  liked idea.
- App-Docs git status CONFIRMED (#97, by file-reading .git/logs —
  no git commands): the repo is real, 29 commits, current through
  "MCTS #96 post-gameplay code fixes warning text."
- The old #72 PWA re-upload loose end is CLOSED (#129, Patrick): the
  earlier PWA build of Mystery Clues Tracker is the old phone
  version, from before the Xcode/WKWebView wrapper. Patrick
  confirmed it is no longer needed or relevant. No re-upload, no
  further action.
- Three reference-only copies were deleted from App-Docs (#129,
  Patrick): mtr-master-test-v2.docx, mtr-master-test.docx, and
  MysteryTracker-spec.md. Each has its real, current copy living in
  the MysteryTracker folder, so nothing was lost.
- elyfont.com home page: add a Mystery Clues Track Sheet card linking
  privacy-policy.html and support.html (both pages live as of #130,
  unlinked from the home page). Deferred by Patrick, #130 — pairs
  naturally with fixing the home card's book-reading mis-description
  (the loose end above).

## At session end

Claude refreshes this file — "Where things stand" rewritten in place,
the closing session added as ONE line under "Session history", and any
line there that no longer bears on live work dropped — plus the active
project's own docs. `Publishing-Strategy.docx` is NOT part of the
routine refresh: it is updated only when something has moved the
strategy forward or backward (Patrick, #146). Such a step shows itself
at the top of Claude's where-things-stand report at a session start —
the app's status with Apple changing is the type — and that is the
moment to ask whether the strategy doc needs a line.

If pending.txt changed, pending.docx is rebuilt
from it to match, machine-checked line-for-line (Patrick, #128).
The refresh is discussed and gets Patrick's go
like any other change (#79), asked in rule 8's form. Claude also scripts a short opener note
and hands it to Patrick in chat — goal, what's decided, the
reading list, and the working rules — at session end
(Patrick, #114/#124). The opener note always begins with
Patrick's scripted line — "#NN — name. Read CLAUDE.md and the
hand-off, then tell me where things stand." — before anything
else (Patrick, #149). Claude also drafts a commit text for each
repo touched, handed in chat beside the opener note
(Patrick, #147). Patrick commits (this repo and any project repos
touched).
