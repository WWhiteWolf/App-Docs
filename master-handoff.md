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
4. Patrick names ONE goal; scope it together; Claude waits for his "go."

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

## Where things stand (updated 2026-07-28, session #145 — nothing built: 22.28's wording settled in chat, then the carry-over rule dropped for sections under rework — §22 to be rebuilt on a fresh setup)

**THE APP IS WITH APPLE AND CARRIES THE RIGHT CODE.** Build
**1.0 (2)** went back in at #140 after the version was pulled from
review; status at that session's end was **1.0 Waiting for Review**.
The release setting is **MANUAL**, so an approval waits for Patrick
rather than putting the app on the store by itself. Nothing in
App Store Connect lives in a repo, so the docs are the only record.
No word from Apple had arrived by the end of #143.

**THE TEST DOCUMENT NOW STANDS AT 405 STEPS, and §22 at 29.** #144
ran as a build session, earliest section forward, one step at a time
with Patrick's go on each change.

**§21 IS DONE — one cell.** 21.4's shower line gained its card
("Ann showed Card 2", read out of `logTurn` at 889 and its call site
at 2381); "its two detail lines" became the ONE line `renderLog`
draws for an Undo entry ("All Turn 7 marks removed.", line 947, the
only writer at 2421); and the screen text went into straight double
quotes per the #142 rule. **#143's notes had these two §21 items one
number low** — they are 21.4 and 21.5, not 21.5 and 21.6. The
findings were right; only the numbers were wrong.

**§22 "PLAYER OUT" IS REBUILT AS FAR AS ITS LOG STEP.** The opening
four steps came down to the modal's one door (markup 575–597,
refusal at 2478). **Ann now leaves by the ⭐ Accuse road at 22.5
through 22.10** — Patrick's own suggestion — because after #133 that
is the only road to a wrong-accusation exit, and that state is what
22.11, 22.16, 22.18, 22.20 and 22.29 all rest on. He also caught
that the first draft had dropped the arm-and-lapse, which is now
22.9. **22.20** moved the "already out" refusal to the ⭐ modal
(line 1748); the Out modal still LISTS a wrongly-accused player
wearing her 😢 (2446, 2460) and will let her be picked — only a quit
leaves both rings. Four in-section cross-references and §23's start
banner were renumbered twice as the section grew.

