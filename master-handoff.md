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

## Where things stand (updated 2026-07-22, session #120 — the game of minimums settled; the Guide cleared for variants)

**#120 was docs only — no code touched, the phone current as of
#115, the script and docx untouched at 258. The GAME OF
MINIMUMS was drafted, marked, and SETTLED at 19 steps into
MysteryCluesTracker/docs/s27-draft.md — NOT yet phone-run. Its
fiction is the official two-player Clue variant (Patrick's
reference), with a fixed deal: the envelope holds Card 4 and
Extra 3, the side pile holds Card 6, Card 7, Card 9, and
Extra 2, and Ann holds Card 5, Card 8, and Extra 1. A 36-step
fully-authentic version was weighed and set aside for
repetition; the drill shape won, then grew by Patrick's marks
— the 🏠 peek, the second-`?` re-ask, and the ∑ ⭐ finale,
each a first for the spec. DECIDED: both closing games get
face-up appendix entries, and §27 becomes FOUR numbered
sections at build time (Block 1, Block 2, the two-player
two-category game, the shrinking game). The Guide was read end
to end against optional variants — nothing rules them out; two
wordings were settled for a later code session, plus a
smarter-messaging item (pending.txt items 6–7). Detail:
build-history.md #120.**

Still open: the minimums game's PHONE RUN and the big
shrinking game's drafting — NEXT, #121; the invisible-message
find's placement; the Feedback-modal bug question (noted #111,
session-sized); the web-spec evaluation (#87); the test-spec
index (#119). Small and parked: the "Every other cell is
clean" gloss in 24.x/25.11 (Patrick: stays parked); the docx
message-font distinction (a build-script styling discussion);
the docx zoom quirk (#114).

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
- #115 (2026-07-20): PANEL WAKE built and phone-proven — nine landings, lastScreen in the snapshot, the #98 Notes→Guide settlement, the Feedback-modal close ruled Apple-consistent, and the boot-order ▶ Play leak (Patrick's phone find) guarded to Setup-only.
- #116 (2026-07-20): the spec rewrite — §25 → the 19-step reopen walk, 22.25–26 merged; the docx at 258; the game-behind-Setup landing ruled unstageable (eight reachable); docs only, no code.
- #117 (2026-07-20): the §27 ground settled — the harvest re-verified against code AND all 258 steps; sixteen tests + walking order agreed; clearAllPlayers and the popup fallbacks dropped (dead/unreachable); the after-the-3rd find; appendix corrected; docs only, no code.
- #118 (2026-07-20): §27 Blocks 1–2 drafted in chat — Block 1 (30 steps) marked and SETTLED, Block 2 (25) unmarked, in docs/s27-draft.md; two phone proofs (marquee scrolls; empty Confirm silent — the invisible-message find); chat-style rules into test-spec-styling.md; docs only, no code.
- #119 (2026-07-21): §27 Block 2 marked, phone-run, and SETTLED; the two closing games DECIDED (the game of minimums, then the big shrinking game); pending.txt refreshed; rule 0 (no shorthand) into both CLAUDE.md files; docs only, no code. (Three deleted session starts preceded it; files unharmed.)
- #120 (2026-07-22): the game of minimums SETTLED at 19 steps on the two-player Clue-variant fiction (not yet phone-run); the appendix entries and the four-section split DECIDED; the Guide cleared for optional variants, two wordings settled for later; docs only, no code.

## Next session's goal (#121, from #120)

**RUN the game of minimums on the phone (19 steps, in
MysteryCluesTracker/docs/s27-draft.md — Patrick's phone
already stands at its start, Block 2's end state) and settle
what the run teaches back into the draft. Then DRAFT the big
shrinking game (6 players, 4 categories, 30 cards, 👋-quitting
players one at a time to prove every count down to two) — it
needs its own staging steps and names for the two new seats.
When all of §27 settles: into build-mcts-test.js on Patrick's
go — plus the §19 two-step addition in the draft file —
regenerate the docx, verify row-for-row, delete s27-draft.md.
At build time §27 becomes FOUR numbered sections and both
closing games get face-up appendix entries (#120).** Also
still open: the invisible "Select a card" find's placement
(pending.docx candidate); the Feedback-modal bug question
(noted #111, session-sized); the web-spec evaluation (#87);
the test-spec index (Patrick, #119 — pending.txt item 2); the
two Guide wordings and the smarter-messaging item (#120 —
pending.txt items 6–7, code changes for their own session).

Opener note for Patrick to paste into #121:

"MCTS #121 — phone-run the game of minimums, then draft the
big shrinking game. Connect App-Docs and MysteryCluesTracker.
Read both CLAUDE.md files (note rule 0: no shorthand or jargon
— full sentences), session-start, the master hand-off,
docs/test-spec-styling.md, docs/s27-draft.md (Blocks 1–2 and
the game of minimums are settled — the minimums game is NOT
yet phone-run; its deal and the build-time decisions sit at
the file's top), and build-history.md's #120 section. Verify
every wording against mystery-clues-tracker.html — never from
memory. My phone stands at Block 2's end state, ready for the
minimums game's step 1. What the run teaches goes back into
the draft on my marks. Then the shrinking game gets discussed
and drafted on my 'Go?'. No code changes expected. One change
at a time; I do all commits."

## Commit status: Patrick's commits, when ready

From #120 — MysteryCluesTracker: docs/s27-draft.md (the
settled game of minimums, its deal, and the build-time
decisions; the Open list retitled for #121), docs/pending.txt
(items 6–7 added; item 1 and the standing notes refreshed),
docs/build-history.md (the #120 section). App-Docs:
master-handoff.md (this refresh). Neither CLAUDE.md was
touched this session. The script and docx were NOT touched in
#120 — still the #116 versions at 258. pending.docx untouched
(the new find's placement is Patrick's to decide). Earlier
sets possibly still uncommitted (#112–#119 files) — confirm
with Patrick.

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
