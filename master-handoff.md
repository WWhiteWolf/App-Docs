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

## Where things stand (updated 2026-07-27, session #144 — the #143 findings built: 21.4 corrected and §22 rebuilt onto the ⭐ Accuse road)

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

**WHAT IS LEFT OF THE #143 LIST — two pieces.** **§22's Log step,
now 22.28**, still reads "Turn 9 — 😢 Ann: Wrong Accusation", which
the app can no longer write (`logOut` is called once, at 2524,
always with `'quit'`); Ann's exit now writes
"Turn 9 — ⭐ Ann accused Card 2, Card 11, Card 20 — wrong". The same
step still says the Undo entry has two detail lines, and calls both
entries "out entries" when only one is. **And APPENDIX D is
untouched** — three functions that no longer exist (`accuseYes`,
`accuseRight`, `wrongAccTap`), five descriptions written before
#133, a coverage map pointing at the OLD §31's numbers in six places
and now at §22's old numbers in about a dozen entries, drifted line
numbers (`logTurn` 860 → 889, `renderTurnBar` 1846 → 1978,
`saveState` 2682 → 2800), and the incomplete `clearCellNote` entry.

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
- #121 (2026-07-22): the game of minimums PHONE-RUN and grown to 20 steps (the Log-check step); the passed-turn find (pending item 8); the second-`?` first-claim corrected (15.2/15.6 had it since #92); the accidental #120-window write repaired by Patrick's git restore; docs only, no code.
- #122 (2026-07-22): the big shrinking game designed, drafted, phone-run, and SETTLED at 47 steps — §27 COMPLETE; Eve and Faye seated; the mark-knowledge-when-it-arrives rule; two code finds (pending 9–10); docs only, no code.
- #123 (2026-07-22): §27 BUILT into the script as §27–30 + Appendices B–C; §19's two steps in; End of Pass DROPPED; the docx at 382, machine-verified row-for-row; the draft handed to Patrick for deletion; no app code.
- #124 (2026-07-23): code cleanup 1 of 2 — items 2 and 5 BUILT; the messaging review opened, its "Me" group BUILT (you-form refusals, the dotless turn bar) and spec-aligned (99 rows, docx at 382); all browser-verified; the styling doc renamed chat&test-spec-styling.md, its shape now law for all chat; the wrapper copy deliberately deferred to #125.
- #125 (2026-07-23): code cleanup 2 of 2 — the messaging review CLOSED (dim-until-picked in three modals; two leave-alone rulings); the passed-turn Log line; the column-naming refusal; the modal rubber-band fix; GAME OVER and the ⭐ ACCUSATION FLOW built (Patrick's in-session design — endings, freeze, undoable accusation, 390-step spec); the wrapper-and-phone pass run — the phone CURRENT.
- #126 (2026-07-23): the appendix SETTLED (Appendix D = list + two-column map, eight new functions not nine); §31 "End of Game" split out; six new tests placed and phone-proven; the mid-ask Next ▶ ruling ("Select 3 or 0…"); the docx at 398, machine-verified; docs and script only, no app code.
- #127 (2026-07-23): Appendix D BUILT (list, map, conclusion; two dead-code finds made accurate); the mid-ask Next ▶ fix BUILT, phone-proven, steps 27.5–27.6 in with the §27 sweep; the docx at 400, machine-verified twice.
- #128 (2026-07-24): the §31 pass CLEAN (17/17, widened from 11); the test-spec INDEX in (computed, never typed); Appendix D reordered — "The Coverage Map & Function List", map first; pending.txt and pending.docx brought current; landscape and the black-on-gold revisit closed by decision; no app code.
- #129 (2026-07-24): Publishing-Strategy.docx revisited and four stale spots fixed (the #72 build-order block retired, product two's name and status, the two lanes sentence, the rollout strategy's old phrasing); the old PWA re-upload loose end chased down and closed; three reference-only files deleted from App-Docs; ROADMAP.md created; the App Store Connect app record for Mystery Clues Track Sheet created — step one of ten, registered without the ✓; no app code.
- #130 (2026-07-24): roadmap steps two and three DONE — privacy-policy.html and support.html written (store-pages/), published live on elyfont.com by Patrick, and saved into App Store Connect (Support URL on the version page, Privacy Policy URL on the App Privacy page); docs/DEPLOY.md created for this project; the separate-docs policy decision; the home-page-card idea parked; no app code.
- #131 (2026-07-24): roadmap steps four through six DONE — App Privacy declarations answered "No" and published ("Data Not Collected"); the age rating questionnaire answered None/No throughout, with one genuine edge case (Social Media Disabled for Users Under 13) worked through to a 4+ rating; primary category set to Entertainment, secondary to Utilities; the Subtitle raised and deliberately left open for step eight; a mid-session conduct reset after Claude broke the click-directions and one-question rules; no app code.
- #132 (2026-07-25): roadmap step seven DONE — seven screenshots reshot on a 9/9/9/3 deck (the Clue-caution catch) and uploaded to the 6.9-inch slot in Patrick's order; the Log shower line rebuilt in-session (You-form, the known card named); the invisible accusation door and the anticlimactic ending logged — the ending's drama named #133's opener; the social-media notice closed (#131 answers stand); rule 11 (announce-and-consent) into both CLAUDE.md files.
- #133 (2026-07-25): the ending's drama — the ⭐ Accuse door (any accuser, four verdicts, no undo past a verdict), the glowing win moment, the quits-only Out modal; slot eight uploaded.
- #134 (2026-07-25): the #133 docs catch-up written and verified; roadmap step eight DONE — description and Subtitle saved and verified on Apple's pages; the ⭐-rejected-in-Description find; the DSA non-trader question closed by reading.
- #135 (2026-07-25): roadmap step nine DONE — the minimum iOS lowered 26.5 → 16.6 and export compliance declared (both code-verified), then build 1.0 (1) archived, validated clean, and uploaded; TestFlight left unused; the unset-shows-"No" encryption find and the Xcode Cloud wrong turn logged; no app code.
- #136 (2026-07-26): roadmap step ten DONE — Keywords (95 bytes) and Promotional Text (169 characters) written from Patrick's own words and saved, "clue" ruled out of both; the Keywords-is-required question answered from Apple's own page; the build attached, six submission blockers cleared, the "You won" shot reshot (the 6.5-inch inheritance trap found by Patrick), and THE APP SUBMITTED FOR REVIEW; no app code.
- #137 (2026-07-26): the grid's mistouching DIAGNOSED from the code (the 430 floor, the always-six columns, 24 × 28 against 44 × 44, no gap and no flash, 🏠 alone acting on first touch, the silent row-off pick in the active column); the #122 fat-finger line found as corroboration; the #86 grid-clip caveat proven and merged with pending 1; Patrick's before-contact insight answered by Apple's Touch Accommodations, and his decision to try the settings before any code; one bug reported and withdrawn; no app code.
- #138 (2026-07-26): DERAILED — Claude lost the session number after a #133 paste, a model switch made it worse, Patrick ended it and no docs were written; but his own find, the turn bar naming the asker instead of the shower after a reopen, was fixed in two lines (lastShowerName into the snapshot) and copied to the wrapper.
- #139 (2026-07-26/27): #138 reconstructed from the code and written up; §25 rebuilt to 20 steps so the doc proves the #138 fix (25.18 reshaped, 25.19 new, Next ▶ into 25.20) — the docx at 401, machine-verified; §31 scoped as a whole rewrite and the entire ⭐ accusation flow harvested from the code into build-history.md; the phase-name inversion recorded; no app code.
- #140 (2026-07-27): Patrick's own agenda in place of §31 — the release paused to MANUAL, the grid rebalanced (∑ and 🏠 24 → 33, players 50 → 47, two borders thinned), the cell note rebuilt (4 characters, Set deleted, Done now saves) and the Guide corrected; the version pulled from review and resubmitted with build 1.0 (2); §19 joined §31 in the test-doc debt; a step-by-step pipeline document asked for and parked.
- #141 (2026-07-27): §31 "End of Game" rewritten to 18 steps on Patrick's design — a fresh three-player game, Seats 2/4/5 un-seated, no turns played, ending on the last live opponent's wrong accusation — phone-run by Patrick and built into the script and the docx (402 steps, machine-verified); three code finds logged; the mistouching remainder parked at his direction; no app code.
- #142 (2026-07-27): §19 "Cell Notes" rewritten to 10 steps — old 19.2/19.3 merged to prove Done saves and closes, "XXXX" and the "XXXX?" cap, the Set button gone from every step, and a new 19.7 proving Close DISCARDS (read out of the modal's markup; the old step had it backwards); the string-quoting rule settled into the styling doc; Appendix D's four map lines renumbered; the docx at 401, machine-verified; no app code.
- #143 (2026-07-27): the wordings sweep RUN — the #132 shower line and the #133 accusation lines checked at every Log-reading step and found clean (21.5 incomplete, the You-form and named card proven nowhere); §22 "Player Out" found still testing the pre-#133 Out modal (six steps) and Appendix D found listing three functions that no longer exist, with its map on the old §31 and its line numbers drifted; nothing built, no app code; the load flag miscounted by feel and corrected.
- #144 (2026-07-27): the #143 findings BUILT — 21.4 corrected (the card in the shower line, the Undo entry's one detail line, the quoting), and #143's own numbering slip recorded; §22 rebuilt from 25 steps to 29 as far as its Log step — the one-door Out modal, Ann's exit moved to the ⭐ Accuse road at 22.5–22.10 with the arm-and-lapse restored, the "already out" refusal moved to the ⭐ modal, and two rounds of renumbering; the docx at 405, machine-verified after every step; §22.28 and Appendix D left; no app code.