**#145 CHANGED THE PLAN FOR §22 — NOTHING BUILT.** Patrick's
ruling, in his own words: almost all sections take over from where
the last one ended; that served a purpose essential for the first
run of tests, and after that first long run it serves no purpose —
it is making things harder with the restriction. There is no reason
to change sections that are correct as they are now, so it applies
only to sections under rework — which is §22. **§22 will be rebuilt
on a fresh setup that meets its own needs** instead of inheriting
the scripted game; §23's start banner (now "straight off 22.29")
moves to name whatever the fresh §22 ends with. His guiding note:
a proof carried from another section can be lost with no harm.
Checked against the whole document: of the four things §22
inherits, three are proved elsewhere (the held-row dimming — §30;
the asker-never-crossed rule — 12.5; the full Log walk — §21), and
one is proved nowhere else — 22.25's "a ✅ replaces hearsay with
fact" (a quitter's ✅ turning another player's old "!" into a ❌) —
which is cheap to keep in the fresh section. **22.28's corrected
wording was settled in chat BEFORE the ruling and never built**
(the one Undo detail line, Ann's ⭐ accusation entry, "Dan's out
entry and Ann's accusation are both permanent history"); the fresh
rebuild will likely fold it in. Full detail: build-history.md #145.

**WHAT IS LEFT OF THE CATCH-UP — the same two pieces.** §22 (now
the fresh-setup rebuild, above) **and APPENDIX D, untouched** —
three functions that no longer exist (`accuseYes`, `accuseRight`,
`wrongAccTap`), five descriptions written before #133, a coverage
map pointing at the OLD §31's numbers in six places and now at
§22's old numbers in about a dozen entries, drifted line numbers
(`logTurn` 860 → 889, `renderTurnBar` 1846 → 1978, `saveState`
2682 → 2800), and the incomplete `clearCellNote` entry. Note the
fresh §22 will move Appendix D's §22 targets again — build the
section first, then the appendix.

**A WORKING NOTE.** Patrick said plainly that he could not track the
renumbering in his head, and a plain numbered list of the section's
Do cells fixed it at once. When a section's numbers shift under him,
print the list without being asked.

Still open (pending.txt numbering): the test-doc catch-up
(pending 4) is now **§22's Log step and Appendix D**. The
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

- #144 (2026-07-27): the #143 findings BUILT — 21.4 corrected (the card in the shower line, the Undo entry's one detail line, the quoting), and #143's own numbering slip recorded; §22 rebuilt from 25 steps to 29 as far as its Log step — the one-door Out modal, Ann's exit moved to the ⭐ Accuse road at 22.5–22.10 with the arm-and-lapse restored, the "already out" refusal moved to the ⭐ modal, and two rounds of renumbering; the docx at 405, machine-verified after every step; §22.28 and Appendix D left; no app code.
- #145 (2026-07-28): NOTHING BUILT — 22.28's corrected wording settled in chat from the code; then Patrick's ruling: the section-to-section carry-over rule is dropped for sections under rework, §22 to be rebuilt on a fresh setup of its own (§23's banner moves with it; only 22.25's ✅-replaces-hearsay proof is unique and kept); docx confirmed in sync at 405; ended early — model usage out after a switch from Opus 5.

## Next session's goal (#146, from #145)

**REBUILD §22 "PLAYER OUT" ON A FRESH SETUP, then Appendix D.**

**§22 first.** Under Patrick's #145 ruling (the carry-over rule is
dropped for sections under rework), §22 no longer inherits the
scripted game — it opens on a fresh setup that meets its own needs.
Claude's standing offer, held over from #145: draft the fresh §22
in the two-column chat shape for Patrick to mark up, per the §22
pattern in chat&test-spec-styling.md — draft, mark-up, phone run,
then into the script on his go. What the draft must carry: Ann,
Bob, Me and Dan seated; the modal's one door and its refusals; the
arm-and-lapse; Ann's exit by the ⭐ Accuse road; the skip forward
and backward; Dan's quit; the quit marks' permanence under Undo;
the settled 22.28 wording folded in; and the one inherited proof
that lives nowhere else — 22.25's "a ✅ replaces hearsay with
fact" (one ask where somebody shows, then the quit holding that
card). §23's start banner moves to name the fresh §22's ending.

**Appendix D after — not before.** The fresh §22 will move the
map's §22 targets again, so the appendix waits for the section.
Its list from #143 stands: remove `accuseYes`, `accuseRight`,
`wrongAccTap`; bring five descriptions current (`openAccuseModal`,
`checkStars`, `undoTurn`, `logTurn`, `logOut`); renumber the
map's six old-§31 references and its §22 references; refresh the
drifted line numbers (`logTurn` 860 → 889, `renderTurnBar`
1846 → 1978, `saveState` 2682 → 2800, `undoTurn` 2241 → 2393);
finish the `clearCellNote` entry (19.4, 19.7, 19.8, 19.9).

**One note, not a job.** The #132 You-form and the named card are
still proven nowhere in the document. Nothing contradicts them and
nothing tests them; whether to spend a step is Patrick's call —
the fresh §22 may be a natural home.

It all goes through `docs/build-mcts-test.js`; the docx is generated
and never hand-edited, then verified row-for-row. The document
stands at 405 steps, §22 at 29 — #145 changed no files but docs.

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
like any other change (#79). Claude also scripts a short opener note
and hands it to Patrick in chat — goal, what's decided, the
reading list, and the working rules — at session end
(Patrick, #114/#124). Patrick commits (this repo and any project repos
touched).
