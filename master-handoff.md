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
   Project: `Projects/elderlyassistant` (its CLAUDE.md names the
   reading order: this hand-off, then docs/build-history.md). Store
   prep after the Mystery rehearsal; Android eventually (#72).
4. **Memory — web** — DROPPED (#72). elyfont.com gets a pointer to the
   App Store listing only.

## Where things stand (updated 2026-07-30, #1-new — Memory's chain
begun: "What's Next" filled and the pending list tidied)

**MYSTERY IS SET DOWN AND UNCHANGED (#152).** The app is with
Apple: build **1.0 (2)**, status **Waiting for Review**, release
setting **MANUAL** — an approval waits for Patrick. Nothing in App
Store Connect lives in a repo, so this is the only record. Its docs
are current and tidy; the stale/dead HTML cleanup waits for the
store.

**MEMORY'S CHAIN IS RUNNING (#1-new, 2026-07-30).** The chain's
first working session filled pending.txt's "What's Next" with
three items, Patrick's word:

- the Home screen's Settings gear in symmetry with the logo,
- the My Day / Pets Day counters losing the log pop-up — editing
  happens in the log itself,
and
- the Shopping List's Shopping-mode highlighting stopped and the
  tiles made thinner.

The list got a deep tidy besides: the five-piece Parked bullet
dissolved (the reminder test checklist passed in full and the
My Week done-date fix confirmed — both recorded in Memory's
build-history — the exact-item tap routing re-homed to Parked,
the dark startup flash to Decisions), the "Memory Assist"
subtitle item re-homed by Patrick's hand to docs/publishing.md,
and two items deleted outright. pending.docx was rebuilt from the
txt and machine-checked word for word (548 words each side, zero
mismatches). The #69 badge-reorder loose end closed — finished,
built, and phone-verified.

Quiet-file notes (this one session only, per the amended rule):
docs/publishing.md now carries the App Store subtitle item, added
by Patrick's hand at #1-new. Memory's CLAUDE.md was amended at
Patrick's word — the quiet files are "quiet until needed," and
any change to one is noted here for the next one session only.

The numbering rule, amended at session 0 (Patrick's word): bare
session numbers always mean the old shared chain; Memory's own
chain is written "#1-new, #2-new, …" — no old reference is ever
edited. The name is "A Place To Remember"; the badge under the
icon is "Memory". Memory runs in its own chat stream.

**STILL OPEN:** the Cowork "Projects" feature — explored, then
parked by Patrick: an accidental "App-Docs" project sits harmless
in the app's Projects panel, and whether a chat inside a project
can connect a second folder is untested.

Standing habits and notes: after any HTML change, re-copy into the
wrapper's www/ and verify the copy matches exactly. Old/saved games
don't exist and don't matter — no migration concerns, ever (#75).
The free script doubles as the paid tier's future answer key (#90).
The paid-tier design/build (upgrade-scope.md "Decided — session #76")
waits until the free product is finished. The App Store listing name
question is settled and the name is registered (#129) — see
MysteryCluesTracker/docs/ROADMAP.md.

## Session history

The full history lives in `MysteryCluesTracker/docs/build-history.md`.
Every section heading there carries its session number, its date and a
one-line summary of what happened — so the list of headings IS the
index. Read those when something needs finding, rather than keeping a
copy here.

Kept here only while they still bear on live work:

- #151 (2026-07-29): THE COLD-START OPENING WRITTEN — CLAUDE.md rule 1 rewritten twice (the second folder left unnamed so the rule serves every project, which put the hand-off read BEFORE the second folder ask), and the hand-off's "At session end" given the passage that makes every opener note carry the folder asks; the "only carrier" claim dropped after CLAUDE.md's text proved to arrive before any folder is connected. The pending list cleaned top to bottom: "What's next" from five items to three all-code ones, "Nice-to-have later" from eight bullets to three, the web app's stray Clue echo rehomed to MysteryTracker's PARKED-ITEMS.md as item 25, the header rewritten to describe this session, 252 lines down to 158. pending.docx deferred by Patrick. Patrick made several of the edits by hand, and flagged that each read of a file needs its own ask.
- #152 (2026-07-29): A scare about the styling docs settled by git
  archaeology — chat&test-spec-styling.md recovered, the #150 split
  proved clean, nothing lost. The pending tidy finished: two sections
  dropped whole, 85 lines, header rewritten; pending.docx rebuilt and
  machine-checked at zero mismatches. Project set down until the app
  is in the store; next: prepare the transition to Memory — the
  HTML cleanup waits for the store.
- 153 > 0 (2026-07-30): The Memory transition session, the bridge
  between the chains. Memory's pending.txt part-tidied (snapshot and
  #40/#41 tombstones out, three sections emptied, Vault import
  re-homed to Parked); the file map settled (mirror Mystery's
  shapes, no project hand-off, old files quiet in place, nothing
  deleted); the numbering rule fixed (bare = old chain, "new#" =
  Memory's new chain); the name settled ("A Place To Remember",
  badge "Memory"); Cowork Projects explored and parked.
- 0 (2026-07-30): The Memory carpentry, all four pieces on their
  own gos — CLAUDE.md to the short-pointer shape; build-history.md
  created, first entry the transition record; pending.txt's header
  and title line finished; pending.docx decided and built,
  machine-checked at zero mismatches. The numbering style amended
  to "#1-new" at Patrick's word. Memory's chain begins at #1-new.
- #1-new (2026-07-30): Memory's chain begun — "What's Next" filled
  with three items (gear symmetry, counters without the log
  pop-up, Shopping List highlighting and tiles); the five-piece
  Parked bullet dissolved, two pieces recorded done; the subtitle
  item re-homed to publishing.md; the quiet-files rule amended to
  "quiet until needed" with one-session notes; the pending header
  now updated at every refresh; pending.docx rebuilt at zero
  mismatches; the #69 badge-reorder loose end closed.

## Next session's goal (from #1-new)

**#2-NEW — WORK THE "WHAT'S NEXT" ITEMS.** Patrick's word at
#1-new: take up pending.txt's three "What's Next" items — the
Home screen's Settings gear in symmetry with the logo; the
My Day / Pets Day counters editing in the log instead of the log
pop-up; and the Shopping List's highlighting stopped in Shopping
mode with thinner tiles. Each is a code change; scope them
together at the session start.

**Waiting behind it:** the MCTS stale/dead HTML cleanup — the three
"What's next" items in MysteryCluesTracker/docs/pending.txt, each a
code change, sitting naturally after the app reaches the store.
Apple's answer on build 1.0 (2) may set its own agenda when it
comes.

The opener note is handed to Patrick in chat at session end —
not stored here (Patrick, #124).

## Loose ends

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

If pending.txt changed, its header line is brought up to date
first — every time (Patrick, #1-new) — then pending.docx is
rebuilt from it to match, machine-checked line-for-line
(Patrick, #128).
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
