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

## Where things stand (updated 2026-07-28, session #147 — the fresh §22 is built into the spec, the document stands at 408 steps, and Appendix D is the one catch-up piece left)

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

**#147 BUILT THE FRESH §22 — 32 STEPS, THE DOCUMENT AT 408.**
Patrick's #145 ruling executed: the section opens on its own game
(New Game — Same Players, Same Deck, by design, keeping §23's deck
proofs standing — and a 3-card hand) and inherits nothing. Beyond
the old section's ground it proves one new thing at Patrick's call:
a wrongly-accused player can then QUIT and leave both rings — Ann
quits on top of her 😢, showing nothing. The section keeps the one
proof unique to it (a quitter's ✅ turning Bob's old "!" into a ❌)
and folds in the 22.28 Log wording settled at #145. Patrick
phone-verified the draft during mark-up BEFORE it touched the
script; the docx was regenerated and machine-verified row-for-row.
§23's opening — banner and five lines — now runs straight off
22.32. Full detail: build-history.md #147.

**THE BARS HAVE NAMES (Patrick, #147): the Turn Bar and the
Message Bar**, declared where the layout walk meets them (8.6 and
8.7) and used throughout the document. "Bottom strip", "message
strip" and "status strip" are gone — three names for one thing,
and on the Game screen "bottom" was simply wrong: messages take
over the hint line between ↩ Undo and Next ▶ (verified at
`showStatus`, line 2765). Inside modals the name stays "the
modal's message line", checked consistent.

**WHAT IS LEFT OF THE CATCH-UP — APPENDIX D ALONE.** Three
functions that no longer exist (`accuseYes`, `accuseRight`,
`wrongAccTap`), five descriptions written before #133, a coverage
map pointing at the OLD §31's numbers in six places and at §22
numbers that #147 has now moved again — its §22 targets must map
to the fresh 22.1–22.32 — drifted line numbers (`logTurn`
860 → 889, `renderTurnBar` 1846 → 1978, `saveState` 2682 → 2800),
and the incomplete `clearCellNote` entry.

**A WORKING NOTE.** Patrick said plainly that he could not track the
renumbering in his head, and a plain numbered list of the section's
Do cells fixed it at once. When a section's numbers shift under him,
print the list without being asked.

Still open (pending.txt numbering): the test-doc catch-up
(pending 4) is now **Appendix D alone**. The
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

## Next session's goal (#148, from #147)

**APPENDIX D — bring the function list and coverage map current.**

The list from #143 stands, with one update from #147: remove
`accuseYes`, `accuseRight` and `wrongAccTap`; bring five
descriptions current (`openAccuseModal`, `checkStars`, `undoTurn`,
`logTurn`, `logOut`); renumber the map's six old-§31 references;
re-point its §22 references at the fresh 22.1–22.32 built at #147;
refresh the drifted line numbers (`logTurn` 860 → 889,
`renderTurnBar` 1846 → 1978, `saveState` 2682 → 2800, `undoTurn`
2241 → 2393); finish the `clearCellNote` entry (19.4, 19.7, 19.8,
19.9).

**One note, not a job.** The #132 You-form and the named card are
still proven nowhere in the document. The fresh §22 gave them no
home — it has no ask of Patrick's that somebody shows. Whether to
spend a step is Patrick's call.

It all goes through `docs/build-mcts-test.js`; the docx is generated
and never hand-edited, then verified row-for-row. The document
stands at 408 steps, §22 at 32.

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

- The commit texts for #147's work were handed in chat at session
  end; if the App-Docs or MysteryCluesTracker commits are missing
  at the next start, ask Patrick before assuming either way.

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
