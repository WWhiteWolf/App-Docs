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

## Where things stand (updated 2026-07-27, session #139 — #138 reconstructed from the code, §25 of the test doc rebuilt to 20 steps, §31 scoped for a full rewrite)

**THE APP IS STILL WITH APPLE.** Submitted 2026-07-26 at #136 with
all ten roadmap steps done — up to 48 hours to review, an email
when decided, release set to AUTOMATIC so an approval puts it on
the store by itself (Apple: up to 24 hours to appear). No answer
had arrived by the end of #139.

**#138 DERAILED AND LEFT NOTHING WRITTEN.** Its goal was the
test-spec catch-up. Patrick proposed that §31 be rewritten whole
rather than patched and pasted a few paragraphs of the #133 record
in as reference; after that paste Claude lost track of which
session it was in, a model switch made it worse, and Patrick ended
it before anything else went wrong. But it was not empty: he found
a real bug during it and it was fixed in two lines. After a close
and reopen, with the ask made and the shower already tapped, the
turn bar named the ASKER instead of the shower — `lastShowerName`
was set as a turn played out but never saved, so the reopen brought
it back empty and line 2013 fell through to the current player. The
fix rides the snapshot (line 2812 saves it, line 2850 restores it).
The Log was never affected. The wrapper copy is byte-identical, and
Patrick has rebuilt in Xcode — **the phone is now current at
#139.** The build sitting with Apple predates the fix.

**#139 RECONSTRUCTED #138 AND REBUILT §25.** The gap was closed
from the code and Patrick's own line numbers, not from memory.
§25 had no step that woke the app with the shower tapped and the
turn not yet advanced — exactly the bug's state — so 25.18 now
closes and reopens straight off the shower tap and checks the bar
reads "Turn 1 — Dan showed ✓"; a new 25.19 carries the Log check
(no second close: 25.14 already proves the Log page wakes); and
25.20 picked up Next ▶, because the tap matters to the document's
single pass even though the Log is written at the shower tap.
§25 is 19 steps → 20, **the docx at 401**, read back by machine.
Patrick proved 25.18 on his phone himself. Also recorded: the
code's phase names and the screen's words nearly invert — phase
`waiting` is the screen's "showed ✓".

**§31 IS THE NEXT PIECE, AND IT IS A WHOLE REWRITE.** All
seventeen steps describe the accusation flow #133 removed — the
modal opening by itself on the fourth ⭐, the two-question "Do you
want to make an accusation?" over "Were you right?", undoable
endings, and Out's 😢 road. Its first two steps are duplicates,
not orphans: §18.5 already tests the more-than-one-⭐ warning, and
Patrick ruled the watcher tests belong there. The whole accusation
flow was read out of the code at #139 and written into
build-history.md "#139" in full — the modal's three parts, both
refusal messages, all four ending lines, the Log line's shape —
**so #140 drafts from that record and does not re-read the code.**
**One question has to be answered first: which ending §31 finishes
on.** Three of the four endings are terminal and no verdict can be
undone, so the section reaches exactly one of them and the
document stops there.

Still open (pending.txt numbering): the Feedback-modal bug
question (pending 2, noted #111); the web-spec evaluation
(pending 3, open since #87); the test-doc catch-up (pending 4) —
half done, §31 is what remains, and it is **#140's goal**; the
mistouching (pending 1, diagnosed #137 — Patrick's next move is
the phone's Touch Accommodations settings, not the code); the
narrow-width screens (pending 5, the same fix as pending 1); and
the stale comment tail at line 810 of mystery-clues-tracker.html
(pending 6), parked by Patrick. Small and parked: the "Every other
cell is clean" gloss in 24.x/25.11; the docx message-font
distinction. The #114 docx zoom quirk is DROPPED (Patrick, #128).

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

## Next session's goal (#140, from #139)

**THE §31 REWRITE — the last of pending item 4.** All seventeen
steps of "31 — End of Game" describe the accusation flow #133
removed, so the section is written fresh, not patched (Patrick's
call). Its first two steps are dropped rather than moved: §18.5
already tests the more-than-one-⭐ warning, and the watcher tests
belong there (Patrick, #139).

**Read `MysteryCluesTracker/docs/build-history.md` "#139" first.**
The whole flow is written out there from the code — the ⭐ Accuse
button as the one door, the modal's three parts and their exact
headings, both dim-tap refusals, the four ending lines and which
one glows, the Log line's format, and the frozen-tap message. It is
there so the code need not be read again.

**The first question, and it shapes everything after it: which
ending does §31 finish on?** Three of the four endings are terminal
and no verdict can be undone — only an opponent's wrong accusation
leaves the game alive. So the section may walk as many
opponent-wrong accusations as it likes but reaches exactly ONE
ending, and the document stops there for good.

It all goes through `docs/build-mcts-test.js`; the docx is
generated and never hand-edited, then verified row-for-row. Still
in item 4 besides §31: the #132 shower line and the #133 Log
wordings wherever else they appear in the 401 steps, and Appendix
D's matching entries.

**Two things may take the agenda first.** Apple's review answer may
arrive and set its own. And Patrick was going to try the phone's
Touch Accommodations settings against the mistouching — whatever
that leaves over is what a code change has to earn, and any code
change now means a new version number and a fresh submission.
Also still available if wanted instead: the Feedback-modal bug
question (pending 2), the web-spec evaluation (pending 3), the
narrow-width screens (pending 5, the same fix as pending 1), and
the one-sentence stale comment at line 810 (pending 6).

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
master-handoff.md (this refresh), Publishing-Strategy.docx (the
next-session note). #139 touched no app code. Nothing in App Store
Connect lives in a repo.

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