## Next session's goal (#145, from #144)

**FINISH THE TEST-DOC CATCH-UP. Two pieces are left, and both are
build work — the finding is done and the code has been read.**

**§22's Log step, now 22.28.** It reads "Turn 9 — 😢 Ann: Wrong
Accusation", which the app can no longer write: `logOut` is called
from one place (2524) and always passes `'quit'`. Ann's exit now
writes an accusation entry — "Turn 9 — ⭐ Ann accused Card 2,
Card 11, Card 20 — wrong" (the cards go in deck order, line 1811).
The same step still says the ↩ Undo entry has "two detail lines"
when it draws one, and it closes by calling both entries "out
entries" when only Dan's is one now.

**Appendix D, untouched.** Remove the three functions that no longer
exist (`accuseYes`, `accuseRight`, `wrongAccTap`); bring five
descriptions current (`openAccuseModal`, `checkStars`, `undoTurn`,
`logTurn`, `logOut`); renumber the coverage map's six references to
the OLD §31 AND its §22 references, which #144 moved by four;
refresh the drifted line numbers (`logTurn` 860 → 889,
`renderTurnBar` 1846 → 1978, `saveState` 2682 → 2800, `undoTurn`
2241 → 2393); and finish the `clearCellNote` entry, which names two
steps where Clear is tapped at four (19.4, 19.7, 19.8, 19.9).

