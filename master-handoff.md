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

Patrick's opener line: "#NN — name. Read CLAUDE.md and the hand-off."
The where-things-stand report comes only after ALL the reading — both
folders, every named doc — never after the first folder alone
(Patrick, #154, correcting a mistake made a dozen times).

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

## Where things stand (updated 2026-08-03, MT#3 — the Mystery Tracker
docs restructured)

**MYSTERY TRACKER'S LIGHT THEME IS BUILT AND COMMITTED.** MT#1 laid the
warm daytime palette into `MysteryTracker.html` and MT#2 settled the
gridwork — the honey-gold turn column, the alternating bands gone from
both themes, the gridlines given their own variable, and the ✓/✕ tints
split per theme so the approved dark theme is frozen. Patrick confirmed
at MT#3 that MT#1 and MT#2 are both committed. Two subjects were scoped
and deliberately not built: the grid's cream field and the light chips
under the small marks. Full detail in `MysteryTracker/docs/handoff.md`.

**MT#3 RESTRUCTURED THAT PROJECT'S DOCS (2026-08-03).** Patrick's ruling:
these files are for Claude's use, not his — he reads a pending file to
orient himself to a project. The measure became the cost of the opening
read, which was 1,477 lines that morning. Mystery Tracker gained a
`build-history.md` for finished work, `PARKED-ITEMS.md` dropped to open
items only and is no longer read at a session opening, `handoff.md` fell
from 375 lines to about 120, and the project's working habits moved into
its own `CLAUDE.md`, which arrives without being fetched.

**THE SESSION OPENING CHANGES SHAPE (MT#3, Patrick's word).** App-Docs is
connected and read as before; then Claude ASKS Patrick which project the
session is in and sends the folder ask for it. The goal lives in the
project, not here, because Patrick runs three projects and the goal has
to stay flexible. This file is to narrow to four things — the projects
and their folders, one line of status each, what is true across all
three, and the loose ends belonging to no single project. **That trim is
NOT yet done, so App-Docs' `CLAUDE.md` rule 1 and this file still
describe the older opening.**


**MEMORY'S CHAIN IS RUNNING (#3-new, 2026-07-31).** Both
"What's Next" items are BUILT, and Patrick verified everything
on the phone through a full EAS build:

- every screen's header buttons are now 54-point circles, the
  labels trimmed to "Home", "+ Add", and "Back" at Patrick's
  word (Vault's "+ New" and To-Do's "New Task" became "+ Add"
  along the way),
- My Day and Pets Day items no longer require a time — the
  shared control gained an optional-time setting (spinners
  dulled at 12:00 PM, box empty, a "No time set" hint), and an
  item without a time shows just its label and gets no
  reminder,
and
- the two header fixes his Simulator test surfaced: the
  thirteen screens without edges={['top']} got it, plus 8
  points of bottom padding, all matching Home and Look Ahead
  (the old #62 taller-header decision reversed — settings.tsx's
  comment records it).

TypeScript came back clean after every piece. The code commit
is Patrick's, made in-session before the build. pending.txt now
carries three new "What's Next" items: Look Ahead's tile format
and its Snooze, the Timer tile's Stop/Continue button and log,
and the Vault restructuring's Home-to-Back change.

Quiet-file note (this one session only, per the amended rule):
docs/publishing.md gained a "Build steps" section at its end —
Patrick's EAS build-and-submit steps, in his own words.

The numbering rule, amended at session 0 and again at
#156 -> MT#0 (Patrick's word): there are THREE chains — bare
session numbers always mean the old shared chain; Memory's own
chain is written "#1-new, #2-new, …"; and Mystery Tracker's own
chain is written "MT#1, MT#2, …". No old reference is ever
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
- #2-new (2026-07-31): The three "What's Next" items built —
  gear to 32 (Patrick's hand), one-tap Log and counters in
  My Day / Pets Day, Shopping highlighting stopped and tiles
  thinned — TypeScript check clean, Patrick verified all in the
  Simulator and committed. reminder-audit.md deleted by Patrick.
  Two new items filed; the opener-note shape amended.
- #3-new (2026-07-31): Round header buttons on all fifteen
  screens (54-point circles, labels Home / + Add / Back) and
  optional times in My Day / Pets Day (control asleep at dulled
  12:00 PM, no reminder without a time); headers re-leveled with
  edges top and bottom padding after the Simulator test; all
  phone-verified through EAS and committed by Patrick. Three new
  items filed; publishing.md gained Build steps; status reports
  drop Mystery.
- #154 (2026-07-31): Mystery's Android branch opened and scoped —
  the road chosen is a signed APK downloadable from elyfont.com
  (wrapper ~150–250 lines of Kotlin, four to six sessions); the
  Play Store parked after Google's 12-tester/14-day gate was
  verified against eight phones counted; the /clues/ page and the
  iOS badge road mapped; elyfont.com fetched (web page reports
  Ver. 5.0, the mobile game absent); the home-card mis-description
  fixed live by Patrick.
- #155 (2026-08-01): The Android wrapper built, signed, and
  phone-proven in ONE session against #154's four-to-six estimate —
  shim faking Apple's bridge (Patrick's ruling: the HTML is never
  changed), all bridges exercised, two wrapper bugs fixed (ignored
  insets padding; the sixth column clipped by the 430-pixel column
  arithmetic — viewport pinned at 430 and scaled), the signing key
  made and kept in iCloud Drive → AndroidKeys, the APK installed on
  Patrick's phone by the real browser-download road, and Chrome's
  stale-cache lesson recorded for the download page.
- #156 -> MT#0 (2026-08-01): light theme scope iPhone & web — a
  scoping session that became the transition into a new chain.
  Patrick's palette direction set (warm oranges, yellows, tans,
  browns; headers still open), the #72 mirror-the-web rule excepted
  for the light theme, and the ORDER REVERSED — the web app first,
  the iPhone app after — on the code evidence that the web already
  has the theme apparatus and the iPhone app has none. Mystery
  Tracker given its own chain, `MT#N`. Three stale items cut from
  the hand-off's "Where things stand." Mystery Tracker's docs read
  for the first time in the new chain: paused since 2026-06-13, all
  committed, no must-do item, and two broken pointers found —
  `docs/session-start.md` does not exist, and the older commit notes
  still name `SESSION-HANDOFF.md`. Nothing built; no app code
  touched.

