# Master hand-off — the one session chain (all projects)

**This folder (Projects → App-Docs) is the single home for cross-project
docs — Patrick's decision, session #71 (2026-07-09): everything in one
folder, backed up and version-controlled (this folder is a git repo;
Patrick does all commits).**

**KEEP THIS FILE TRIM (Patrick, #97).** Only the CURRENT state is
written out in full. Each finished session gets ONE line in the history
index below — its full detail lives in the active project's own docs
(for the mobile app: `MysteryCluesTracker/docs/upgrade-scope.md`).
At the session-end refresh, fold the closing session into one index
line and rewrite "Where things stand" in place — never let per-session
paragraphs accumulate here. Git holds every old version of this file.

## How a session starts

1. Patrick connects **Projects → App-Docs** (this folder) and says read
   the master hand-off.
2. Claude reads this file, then `Publishing-Strategy.docx` (the north
   star: strategy, standing rules, the four products, the learning
   tracker) if the session is publishing/business-side.
3. Claude connects whichever project folder the session's goal lives in
   and reads THAT project's own docs (each app keeps its own material).
4. Patrick names ONE goal; scope it together; Claude waits for his "go."

Patrick's opener line: "#NN — name. Read CLAUDE.md, session-start.md,
and the hand-off, then tell me where things stand."

## Standing rules (short form — the full set is in the strategy doc and elderlyassistant/docs/session-start.md)

- Patrick does ALL git commits. Claude runs NO git commands at all in
  Patrick's repos — in #71 even a read-only `git status` left index.lock
  files behind that would have blocked his commits. Look at files
  directly instead.
- One step at a time; discuss before building; wait for the go — a go
  exists only after Claude asks "Go?" as its own question and Patrick
  answers it (#88).
- Verify before asserting — read the actual code/files, don't guess.
- One question at a time; genuinely open questions — no boxed
  choices, no "X or Y?" questions.
- Never give click-directions for a screen Claude can't see.
- Patrick leads; Claude doesn't steer. No urgency — his pace. He's
  retired; this is a hobby — no deadlines, no clerk-abrupt tone; warm
  and conversational. Not wasteful of his time, but never hurried.
  Patrick lives alone; Claude's tone is sometimes the only
  conversation he gets all day — it matters. The conversation is
  part of the work, not overhead.

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

## Where things stand (updated 2026-07-20, session #114 — the Welcome Back removal BUILT and phone-verified; PANEL WAKE decided, not built)

**#114 closed its goal: the Welcome Back removal is BUILT to
the #113 scope and fully verified — Firefox and Chrome
(Patrick), the wrapper's www/ copy diff-verified, the Xcode
build done, and the phone walk clean: from both Setup and Game,
after a simple close, a phone lock, and a power cycle, the app
wakes silently, exactly as left. One find rode along, judged
in-scope: startNewGame carried a closeModal('modalWelcome')
that would have crashed New Game once the modal div was gone —
removed with the rest. firstLaunch is now written but never
read; Patrick ruled it stays for now. The edge-seam pending
item is believed closed by the removal — not separately
re-tested. The phone is CURRENT.**

**PANEL WAKE is DECIDED (Patrick, #114) — NOT built: the app
will wake exactly where it was closed, the three side pages
(Log, Notes, Guide) included. Research-backed (Apple's
state-restoration guidance, NN/g's interruption research,
platform practice — Mail/Notes/Books). Entry and build sketch
in upgrade-scope.md: snapshot on panel opens, persist
lastScreen, loadState's landings grow to nine (first launch
untouched), the parked Notes→Guide quirk (#98) gets settled on
the way. Order settled by Patrick (#114): code first, THEN the
spec — the §25 / 22.25–26 rewrite follows the panel-wake
build.**

Still open: the Feedback-modal bug question (noted #111,
session-sized); the web-spec evaluation (#87); §27 drafting,
harvest in hand. Small and parked: seven docx files got an
in-file zoom of 125% (#114), but Patrick's opening app ignores
the saved setting and the files' own font sizes differ —
revisit some other time.

Standing habits and notes: after any HTML change, re-copy into the
wrapper's www/ and verify the copy matches exactly. Old/saved games
don't exist and don't matter — no migration concerns, ever (#75).
The free script doubles as the paid tier's future answer key (#90).
The paid-tier design/build (upgrade-scope.md "Decided — session #76")
waits until the free product is finished. At listing time: confirm
"Mystery Clues Track Sheet" is available.

## Session history index (detail: the matching section in MysteryCluesTracker/docs/build-history.md)

- #71 (2026-07-09): App-Docs becomes the one docs home; strategy set; the four products named.
- #72 (2026-07-10): Memory-web dropped; mobile mechanical cleanup done; the full design scope completed.
- #73 (2026-07-10): The Setup build done, Patrick-verified in-browser.
- #74 (2026-07-10): The game play build done — tier gate out, deductions out, Player Out's two models, the 🏠 column.
- #75 (2026-07-11): The catch-up session — all seven items closed.
- #76 (2026-07-11): The two-tier scope decided — free = today's app; paid = the web's seven helpers.
- #77 (2026-07-11): The Guide editing pass done; the 💬 feedback mailto bug found and fixed.
- #78 (2026-07-12): Renamed "Mystery Clues Track Sheet"; dictation-comes-free amended; disclaimer settled.
- #79 (2026-07-12): The wrapper started; the real app ran in the simulator; the fonts problem opened.
- #80 (2026-07-12): Native-vs-wrapper SETTLED — stays a wrapper; #79 commits done; conduct rules 7–8 written.
- #81 (2026-07-12): The www folder-reference fix — fonts load; the hand-quick-steps-to-Patrick rule.
- #82 (2026-07-12): The data-safety bridge built and half-proven; the dead-Next bug opened.
- #83 (2026-07-13): Dead-Next closed (an invisible warning); message outlets on every screen; Log Copy fixed; the bridge fully proven.
- #84 (2026-07-13): Dressing 2/3 — home-screen name, app icon, the header emblem.
- #85 (2026-07-13): Dressing 3/3 — iPhone-only, portrait lock; the deleted-target incident cleanly recovered.
- #86 (2026-07-13): The real-device check — the app runs on Patrick's iPhone; three phone finds fixed; quirk queue empty.
- #87 (2026-07-14): pending.txt created; the web test doc evaluated — the format transfers.
- #88 (2026-07-14): The mobile test doc begun — §1–5 (53 steps); the cast decided; the "Go?" rule.
- #89 (2026-07-14): §6–7 written — setup coverage closed (71 steps); the player-popup Clear fix.
- #90 (2026-07-14): The scripted game designed (21-card deck, the family deal, eight turns); §8 built (83 steps).
- #91 (2026-07-15): Appendix A + turns T1–T4 as §9–12 (107 steps).
- #92 (2026-07-15): The guard turns §13–16 — the scripted game complete in the doc (138 steps).
- #93 (2026-07-15): Both #92 code items closed — the hint line and the message wording.
- #94 (2026-07-15): §17–19 written (163 steps); the five #93 wording alignments.
- #95 (2026-07-16): §20–21 written (180 steps); the Notepad status strip; Undo now logged — honest history.
- #96 (2026-07-16): Warnings white + the Setup strip black-on-gold; the duplication item moved to #97.
- #97 (2026-07-16): The doc trim + the message dedup + the ✓ title; died on a 529 crash — committed, undocumented until #98.
- #98 (2026-07-16): The spec catch-up (13 wordings) + four phone fixes (Play-in-Guide, the mailto bridge, the header, out-of-turn taps) — all phone-verified; the phone is current.
- #99 (2026-07-17): §22 Player Out drafted, settled, and phone-run (26 steps, in s22-draft.md — not yet in the script) + two phone-found fixes built and verified same-night: in-modal messages, the readable quit header.
- #100 (2026-07-17): §22 dropped in — the docx at 206 steps, row-for-row verified; test-spec-styling.md created; §23 drafted and partly phone-run, not settled; ended on a go-rule breach.
- #101–#102 (2026-07-16/17, cloud): run in the cloud by accident (≈15% Fable usage burned); the #100 docs refresh recovered and written; the §23 draft stayed chat-only and was lost with the cloud scroll-back; detail thin, honestly marked.
- #103 (2026-07-17): §23 reconstructed at 15 steps (s23-draft.md); four modals given message lines, phone-verified; spec: ⚠ precaution, computed step count (206), 3.8/3.9/5.7/18.6 enriched, "The bottom strip shows:" convention; phone fresh-installed — game state to rebuild.
- #104 (2026-07-17): §23 run (15/15 pass), settled, into the script — the docx at 221; the lettering find pinned (the Log's empty-state line); the reopen bug logged; both drafts deleted.
- #105 (2026-07-18): pending.txt trimmed to glance-length; §24 drafted spec-first into s24-draft.md; the Feedback-modal redesign decided; the reopen bug grown; the deck decoupling decided.
- #106 (2026-07-18): the Feedback modal rebuilt to spec and phone-verified; §24 run 15/15 and into the script — the docx at 236; rule 10 (ask, don't assume) into both CLAUDE.md files.
- #107 (2026-07-18): the reopen bug diagnosed (three Setup-side mechanisms; mid-game path phone-proven good); the quit-clamp bug and the buried-direction spec fix found by Patrick's own testing; the phone staged with the §22 end-state; docs only, no code.
- #108 (2026-07-18): the reopen bug FIXED — the ONE Welcome Back modal built (status lines, greyed picks, two-tap Continue/Done), the deck decoupled (mctDeck), the New Game modal reworked, picks now save; pending 1/3/4 closed, browser- and phone-verified; two new finds logged (Cancel/Close, the fresh-install seam).
- #109 (2026-07-19): the sibling modals designed and built (Cancel/Close, return-as-left restore, the two no-move fixes) — browser-verified, phone built; §25 drafted (s25-draft.md), not run; ended on a staging muddle — the phone's state unconfirmed.
- #110 (2026-07-19): §25 settled and into the script (258); the wordings sweep + the buried directions — the docx at 259; the Guide's New section rewritten (awaits the Xcode build); the draft deleted.
- #111 (2026-07-19): §26 settled, phone-proven, and into the script — the docx at 262; the quit road's two pointer fixes; the Log line and ∑ ✕ restyles; the Xcode build done — the phone current, all eye-checked.
- #112 (2026-07-19): the function appendix built and verified (108 functions, coverage map, §27 harvest); the 1.9 find; the Welcome Back modal removal DECIDED, ledger in upgrade-scope.md — nothing built, no code touched.
- #113 (2026-07-20): the New Game modal SETTLED (nothing changes; no new fresh-start road); the Welcome Back removal SCOPED into upgrade-scope.md from a fresh code read; build sized as a dedicated session — docs only, no code touched.
- #114 (2026-07-20): the Welcome Back removal BUILT and phone-verified (close, lock, power cycle — both rooms); the startNewGame crash find removed in-scope; PANEL WAKE decided (research-backed), code-then-spec order set; seven docx zoomed 125% in-file (opening app ignores it — parked).

## Next session's goal (#115, from #114 — sized with Patrick)

**BUILD PANEL WAKE: the app wakes exactly where it was closed —
Log, Notes, and Guide included (upgrade-scope.md, the #114
panel-wake entry). Snapshot on panel opens and the roads out,
persist lastScreen in the mctGame record, grow loadState's
landings to nine (first launch untouched), settle the parked
Notes→Guide lastScreen quirk (#98) on the way; verify all nine
landings in browser and on the phone; wrapper www/ re-copy;
Xcode build.** THEN the spec: §25 / 22.25–26 rewritten once,
against the final reopen behavior (Patrick, #114: code first,
then spec and docs). Also still open: the Feedback-modal bug
question (noted #111, session-sized), the web-spec evaluation
(#87), and §27 drafting (harvest in hand).

## Commit status: Patrick's commits, when ready

Possibly still uncommitted from #112/#113 — confirm with
Patrick: docs/mcts-function-appendix.md (NEW), the #112–#113
refresh sets, pending.txt deletion after commit. From #114,
MysteryCluesTracker: mystery-clues-tracker.html (the removal),
wrapper .../www/mystery-clues-tracker.html (the diff-verified
copy), docs/upgrade-scope.md (removal marked built + the
panel-wake entry), docs/build-history.md (the #114 section),
docs/pending.docx (refreshed + re-zoomed), and zoom-only
touches to docs/mcts-master-test.docx and
docs/mct-checklist-appendix.docx. App-Docs: master-handoff.md
(this refresh), plus zoom-only touches to
Publishing-Strategy.docx, My-Tools-and-Extensions.docx,
mtr-master-test.docx, mtr-master-test-v2.docx.

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

## At session end

Claude refreshes this file — "Where things stand" rewritten in place,
the finished session folded into ONE history-index line — plus the
strategy doc's "Next session — start here" note and the active
project's own docs. The refresh is discussed and gets Patrick's go
like any other change (#79). Claude also scripts a short opener note
for Patrick to paste into the next session — goal, what's decided,
the reading list, and the working rules — as part of the refresh
(Patrick, #114). Patrick commits (this repo and any project repos
touched).
