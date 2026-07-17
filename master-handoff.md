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

## Where things stand (updated 2026-07-17, session #103 — modal message lines built & phone-verified; spec refreshed; §23 reconstructed, not settled)

**The app changed this session: FOUR modals gained the #99 message
line (New Game, Template Action, ∑ Summary, Edit Cards) — one
`<div class="modal-msg">` each in `mystery-clues-tracker.html`, the
wrapper's www/ copy verified byte-identical, all four PHONE-VERIFIED
by Patrick on a fresh build. The spec was refreshed twice, each
regeneration verified row-for-row: (1) a bold ⚠ front-page
precaution (read "Make sure" BEFORE the "Do" — some responses last
only seconds), the step count now COMPUTED by the script (reads 206;
TBD gone for good), and the arming steps 3.8 / 3.9 / 5.7 / 18.6
enriched with the in-modal message; (2) the seven bare "Status:"
wordings replaced with "The bottom strip shows: …", 5.8 additionally
marked "for a few seconds". §23 New Game was RECONSTRUCTED in chat
from the code paths plus build-history's record of Patrick's #100
markup (the cloud ate the original): 15 steps — 23.1 split into tap
and type, the banner carrying the ∑/🏠 state — saved as
`docs/s23-draft.md`. NOT settled, NOT in the script, NOT yet
phone-run.**

The phone is FRESH-INSTALLED (state wiped): the scripted-game state
must be rebuilt through §22's end before §23 can run. Still open:
the "lettering too small" phone note, spot never pinned. Decided
#103: the card-row ✕ in Edit Cards stays silent (by design — nothing
touches the deck until Save). NEW observation, parked for §25:
Welcome Back's two New Game buttons fire on a SINGLE tap — no
arming — in contrast to the in-game New button's two-tap.
`s22-draft.md` is still on disk — deletion waits on Patrick
confirming §22 reads right in the regenerated docx.

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

## Next session's goal (#104, from #103)

**Rebuild the scripted-game state on the phone, run §23 from
`docs/s23-draft.md` (15 steps), pin the "lettering too small" find
along the way, settle the section, then — on its go — drop it into
the script. Then §24 (Guide & 💬 Feedback), §25 (Welcome Back &
resume; carries the new single-tap observation) if bandwidth.**
Still open from #87: the web SPEC doc (App-Docs
`MysteryTracker-spec.md`) evaluated for a mobile edition.

## Commit status (#103): Patrick's commits, when ready

MysteryCluesTracker: mystery-clues-tracker.html + the wrapper's www/
copy (the four modal-msg lines), docs/build-mcts-test.js +
docs/mcts-master-test.docx (both spec passes), docs/s23-draft.md
(NEW), docs/build-history.md (#103 section), docs/pending.txt — plus
anything of #100's still uncommitted (docs/test-spec-styling.md,
earlier script/docx states ride along automatically). App-Docs:
master-handoff.md (this refresh). Delete docs/s22-draft.md before
committing, once §22 is confirmed in the docx. Any older #98/#99
items not yet committed ride along (ContentView.swift,
upgrade-scope.md; elderlyassistant and MysteryTracker CLAUDE.md).

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
like any other change (#79). Patrick commits (this repo and any
project repos touched).
