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

## Where things stand (updated 2026-07-28, session #148 — Appendix D's line numbers current, the accusation family settled awaiting paste, §31 holds the three ending proofs, and the docx is one regeneration behind)

**#146 RESTRUCTURED THE DOCS — NO APP CODE, NO TEST DOCUMENT.**
`App-Docs/CLAUDE.md` now holds how Claude conducts itself, in twenty
rules, and it is the file that arrives automatically before anything
is read. This hand-off holds where things stand, the next goal and
how a session runs. Each project's own `CLAUDE.md` holds its reading
list and nothing else. `session-start.md` is gone. **A session start
reads: this file, then the project's `CLAUDE.md` and the files it
names** — for the mobile app that is the one section of
`build-history.md` this file points at, and
`chat&test-spec-styling.md`. NOT read at a start:
`upgrade-scope.md`, `pending.txt` and `pending.docx`. The automatic
reading fell from about 100,000 characters to about 28,000. Full
detail: build-history.md #146.

**THE APP IS WITH APPLE.** Build **1.0 (2)**, status **Waiting for
Review**, release setting **MANUAL** — so an approval waits for
Patrick rather than putting the app on the store by itself. No word
from Apple as of #143. Nothing in App Store Connect lives in a repo,
so this is the only record.

**#148 BROUGHT APPENDIX D'S LINE NUMBERS CURRENT AND BUILT THE
THREE ENDING PROOFS INTO §31.** The sweep: every function entry in
Appendix D now carries the position its code holds in
mystery-clues-tracker.html today, dated "as of #148" — 109
name-and-number pairs machine-checked afresh after the edit, zero
mismatches; the three dead functions' entries were left untouched
for their own piece. Then, at Patrick's call, §31 gained three
short games at its end (31.19–31.27): "Game over — you lost",
"Game over — Ann won" — bigger letters, no glow — and "⭐ Game
over — you won!" breathing its glow to close the document, with
the Log's "— right" line proved in the last game. A page-wide
"— THE END OF TESTING —" banner now follows the last step, styled
like the section banners. §31 stands at 27 steps, the document at
417. Full detail: build-history.md #148.

**THE DOCX IS ONE REGENERATION BEHIND THE SCRIPT (Patrick's
ruling, #148).** mcts-master-test.docx still holds 408 steps
against the script's 417. Regenerating it and verifying it
row-for-row is #149's first job.

**THE ACCUSATION FAMILY IS SETTLED BUT NOT YET PASTED.** Family
M's rewrite from the #133 code — four functions replacing the dead
three — was drafted, reviewed and settled at #148. The settled
wording is preserved word for word in build-history.md #148; #149
pastes it into Appendix D. The reading also taught: checkStars no
longer opens the accusation modal, and undoTurn's take-back is
gone from the code — no verdict can be undone.

**REVIEW AND TEST TOGETHER (Patrick's rule, #148).** Written into
chat&test-spec-styling.md step 3: whenever the current code is
already loaded on Patrick's phone, his review IS a phone run — he
runs a draft as he reads it. The phone is the only real proof.

**WHAT IS LEFT OF APPENDIX D.** Pasting the settled family M
(entries and map rows in; `accuseYes`, `accuseRight` and
`wrongAccTap` out); four descriptions brought current
(`checkStars`, `undoTurn`, `logTurn`, `logOut`); the coverage map
re-derived — its §31 references against the rebuilt section (the
old numbers predate even the 18-step rebuild, and #148 took it to
27) and its §22 references against the fresh 22.1–22.32; the
`clearCellNote` entry finished (19.4, 19.7, 19.8, 19.9); and the
stray word "ink" taken out of `addMark`'s map row.

**A WORKING NOTE.** Patrick said plainly that he could not track the
renumbering in his head, and a plain numbered list of the section's
Do cells fixed it at once. When a section's numbers shift under him,
print the list without being asked.

Still open (pending.txt numbering): the test-doc catch-up
(pending 4) is **Appendix D, part done at #148**. The
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

- #146 (2026-07-28): NO APP CODE AND NO TEST DOCUMENT — the docs restructured on Patrick's aim of fewer files, shorter, nothing said twice: `App-Docs/CLAUDE.md` rewritten as the one home for conduct (twenty rules), `session-start.md` retired, `MysteryCluesTracker/CLAUDE.md` cut to a reading list, eleven files deleted, the hand-off cut from 434 lines to 263, and `Publishing-Strategy.docx` taken out of the routine refresh; a broken pointer to the deleted `session-start.md` was left in `CLAUDE.md` rule 1 and cost the next session a blind start before it was fixed.

- #147 (2026-07-28): THE FRESH §22 BUILT INTO THE SPEC — 32 steps on its own game (document 405 → 408), drafted in chat, marked up, and phone-verified by Patrick before entering the script; Ann's quit-after-wrong-accusation proof added at his call; §23's opening aligned (six lines); the Turn Bar and Message Bar named at 8.6/8.7 and carried through the whole document; CLAUDE.md rule 8 tightened — every "Go?" must live in a sentence naming its actions and targets — and commit-text drafting added to the session-end routine.

- #148 (2026-07-28): APPENDIX D'S LINE NUMBERS SWEPT AND THE THREE ENDINGS BUILT — every function entry's line number brought current ("as of #148"; 109 pairs machine-checked, zero mismatches); the accusation family rewritten from the #133 code and settled in chat, preserved in build-history #148 for #149's paste; §31 extended 18 → 27 steps with the you-lost, Ann-won and glowing-win endings and the page-wide "— THE END OF TESTING —" banner (document 408 → 417; the docx NOT regenerated, by Patrick's ruling); the review-and-test-together rule written into the styling doc; two ideas parked in NICE-TO-HAVE (capitalizing the game-over lines; the Log copied to the clipboard at game over); the stale You-form note dropped.

## Next session's goal (#149, from #148)

**FINISH APPENDIX D — the docx first.**

1. Regenerate `docs/mcts-master-test.docx` and verify it
   row-for-row: 417 steps, §31 at 27, the end-of-testing banner —
   the script moved at #148 and the docx did not.
2. Paste the settled accusation-family wording from
   build-history.md #148 into Appendix D: the four new entries and
   map rows in; `accuseYes`, `accuseRight` and `wrongAccTap` out.
3. Bring the four descriptions current: `checkStars`, `undoTurn`,
   `logTurn`, `logOut`.
4. Re-derive the coverage map's §31 and §22 references (the
   rebuilt 27-step §31; the fresh 22.1–22.32).
5. The tail: `clearCellNote`'s 19.7 and 19.8; the "ink" in
   `addMark`'s map row.

It all goes through `docs/build-mcts-test.js`; the docx is generated
and never hand-edited, then verified row-for-row. The document
stands at 417 steps in the script, 408 in the docx until step 1
runs.

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
(Patrick, #114/#124). Claude also drafts a commit text for each
repo touched, handed in chat beside the opener note
(Patrick, #147). Patrick commits (this repo and any project repos
touched).
