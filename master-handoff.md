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

## Where things stand (updated 2026-07-29, session #151 — the cold-start opening written into rule 1 and the hand-off, and the pending list cut from 252 lines to 158)

**THE APP IS WITH APPLE.** Build **1.0 (2)**, status **Waiting for
Review**, release setting **MANUAL** — so an approval waits for
Patrick rather than putting the app on the store by itself. No word
from Apple as of #143. Nothing in App Store Connect lives in a repo,
so this is the only record.

**THE TEST DOCUMENT IS FINISHED AND PROVED (#150).** 424 steps,
§1–31, with §27 at 36 and §31 at 31. Every edit was regenerated from
an exact copy of the script and machine-verified — the step table's
488 rows and the coverage map's 134 rows both at zero mismatches.
Full detail: build-history.md #150.

**THE OPENING PROCEDURE IS WRITTEN (#151).** The edit paused at #150
is done. CLAUDE.md rule 1 now says to ask through the
folder-permission button for App-Docs, read it and this hand-off, let
this file name the project the goal lives in, ask the same way for
that folder, read its docs, and give ONE status report after all the
reading. No project folder is named there, so the rule serves every
product. The "At session end" section carries the matching passage
for the opener note, which DOES name the real folder — at session end
the next project is known. Corrected in passing: CLAUDE.md's own text
reaches Claude before any folder is connected; only the files inside
the folders are out of reach.

**THE PENDING LIST IS HALF TIDIED (#151).** pending.txt went from 252
lines to 158. "What's next" now holds three items, all of them stale
or dead code: the line-810 comment, the #80 dust list, and the six
bits of leftover code. "Nice-to-have later" holds three: the pipeline
document, the Notepad Guide button, and the Capitalize item. Dropped
as dead at Patrick's word: the web-spec evaluation (its App-Docs path
died at #129 — the spec lives at
MysteryTracker/docs/MysteryTracker-spec.md), the mistouching item,
the Feedback-modal bug question, the narrow-width screens, the
grid-clip caveat, and the elyfont.com home-page bullet, that last one
surviving under "Loose ends" below. The web app's stray Clue echo was
rehomed to MysteryTracker/docs/PARKED-ITEMS.md as item 25 before its
bullet went.

**A WORKING NOTE (#149).** Patrick said plainly that he could not
track renumbering in his head, and a plain numbered list of the
section's Do cells fixed it at once. When a section's numbers shift
under him, print the list without being asked.

Still open: **pending.docx no longer matches pending.txt.** Patrick
deferred the rebuild, and the standing rule is that the docx is
rebuilt from the txt and machine-checked whenever the txt changes, so
it rides with #152's goal. The rest of pending.txt still wants a
going-over — "Where things stand right now" (ten bullets, several of
them still calling #140 "this session"), "At listing time", and
"Waiting on purpose". The mistouching remainder stays **parked by
Patrick** (#141): the phone's Touch Accommodations settings, a
visible pressed state and taller rows are not to be raised again
until he calls for them.

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

- #151 (2026-07-29): THE COLD-START OPENING WRITTEN — CLAUDE.md rule 1 rewritten twice (the second folder left unnamed so the rule serves every project, which put the hand-off read BEFORE the second folder ask), and the hand-off's "At session end" given the passage that makes every opener note carry the folder asks; the "only carrier" claim dropped after CLAUDE.md's text proved to arrive before any folder is connected. The pending list cleaned top to bottom: "What's next" from five items to three all-code ones, "Nice-to-have later" from eight bullets to three, the web app's stray Clue echo rehomed to MysteryTracker's PARKED-ITEMS.md as item 25, the header rewritten to describe this session, 252 lines down to 158. pending.docx deferred by Patrick. Patrick made several of the edits by hand, and flagged that each read of a file needs its own ask.

## Next session's goal (#152, from #151)

**FINISH THE PENDING TIDY, THEN REBUILD pending.docx.** Three
sections have not been through it: "Where things stand right now"
(ten bullets, several still speaking of #140 as "this session"), "At
listing time", and "Waiting on purpose". When the txt is settled,
pending.docx is rebuilt from it and machine-checked line-for-line, as
always.

**What may take the agenda instead.** Apple's answer on build
1.0 (2) may arrive and set its own — the release is MANUAL, so an
approval waits for Patrick. **The mistouching remainder is PARKED
by Patrick (#141)** and is not to be raised until he calls for it.
Available once the tidy is done: all three items in "What's next" —
the line-810 comment, the #80 dust list and the six bits of leftover
code — bearing in mind that each is a code change, meaning a new
version number and a fresh submission while 1.0 (2) sits with Apple.

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
else (Patrick, #149). The note itself must carry the cold start.
It opens with the folder asks in rule 1's order —
`Projects/App-Docs` through the folder-permission button first,
then the project folder the next session's goal lives in, named
outright rather than left to a guess — and ONE status report
after all the reading, never one per folder; then it closes with
a one-line summary of the working rules. A fresh session holds
nothing but the paste until the first folder is connected: the
conduct rules in `App-Docs/CLAUDE.md` arrive on their own, but no
file in any folder can be opened, so the note has to carry the
opening itself (proved at #151's opening; Patrick, #150/#151).
Every session-end note is built to that shape.
The note is handed as its OWN message,
separate from the refresh report — folded into a long report
it gets missed (Patrick, #150). Claude also drafts a commit text for each
repo touched, handed in chat beside the opener note
(Patrick, #147). A commit text's first line must fit the summary
field — about 50 characters — with anything more handed as a
separate body below it (Patrick, #149). Patrick commits (this
repo and any project repos touched).