**One note, not a job.** The #132 You-form and the named card are
still proven nowhere in the document. Nothing contradicts them and
nothing tests them; whether to spend a step is Patrick's call.

It all goes through `docs/build-mcts-test.js`; the docx is generated
and never hand-edited, then verified row-for-row. The document
stands at 405 steps, §22 at 29.

**How #144 worked, and it worked well.** Patrick named the section,
Claude went straight to the file, and the section was walked step by
step — each step either reported as reading true and passed over, or
corrected, proposed in full, and built on his go. Steps that need no
change do not get a stop.

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

## Commit status: Patrick's commits, when ready

The #135 and #136 lists are both COMMITTED — #135 mid-session at
#136, and #136 confirmed by Patrick at #137. Nothing is left
waiting from either.

The #137 list was committed by Patrick at the start of #139.

From #138 — MysteryCluesTracker: mystery-clues-tracker.html (the
two-line turn-bar fix at 2811–2812 and 2850) and the wrapper's
www/ copy of the same file. Nothing else; that session wrote no
docs.

From #139 — MysteryCluesTracker: docs/build-mcts-test.js (§25's
three steps), docs/mcts-master-test.docx (regenerated, 401 steps,
machine-verified), docs/build-history.md (the #138 and #139
sections), docs/pending.txt (the header date, the standing block,
item 4 rewritten), docs/pending.docx (rebuilt from the txt and
machine-checked — 32 paragraphs, five bold headers, 11,198
characters matching the source exactly); App-Docs:
master-handoff.md, Publishing-Strategy.docx (the
next-session note). #139 touched no app code. Nothing in App Store
Connect lives in a repo.