- MT#1 (2026-08-02): the light theme's palette BUILT in the web app —
  the amber page background reached by warming the light background
  toward the mobile header rather than adding a band, eight pale
  surfaces taken to tan and cream, the four category banners set to
  the mobile app's colors in both themes, the two bars above the grid
  turned into dark islands that borrow the dark theme's whole color
  set (which fixed the near-white game bar), the heading band turned
  cream with dark letters, the ✓/✕ cell tints softened and deepened,
  and the two turn tints made one soft blue. Six theme items parked as
  26–31; three filing repairs discussed and deliberately not built,
  parked as 32.

- MT#2 (2026-08-03): the light theme's GRIDWORK — the turn column taken
  from soft blue to a honey gold, the alternating row bands removed from
  both themes, the gridlines given their own `--grid-line` variable and
  strengthened twice, and the ✓/✕ tints brightened, thinned, ringed, the
  ✕ ring toned down, then split into per-theme variables so the dark
  theme's approved values are frozen. One road tried and rejected by
  Patrick (recoloring the cell border instead of ringing it). Two
  subjects scoped and not built — the grid's cream field and the light
  chips under the small marks — parked as 33, 34 and 35. Patrick asked
  for a docs-trimming session next.

- MT#3 (2026-08-03): Mystery Tracker's docs restructured, on Patrick's
  ruling that they exist for Claude's use and that the opening read is
  what needs to shrink. `build-history.md` created and given the closed
  section, the June commit notes, the MT#1/MT#2 session records and item
  6's built record; `PARKED-ITEMS.md` cut from 546 lines to 158 and
  dropped from the opening read; `handoff.md` rewritten around the
  app's current state; the project's own habits moved into its
  `CLAUDE.md`. The opening reshaped so Claude asks which project the
  session is in. Three pieces left for MT#4 — a pending file for
  Patrick, this file's trim, and the two `CLAUDE.md` files, which
  Patrick named as MT#4's goal.

## Next session's goal (from #3-new and MT#1)

**#4-NEW (MEMORY) — TAKE UP THE "WHAT'S NEXT" ITEMS.**
Patrick's word at #3-new: take up pending.txt's three "What's
Next" items — Look Ahead's tile format changed and its Snooze
changed or dropped; the Timer tile gaining a Stop (Pause) /
Continue (Go) button and a log; and the Vault restructuring's
"Home"-to-"Back" button change. Each is a code change; scope
them together at the session start.

**MT#4 (MYSTERY TRACKER — WEB) — THE TWO `CLAUDE.md` FILES.**
Patrick's word at MT#3. They are 207 lines together and are the only
real weight left at a session opening. App-Docs' rule 1 also still
describes the old opening and needs bringing into line. Riding with it,
by MT#3's own list: a pending file for Patrick in Memory's shape, and
this hand-off's trim to its four things.

**Waiting behind that:** the grid's cream field, parked as item 33 —
the piece MT#2 stopped mid-question on. The color was never chosen, and
deepening it is the lever that would fix item 35. Also open from the
light theme: items 26, 28, 29, 31 and 34. Item 27 stays Patrick's word
for its own session, being app behavior rather than color.


Two things to remember: `DEPLOY.md` says the live site is served
from a DIFFERENT public repo (`WWhiteWolf/mystery-tracker`) so a
private-repo commit changes nothing anyone can see, and Patrick's
browser is Firefox — hard-reload with Cmd+Shift+R after every edit
or the old file gets served. Whether a palette change touches the
spec and its docx is still UNDECIDED.

**Waiting behind it:** the Android road's remaining legs — the APK
upload to the public mystery-tracker repo and the elyfont.com
download page (with its version note; a versioned filename
sidesteps Chrome's cache; bump versionCode first), and the
Android testing-depth call. Also the MCTS stale/dead HTML cleanup —
the three "What's next" items in
MysteryCluesTracker/docs/pending.txt, each a code change, sitting
naturally after the app reaches the store. Apple's answer on
build 1.0 (2) may set its own agenda when it comes. And the light
theme's second half — carrying the settled palette into the iPhone
app, which first needs its sixty-six literal colors pulled into
named variables before any light color can be looked at there.

The opener note is handed to Patrick in chat at session end —
not stored here (Patrick, #124).

## Loose ends

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
  unlinked from the home page). Deferred by Patrick, #130. The home
  card's book-reading mis-description that once paired with this was
  fixed live by Patrick at #154; this card item now stands alone.

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
hand-off." — before anything else (Patrick, #149; the "then tell
me where things stand" tail moved out of the first line at #154 —
it closes the folder-ask paragraph instead, after the second
folder's reading). The note itself must carry the cold start.
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
