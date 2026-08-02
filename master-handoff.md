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

## Where things stand (updated 2026-08-01, #156 -> MT#0 — the light
theme scoped, the order reversed to the web first, Mystery Tracker
given its own chain)

**THE LIGHT THEME IS SCOPED, AND THE ORDER IS REVERSED
(#156 -> MT#0, 2026-08-01).** Patrick's direction is a warm daytime
look — oranges, yellows, tans, browns — NOT the cold white kind, and
NOT the web app's existing light theme, which he does not like. That
excepts the light theme from the #72 mirror-the-web rule; the rule
stands everywhere else. Still OPEN: whether the headers hold their
present colors or shift to blend with a lighter grid. The palette now
gets designed in the WEB app first and the iPhone app follows later,
because the web already carries the apparatus — a dark `:root` and a
`:root.light` under the same variable names, plus a no-flash script —
while the iPhone app has no theme switch at all and about sixty-six
literal colors sitting outside its thirteen variables. Mystery Tracker
also gained its own numbering chain, `MT#N`, and MT#1 is the first
real session in it. Nothing was built and no app code was touched;
full detail in build-history.md's `#156 -> MT#0` section.

**MYSTERY'S ANDROID WRAPPER IS BUILT, SIGNED, AND PHONE-PROVEN
(#155, 2026-08-01).** *(This paragraph rides one more refresh at
Patrick's word, #156 -> MT#0, then goes.)* The
wrapper #154 scoped at four to six sessions took one: Android
Studio (Quail 3) on the Mac, the project at
`MysteryCluesTracker/wrapper-android` (package
com.elyfont.mysteryclues, Kotlin, minimum API 26), one
MainActivity.kt whose injected shim fakes Apple's bridge object —
Patrick's ruling: the game HTML is NEVER changed; the wrapper
adapts. All three bridges were exercised on the emulator; storage
and clipboard proven again on Patrick's own Android phone; the
mailto compose half waits for a phone with email configured. Two
wrapper bugs found and fixed along the way: WebView ignoring its
own inset padding (a container carries it now), and the sixth
player column clipped — the sheet's columns total exactly 430 CSS
pixels, wider than most Android screens, so the wrapper pins the
viewport at 430 and scales the page down whole. The signing key
lives at iCloud Drive → AndroidKeys (alias mystery; passwords in
Patrick's paper notes; the key must never enter a repo, and every
future update needs it). `app-release.apk` reached the phone by
the real elyfont.com road — browser download over Wi-Fi,
unknown-source walk, install. One lesson for the download page:
Chrome re-served its stale cached APK until history was cleared,
so the page wants a version note, a versioned filename would
sidestep the cache, and the next release build should bump
versionCode. Still ahead: the elyfont.com upload and download
page, the testing-depth call (424 steps on Android is Patrick's,
undecided), and the /clues/ page question. The stale/dead HTML
cleanup still waits for the store. Amendment note (standing from
#154): how the #3-new no-Mystery-in-status-reports ruling applies
now the branch is live has not been re-discussed.

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

## Next session's goal (from #3-new and #156 -> MT#0)

**#4-NEW (MEMORY) — TAKE UP THE "WHAT'S NEXT" ITEMS.**
Patrick's word at #3-new: take up pending.txt's three "What's
Next" items — Look Ahead's tile format changed and its Snooze
changed or dropped; the Timer tile gaining a Stop (Pause) /
Continue (Go) button and a log; and the Vault restructuring's
"Home"-to-"Back" button change. Each is a code change; scope
them together at the session start.

**MT#1 (MYSTERY TRACKER — WEB) — THE LIGHT THEME, DESIGNED IN THE
WEB APP.** Patrick's word at #156 -> MT#0: the palette gets made
where it can be seen changing. Connect `Projects/MysteryTracker`
and read its `CLAUDE.md`, `docs/handoff.md` and `docs/ROADMAP.md`
— with the warning that the filing has drifted, so treat them as
how things were LEFT, not how they are. The direction is a warm
daytime look — oranges, yellows, tans, browns — and NOT the light
theme that file already carries, which Patrick does not like. Open
question to settle: whether the headers hold their present colors
or shift to blend with a lighter grid. The web's `:root.light`
block is where a candidate palette gets tried; parked item 24 (the
dead `--sum-dot-fg` variable, defined in both theme blocks and
referenced nowhere) is already a theme item and belongs in the
same pass. Two things to remember: `DEPLOY.md` says the live site
is served from a DIFFERENT public repo (`WWhiteWolf/mystery-tracker`)
so a private-repo commit changes nothing anyone can see, and
Patrick's browser is Firefox — hard-reload with Cmd+Shift+R after
every edit or the old file gets served. Whether a palette change
touches the spec and its docx is UNDECIDED.

**Repairs waiting in that project, deliberately not done at
#156 -> MT#0:** `docs/session-start.md` does not exist even though
the master hand-off and that project's own `CLAUDE.md` rule 1 both
name it as the first read, and the older commit notes in
`handoff.md` and `ROADMAP.md` still name `SESSION-HANDOFF.md`,
which became `docs/handoff.md`. Each wants its own discussion.

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