From #140 — MysteryCluesTracker, APP CODE THIS TIME:
mystery-clues-tracker.html (fourteen lines — seven for the grid
widths and borders at 134/143/153/156/158/159/162, five for the
cell note at 183/629/631/632/636, and the two Guide lines at 397
and 430); the wrapper's www/ copy of the same file (verified
byte-for-byte); and the wrapper's
MysteryCluesTrackSheet.xcodeproj/project.pbxproj
(CURRENT_PROJECT_VERSION 1 → 2 in both Debug and Release —
MARKETING_VERSION unchanged at 1.0). Docs: docs/build-history.md
(the #140 section), docs/pending.txt (header, standing block,
items 1 and 4, and the pipeline document into NICE-TO-HAVE),
docs/pending.docx (rebuilt from the txt — 44 paragraphs, five bold
headers, word-for-word identical to the source by machine check),
docs/upgrade-scope.md (the 🏠 mockup entry amended — 33px, and only
the right gold border still 2px);
App-Docs: master-handoff.md (this refresh), Publishing-Strategy.docx
(the next-session note). Nothing in App Store Connect lives in a
repo, so the release setting, the removal from review and the
resubmission are recorded in the docs only.

From #141 — MysteryCluesTracker: docs/build-mcts-test.js (§31's
seventeen steps replaced by eighteen and its Start banner rewritten),
docs/mcts-master-test.docx (regenerated, 402 steps, machine-verified
row-for-row), docs/build-history.md (the #141 section),
docs/pending.txt (header, the test-doc line, item 4 cut back to §19,
and the unreachable refusal into the dead-code list),
docs/pending.docx (rebuilt from the txt — 44 paragraphs, five bold
headers, word-for-word identical to the source by machine check);
App-Docs: master-handoff.md (this refresh), Publishing-Strategy.docx
(the next-session note). #141 touched NO app code, and no draft file
was made — Patrick's ruling; he keeps the §31 draft in Word.

From #142 — MysteryCluesTracker: docs/build-mcts-test.js (§19's
eleven step pairs replaced by ten, and Appendix D's four cell-note
map lines renumbered); docs/mcts-master-test.docx (regenerated, 401
steps, machine-verified); docs/build-history.md (the #142 section);
docs/pending.txt (header, the test-doc line in the standing block,
and item 4 rewritten); docs/pending.docx (rebuilt from the txt —
44 paragraphs, five bold headers, every paragraph matching the
source word for word by machine check); docs/chat&test-spec-styling.md
(the string-quoting rule); App-Docs: master-handoff.md (this
refresh), Publishing-Strategy.docx (the next-session note). #142
touched NO app code, and no draft file was made — the §19 draft
lived in chat and Patrick phone-checked it there.

From #143 — MysteryCluesTracker: docs/build-history.md (the #143
section), docs/pending.txt (the header, the test-doc line in the
standing block, and item 4 rewritten around the sweep's result),
docs/pending.docx (rebuilt from the txt and machine-checked
paragraph by paragraph); App-Docs: master-handoff.md (this refresh),
Publishing-Strategy.docx (the next-session note). **#143 changed
NOTHING in the app and NOTHING in the test document** —
build-mcts-test.js and mcts-master-test.docx are untouched, and the
document still stands at 401 steps. No draft file was made and no
git commands were run.

From #144 — MysteryCluesTracker: `docs/build-mcts-test.js` (21.4's
Make sure; §22's steps 1, 2, 4, the new 5–10 block replacing the old
5–6, 20 and 21; four in-section cross-references and §23's start
banner); `docs/mcts-master-test.docx` (regenerated, 405 steps,
machine-verified after every single change — the step count, exactly
which cells differed, every §22 cell matched to the script word for
word, the tester columns empty, and §1–21 and §23-onward untouched
but for the renumbering); `docs/build-history.md` (the #144 section);
`docs/pending.txt` (the header, the standing block's test-doc line,
and item 4 rewritten around what is built and what is left);
`docs/pending.docx` (rebuilt from the txt — 48 paragraphs, five bold
headers, every paragraph matching the source word for word by machine
check); App-Docs: `master-handoff.md` (this refresh),
`Publishing-Strategy.docx` (the next-session note). **#144 touched NO
app code and no draft file was made** — every step was settled in
chat. No git commands were run.

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
the finished session folded into ONE history-index line — plus the
strategy doc's "Next session — start here" note and the active
project's own docs. If pending.txt changed, pending.docx is rebuilt
from it to match, machine-checked line-for-line (Patrick, #128).
The refresh is discussed and gets Patrick's go
like any other change (#79). Claude also scripts a short opener note
and hands it to Patrick in chat — goal, what's decided, the
reading list, and the working rules — at session end
(Patrick, #114/#124). Patrick commits (this repo and any project repos
touched).
