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

## Where things stand (updated 2026-07-29, session #150 — the coverage gaps filled and proved at 424, and #151 takes the pending cleanup)

**THE APP IS WITH APPLE.** Build **1.0 (2)**, status **Waiting for
Review**, release setting **MANUAL** — so an approval waits for
Patrick rather than putting the app on the store by itself. No word
from Apple as of #143. Nothing in App Store Connect lives in a repo,
so this is the only record.

**#150 FILLED THE COVERAGE GAPS.** Seven steps added, each drafted
in chat from the real code paths and phone-run by Patrick before
the paste: §27 grew to 36 steps (27.34 the quit ending surviving a
kill-and-relaunch, 27.35 the freeze re-proved after the wake,
27.36 the Log, the Notepad, and the Guide all opening at game
over), and §31 grew to 31 (31.28 the frozen screen on the
accusation road, 31.29 the glowing win surviving the relaunch,
31.30 the freeze after the wake, 31.31 the three doors at this
ending too). Nine Appendix D rows brought current — gameOverGuard
now cites both roads by name. The document stands at 424 steps;
after every edit the docx was rebuilt from an exact copy of the
script and machine-verified — the step table's 488 rows and the
coverage map's 134 rows both at zero mismatches, the copy into
docs proved by checksum. One finding corrected the record: before
#150 NO ending's survival was proved anywhere — the old note that
§27 proved the quit ending's survival was wrong; §27 had no reopen
step at all. Full detail: build-history.md #150.

**THE CONDUCT DOCS SPLIT (#150, Patrick's call).**
`chat&test-spec-styling.md` is renamed `test-spec-styling.md` and
trimmed to spec-only; its chat-reporting section now lives solely
in `App-Docs/CLAUDE.md` — the one home for conduct — where rule 16
gained the one line it lacked ("If Claude's checking starts to
thin as the session fills, it says so out loud").
`MysteryCluesTracker/CLAUDE.md`'s reading list points at the new
name. Patrick did the rename; Claude made the three edits.

**THE OPENING-PROCEDURE EDIT IS STILL OPEN (#150).** Patrick asked
for CLAUDE.md rule 1 to become a two-button opening: Claude asks
through the folder-permission button to connect App-Docs, reads
its CLAUDE.md and the hand-off; then asks the same way for
MysteryCluesTracker and reads its CLAUDE.md and
test-spec-styling.md; ONE status report after all the reading,
never one per folder. The wording was drafted and approved in
shape, then paused by Patrick before writing. It waits for his go.

**A WORKING NOTE (#149).** Patrick said plainly that he could not
track renumbering in his head, and a plain numbered list of the
section's Do cells fixed it at once. When a section's numbers
shift under him, print the list without being asked.

Still open: **pending.txt is STALE — cleaning it up is #151's
goal (Patrick's call, #150).** At #150 it was updated only for the
finished coverage-gaps work; every other line stands as earlier
sessions left it and wants a going-over with Patrick, the docx
rebuilt at the end. The mistouching remainder stays **parked by
Patrick** (#141) — the phone's Touch Accommodations settings, a
visible pressed state and taller rows are not to be raised again
until he calls for them; reclaiming the never-used seats' width is
the same fix as the narrow-width screens. Also live: the
Feedback-modal bug question, the web-spec evaluation, the stale
comment tail at line 810, and the step-by-step pipeline document
Patrick asked for at #140 and parked into NICE-TO-HAVE.

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

- #150 (2026-07-29): THE COVERAGE GAPS FILLED — seven steps added, drafted in chat and phone-run before the paste (§27 → 36: the quit ending's reopen proof, the freeze after the wake, the three doors at game over; §31 → 31: the accusation-road freeze, the glowing win's reopen proof, the doors again); nine Appendix D rows brought current; the document at 424, the step table (488 rows) and the coverage map (134 rows) machine-verified at zero mismatches; the finding that NO ending's survival had been proved anywhere before; the conduct docs split (test-spec-styling.md spec-only, chat rules solely in CLAUDE.md); the rule-1 two-button opening drafted and paused; the pending cleanup set as #151's goal.

## Next session's goal (#151, from #150)

**CLEAN UP pending.txt — the list is stale (Patrick's call,
#150).** Go through it with Patrick top to bottom, bring every
line current, and drop what is done or dead. #150 already
corrected the two blocks its own work touched (the header and the
test-doc standing note, plus the coverage-gaps item's removal);
the rest stands as sessions around #140 left it. When the txt is
settled, `pending.docx` is rebuilt from it and machine-checked
against it, as always.

**What may take the agenda instead.** Apple's answer on build
1.0 (2) may arrive and set its own — the release is MANUAL, so an
approval waits for Patrick. **The mistouching remainder is PARKED
by Patrick (#141)** and is not to be raised until he calls for it.
Also available: the paused rule-1 two-button opening edit, the
Feedback-modal bug question, the web-spec evaluation, the
narrow-width screens, the one-sentence stale comment at line 810,
and the step-by-step pipeline document.

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
(Patrick, #147). A commit text's first line must fit the summary
field — about 50 characters — with anything more handed as a
separate body below it (Patrick, #149). Patrick commits (this
repo and any project repos touched).
