# Master hand-off — the one session chain (all projects)

**This folder (Projects → App-Docs) is the single home for cross-project
docs — Patrick's decision, session #71 (2026-07-09): everything in one
folder, backed up and version-controlled (this folder is a git repo;
Patrick does all commits).** Moved here from OneDrive → App-Docs the same
day; the OneDrive move had been convenience only.

## How a session starts

1. Patrick connects **Projects → App-Docs** (this folder) and says read
   the master hand-off.
2. Claude reads this file, then `Publishing-Strategy.docx` (the north
   star: strategy, standing rules, the four products, the learning
   tracker) if the session is publishing/business-side.
3. Claude connects whichever project folder the session's goal lives in
   and reads THAT project's own docs (each app keeps its own material).
4. Patrick names ONE goal; scope it together; Claude waits for his "go."

## Standing rules (short form — the full set is in the strategy doc and elderlyassistant/docs/session-start.md)

- Patrick does ALL git commits. Claude runs NO git commands at all in
  Patrick's repos — in #71 even a read-only `git status` left index.lock
  files behind that would have blocked his commits. Look at files
  directly instead.
- One step at a time; discuss before building; wait for the go.
- Verify before asserting — read the actual code/files, don't guess.
- One question at a time; open questions, no boxed choices.
- Never give click-directions for a screen Claude can't see.
- Patrick leads; Claude doesn't steer. No urgency — his pace. He's
  retired; this is a hobby — no deadlines, no clerk-abrupt tone; warm
  and conversational. Not wasteful of his time, but never hurried.
  Patrick lives alone; Claude's tone is sometimes the only
  conversation he gets all day — it matters. The conversation is
  part of the work, not overhead.

## Where things stand (updated 2026-07-16, session #95 — test doc §20–21 written; Notepad strip + Undo log built)

**The products, all to be published (decided #71; Memory-web dropped #72):**

1. **Mystery Tracker — web** — live at elyfont.com, Beta. Project:
   `Projects/MysteryTracker` (its own session docs: docs/session-start.md,
   docs/handoff.md, ROADMAP.md etc. — renamed #80 to match the other
   projects' naming).
2. **Mystery Tracker — mobile** (renamed from "Mystery Clues Tracker",
   #71) — PWA, Beta. **← THE ACTIVE EFFORT: clean up → App Store, FREE,
   via a bare Xcode+WKWebView wrapper. Read
   `Projects/MysteryCluesTracker/docs/upgrade-scope.md` FIRST — it holds
   every decision.** Progress (#72): ALL mechanical cleanup done and
   Patrick-verified (rename, voice claim, new icon, relative paths,
   bundled fonts — fully offline). No-thinking directive logged. Xcode
   26.6 + iOS components installed, Apple ID signed in, Dev account
   held — the toolchain is ready. #72 second sitting: the SCOPE IS
   COMPLETE — every design question decided and in upgrade-scope.md
   (🏠 = ✓-only toggle, mockup approved; mirror-the-web standing rule;
   truly-variable structure, player-shaped at setup; band 4 = web
   gold; setup mockup approved; templates carry the whole structure;
   minimums 15-card deck / 2 players / 2 cards / Me slot; asks = one
   card per non-empty category, auto-commit; 2-of-3 auto-check OUT;
   tinting ports as-is; LANDSCAPE DEFERRED till after the product is
   finished — ships portrait-only). **#73 (2026-07-10): the SETUP
   BUILD IS DONE and Patrick-verified in-browser** — categories data
   model; full setup UI (add/rename/delete categories, add/remove
   cards, counters, hint, gold band 4); defaults REDEFINED to
   Category 1–3 / Card 1–27 (de-Clue complete, mirrors the web);
   empty categories auto-delete; minimums REDEFINED (3 in Me hand /
   2 players / 2 active categories / 3 cards per active category /
   12-card deck); ask size = active categories (built). Details in
   upgrade-scope.md's "Built — session #73" section. CLAUDE.md rule 6
   added to all three project folders (no defensiveness — move ahead).
   **#74 (2026-07-10): the GAME PLAY BUILD IS DONE and Patrick-verified
   in-browser** — tier gate removed (Card Count + turn superscripts
   OUT entirely, Patrick's #74 redefinition; Log/Notepad standard);
   ALL deductions removed (no-thinking complete in code); Player Out
   rebuilt as TWO models (😢 Wrong Accusation = turn skipped, still
   shows, light fade; 👋 Quit = cards shown, column ✗-filled, fully
   out; permanent marks + log entries, Undo-proof); 🏠 House column
   built (spec Page 9, touch-adapted); ✓/✗ tinting ported; Σ ✕
   recolored red; ask-guard message generalized. Details in
   upgrade-scope.md's "Built — session #74". NEW RESOURCE:
   `MysteryTracker-spec.md` (the web app's functional spec) — Patrick
   supplied it mid-session; it drove the 🏠 and Player Out builds.
   SAVED into App-Docs by Patrick, #75. **#75 (2026-07-11): the
   CATCH-UP SESSION IS DONE — all seven items, each Patrick-verified
   in-browser:** shower-initial in Me's column removed (the `shownme`
   mark gone entirely); full Guide factual pass (three "3 cards"
   spots, "Me" mark wording, stale Renaming Cards section replaced,
   ride-along: live asking hint no longer hard-codes "three");
   gold-band aesthetics CLOSED no change; P5/P6 dark empty columns
   SETTLED as-is (deliberate deviation from the web); Play button now
   always visible on Setup, dimmed until ready, tap-when-dim names
   the first unmet condition; duplicate card names guarded at the
   Edit modal's Save (deck-wide, case-insensitive, rejected Save
   changes nothing); `loadState` duplicate line removed. Ride-along:
   grid scroll bars slimmed to 4px (desktop bar was clipping P6).
   STANDING NOTE (Patrick, #75): old/saved games don't exist and
   don't matter — no migration concerns, ever. FUTURE SESSION noted:
   a Guide EDITING pass (wording/flow; first case: SETUP intro's
   "from the list below"). Business-side notes (Sonnet session,
   2026-07-11, saved as `session-notes-hasbro-and-tiering.md` in
   App-Docs): Hasbro Spark CLOSED (not pursuing); monetization
   pricing model OPEN; TIERING DECIDED — fold tiering hooks back
   into this rebuild, scoped in a coding session first.
   **#76 (2026-07-11, "the two-tier session"): the TIERING SCOPE IS
   DECIDED** — scoping only, no code changes. Patrick threw out all
   prior tiering rules and wrote new ones: TWO tiers. Free = today's
   app exactly (records everything, concludes nothing — no-thinking
   is the free tier's character). Paid (name OPEN) = the thinking:
   the web's seven Appendix B read-only helpers (never place a
   mark). Turn tags stay OUT of both tiers (cluttered the grid).
   OPEN idea: infer player card counts instead of restoring a typed
   Card Count field (Patrick's family variant — even deal, leftovers
   face down on the board — makes counts exact; the 🏠 column was
   born from that variant). Coaching ideas parked for much later.
   Still OPEN: gate mechanics (unlock method, dormancy in the free
   app) and pricing. Full detail: upgrade-scope.md "Decided —
   session #76". Ride-alongs: notes file CORRECTED (tiering was in
   the MOBILE app, never the web) + #76 market/visibility addendum
   added (Clue Solver = closest competitor, entirely free with a
   deduction engine, ~3 ratings; Board Game Stats = the model to
   copy; the category is hard to find in the store). NEW reference
   file `MysteryCluesTracker/docs/pre74-tiering-reference.html`
   (Patrick pulled the pre-#74 tier code from git; does NOT ship).
   Tone rules expanded in all three projects' CLAUDE.md +
   elderlyassistant session-start (retired/hobby pace, warm
   workbench tone, Patrick lives alone — the conversation is part
   of the work). **#77 (2026-07-11, "the Guide editing session"):
   the GUIDE EDITING PASS IS DONE** — every section walked, Patrick
   reading in-browser as the work went. Highlights: SETUP intro
   rewritten as a true introduction (friendlier flowing tone = the
   pass's standard); SETUP sections REORDERED to the real flow
   (Categories → Editing → Templates → Players → Cards Held →
   Play; "Cards" renamed "Cards Held"); Editing section restructured
   to statement + bullets; duplicate NEW GAME section removed;
   "nickname" → "name" (Guide + popup placeholder); marks list
   gained a "Me" bullet and a persistent-"?" rewording; When Someone
   Shows trimmed to present tense; ∑ and Cell Note intros rewritten;
   two factual fixes (Undo greys only at GAME start; 👋 Quit also
   ❌s shown cards in other columns). RIDE-ALONG (Patrick's find,
   real bug): the 💬 feedback mailto had NO recipient — feedback
   could never arrive. Now sends to jojoMurphy@tuta.com (his
   reserved address); modal wording de-beta'd; new SUGGESTIONS
   Guide section; button restyled to the gold pill. Full detail:
   upgrade-scope.md "Built — session #77".
   **#78 (2026-07-12, "the pre-wrapper decisions session"): the app
   is RENAMED "Mystery Clues Track Sheet"** (no hyphen; home-screen
   label "Mystery ✓", plain U+2713 not the ✅ emoji; #71's
   match-the-web rule and fallbacks void; the "is 'Clues' generic?"
   question researched and settled — descriptive use, Hasbro v. Clue
   Computing, not legal advice; name availability still checked at
   listing time). Changed in all seven code spots (manifest ×2,
   title, apple-title, header, welcome line, feedback email) and
   Patrick-verified in-browser. VOICE INPUT AMENDED: field dictation
   into Setup's text fields comes FREE via the iOS keyboard once
   wrapped — nothing to build; voice commands stay out. DISCLAIMER
   SETTLED: none in the app; if one goes in the store description at
   listing time it names nobody ("Not affiliated with or endorsed by
   any…"). OPEN: whether the first-launch Welcome modal should
   mention the 💬 feedback button (code fact: 💬 lives only in the
   Guide screen's footer — the Guide is feedback's single doorway).
   The wrapper was not started. SESSION-CONDUCT notes (Patrick, #78,
   after mid-session rule slips): one goal then break — a session's
   length is VOLUME (files read, screenshots, research), not
   minutes; Patrick may say "rules check" mid-session = Claude
   re-reads CLAUDE.md right then; the first slip gets called
   immediately, not endured. Full detail: upgrade-scope.md
   "Decided + built — session #78".
   **#79 (2026-07-12, "the wrapper begins"): the WELCOME MODAL now
   mentions the 💬 feedback button (the #78 open question SETTLED —
   Patrick chose the friendly gesture; wording in upgrade-scope #79),
   Patrick-verified in-browser. THE WRAPPER IS STARTED:** Xcode
   project created at `MysteryCluesTracker/wrapper/` (bundle ID
   com.elyfont.MysteryCluesTrackSheet, Team set, NO nested git);
   toolchain proven end to end (Hello-world ran on Mac and iPhone 17
   Pro simulator; codesign keychain prompt handled); HTML + static
   COPIED into the project (Xcode 26 offers no reference-in-place —
   standing habit: re-copy + diff when the HTML changes);
   ContentView.swift replaced with a WKWebView loader; the REAL APP
   RAN in the simulator. OPEN PROBLEM stopping the session: custom
   fonts don't load (proven by a Courier-fallback experiment, since
   reverted; WKWebView sandbox wants one dedicated web folder). A
   www/ restructure hit Xcode 26's synchronized-folder FLATTENING
   (bundle loses subfolders — proven by a temp in-app diagnostic
   that's STILL IN ContentView.swift). THE AGREED FIX awaits #80:
   move www/ beside the .xcodeproj and add it as a classic folder
   reference by hand-editing project.pbxproj (Xcode quit first).
   Full detail: upgrade-scope.md "Built — session #79".
   SESSION-CONDUCT agreements (#79 end-of-session talk), TO BE
   WRITTEN INTO CLAUDE.md AT #80: (a) load flag by COUNTING, not
   feel — around a dozen screenshots, or one big research detour,
   Claude names the next natural breakpoint out loud (screenshots
   are Claude's heaviest load; screen-heavy sessions fill Claude
   fastest — the #78 "length is volume" note, now with a number);
   (b) the session-END docs refresh is NOT pre-approved — it gets
   discussed and gets Patrick's go like any other change (the #79
   slip: Claude edited both docs on "session's over" without
   asking first).
3. **A Place To Remember (Memory) — iPhone** — Alpha, mostly built.
   Project: `Projects/elderlyassistant` (its own session docs:
   docs/handoff.md, pending.txt, parked-items.md, session-start.md).
   Store prep comes after the Mystery rehearsal. Android version
   eventually, after the iPhone build (decided #72).
4. **Memory — web** — DROPPED (decided 2026-07-10, session #72): no web
   version. The app is built around the rich reminder scheme, which the
   web can't carry. elyfont.com gets a pointer to the App Store listing
   only.

**#80 (2026-07-12, same day; session titled "#79 Retry"): the
discussion-items session.
NATIVE-VS-WRAPPER SETTLED (Patrick): the app STAYS a WKWebView
wrapper — no native Swift rewrite; "decided for purposes of the
project"; future sessions don't re-open it** (full reasoning + a
fresh-eyes code-cleanliness report in upgrade-scope.md's "#80"
section — verdict: the HTML is clean, not the messy first draft the
rewrite principle warns about; a ~30-line optional dust list is
recorded there). **The #79 COMMITS ARE DONE, both repos** — verified
in .git/logs by file-reading, no git commands. The wrapper got its
first commit. NEW root `.gitignore` in MysteryCluesTracker keeps
xcuserdata/, *.xcuserstate, and .DS_Store out of history (a first
staged commit was aborted; `git reset` + `git rm --cached .DS_Store`
+ re-add produced the clean one). The two #79 session-conduct
agreements are WRITTEN (#80) as CLAUDE.md rules 7 and 8 in ALL THREE
project CLAUDE.md files — this repo, MysteryCluesTracker, and
elderlyassistant (added later the same session). ALSO #80, web-side
housekeeping: MysteryTracker's session docs RENAMED to match the
other projects (docs/RESUME-HERE.md → docs/session-start.md,
docs/SESSION-HANDOFF.md → docs/handoff.md; six live pointers
updated, ROADMAP's history mentions left as written). ALSO DONE
same session: a root CLAUDE.md created there (the full 8 rules,
rule 1 pointing at its session-start/handoff pair — all FOUR
project folders now open the same way; the old EMPTY docs/CLAUDE.md
deleted), session-start.md's stale OneDrive → App-Pubs pointer
corrected to Projects → App-Docs, and its title line renamed to
match. MysteryTracker's repo has all of this uncommitted —
Patrick's commit when ready.
Conduct note, logged without blame per rule 6: Claude ran `git
status` early in the session (rule slip, self-caught) — it left an
index.lock that Patrick deleted; the rule stands reaffirmed.

**#81 (2026-07-12): the www folder-reference fix — DONE, FONTS
LOAD.** The #79 open problem is closed on the first run: `www/`
moved beside the .xcodeproj, project.pbxproj hand-edited (Xcode
quit first) to add it as a classic structure-preserving folder
reference in the Resources phase; Patrick's simulator screenshot
showed the real app with the real Playfair/Lora lettering, and the
#79 sandbox-extension console errors are gone. The temp diagnostic
is OUT of ContentView.swift — Patrick removed it himself in Xcode
and re-ran (identical). NEW STANDING RULE (Patrick, #81), in the
CLAUDE.md files: when a step is quicker for Patrick to do by hand,
Claude describes it and hands it to him instead of burning tool
calls. Full detail: upgrade-scope.md "Built — session #81".

**#82 (2026-07-12): the DATA-SAFETY BRIDGE IS BUILT and half-proven.**
JS half: a guarded block in the HTML patches Storage.prototype and
posts every localStorage write/remove to a "storage" message handler
(no-op in a plain browser — Patrick browser-verified full behavior
unchanged; www/ re-copied, diff-identical). Swift half: Coordinator
mirrors into UserDefaults under `mct.mirror.`; a document-start
WKUserScript restores the mirror at launch. JS→native PROVEN in the
Xcode console (`storage bridge: set mctGame` lines as Patrick
played). ROLLBACK BUG found (Patrick: stop/restart resumed "in odd
spots") and FIXED — the restore was an unconditional copy and an
abrupt kill can leave the mirror a beat behind; it is now
FILL-GAPS-ONLY (restores only keys localStorage lacks). Web Inspector
ENABLED (`isInspectable`, #if DEBUG) and Patrick attached Safari's
inspector to the simulator and used its console — the tool is set up.
**OPEN BUG, mid-diagnosis when the session closed: after a
stop/restart + resume, Next is DEAD — no turn advance, no console
error; live sessions are fine (the fault arrives via the save/load
round-trip). The next diagnostic is READY: type `nextPlayer()` in the
inspector console — advance = touch/overlay problem, no advance =
state problem.** Wipe test (restore's full proof) not yet run. NEW
quirk queue: Log Copy dead in wrapper (cause found: no
navigator.clipboard on file://; fix routes discussed, UNDECIDED);
Notes keyboard pushes the page up (uninvestigated); card names
bigger + NORMAL weight (430px grid budget makes it a design talk).
Full detail: upgrade-scope.md "Built — session #82".

**#83 (2026-07-13): dead-Next CLOSED, messages seen, Copy FIXED, the
BRIDGE IS FULLY PROVEN.** The dead-Next "bug" was never a bug in the
turn logic and never resume-related — the nobody-showed guard was
refusing correctly (an asked card had a confirmed ✓); the real defect
was an invisible warning. THE FIX, mirror-the-web: the web's scrolling
status renderer ported; game-screen messages now take over the hint
line between Undo and Next (red for warnings); Setup's strip redressed
to be seen; NEW Log-screen strip (that screen had no message outlet at
all). LOG COPY fixed the permanent way (Patrick's call): a second
bridge handler "clipboard" → UIPasteboard; paste-proven into Notes.
WIPE TEST PASSED twice — first run caught a real gap (pre-bridge keys
like the first-launch flag had no mirror copy), fixed with a
full-sync-at-launch in the bridge block; second run clean. The bridge
now has every proof. Quirk queue remaining: Notes keyboard push
(uninvestigated), card names bigger/normal weight (design talk).
Full detail: upgrade-scope.md "Built — session #83".

**#84 (2026-07-13): DRESSING, two of three, plus the header emblem.**
Home-screen name DONE ("Mystery ✓", plain U+2713 — verified in
pbxproj, both configs; Patrick-verified on the home screen). App icon
INSTALLED (icon-1024.png into the AppIcon Any-Appearance well; a
stray first-drag image set caught and removed; verified on disk and
home screen). NEW decision + build the same session: the 🔍 in the
app's four header spots (main h1, Welcome, both Welcome Backs)
REPLACED by the icon's fanned cards with the tile removed — new
`static/icon-cards.svg` + one `.title-icon` CSS rule — Patrick's tie
from the home screen to the app name; browser- and wrapper-verified,
www/ diff-identical. CODE-FACT correction: www/ lives INSIDE the
inner source folder as an Xcode 26 synchronized-group explicit
folder, not beside the .xcodeproj as the #81 note said. Full detail:
upgrade-scope.md "Built — session #84".

**#85 (2026-07-13, "Dressing 3/3"): DRESSING IS COMPLETE — iPhone-only
+ the portrait lock, both Patrick's hand in Xcode, both
pbxproj-verified.** NEW DECISION: the app is iPhone-ONLY on the store
(device family was Xcode's default 1,2,7; iPad, Apple Vision, and Mac
destinations removed; `TARGETED_DEVICE_FAMILY = 1`, Catalyst off,
both configs — also sidesteps Apple's Requires-Full-Screen rule for
orientation-locked iPad apps). PORTRAIT LOCK set (Landscape
Left/Right unchecked; `...Orientations = Portrait` both configs) and
**Patrick-proven in the simulator — rotated, it held portrait.** The
HTML's own landscape block untouched (#71 stands). INCIDENT, cleanly
recovered: the wrong minus button (TARGETS-list one, not the
Supported-Destinations one) deleted the WHOLE TARGET; verified via a
sandbox copy of the repo (no git commands in the repo) that HEAD held
the healthy pbxproj and only that file differed; Xcode quit; Patrick
`git restore`d it. Trap + detail in upgrade-scope.md "#85". DUST left
on purpose: the inert `...Orientations_iPad` key stays. Today's whole
disk footprint: project.pbxproj (+ the docs refresh).

**#86 (2026-07-13): the REAL-DEVICE CHECK — the app RUNS ON PATRICK'S
ACTUAL iPHONE, end to end.** First device run (only hiccup: the phone
needed picking in the destination list; trust + Developer Mode were
already in place from the Memory app's runs). ALL THREE simulator
threats dissolved on real hardware — header-title wrap, grid fit, and
the Notes keyboard push are NOT present on the phone (per the #85
rule, nothing to do for them; closed). DICTATION into Setup's text
fields WORKS — the #78 prediction held, nothing built. The phone
surfaced three real items, all fixed and phone-proven the same
session: Out button lost after Log/Notes/Guide (the three "Game →"
returns restored only New — now restore Out too); card names now
12px NORMAL weight, was 10px bold (the #82 design-talk item closed
with no column widening — "Conservatory" fits); grid horizontal push
stopped (`.grid-wrap` overflow-x:hidden; vertical untouched). The
quirk queue is EMPTY. Full detail: upgrade-scope.md "Checked +
built — session #86".

**#87 (2026-07-14): pending.txt + the TEST-DOC EVALUATION.** NEW
`MysteryCluesTracker/docs/pending.txt` — a plain-language "what's
still left" list in the elderlyassistant style, this app only
(Patrick's ask; refreshing it joins the session-end docs routine).
Verified on the way: the three #72 delete-at-commit files are already
gone from disk. THE TEST-DOC HALF of #87's goal is DONE: the web's
test doc located (`MysteryTracker/docs/mtr-master-test-v2.docx` —
REPO COPY STALE at 203 steps; Patrick's current draft is 267 steps,
session upload; he updates the repo copy himself). All 22 sections
read, mobile facts code-verified. VERDICT: the format (5-column
tickable table, sections, tally) and the scripted-game spine transfer
beautifully; content is half adapt (the play sections, 🏠, Player
Out, New Game, Guide), a quarter drop (category moves, right-click
manual marks, theme, keyboard steps — mobile deletes, never mutes), a
quarter write-new (Welcome modals, templates, guards, Σ picker, Cell
Notes, Notepad, native Log Copy, status strips, 💬, wrapper
behaviors). Full detail: upgrade-scope.md "#87". The SPEC-doc half
was NOT reached — still open, tracked in pending.txt.

**#88 (2026-07-14): THE MOBILE TEST DOC IS BEGUN.** New
`MysteryCluesTracker/docs/mcts-master-test.docx` — the web's 5-column
tickable format; cover carries a no-affiliation line; 25-section map
agreed (app-flow order; web §2/§14/§19 dropped; the web 3.12
Clue-names note carried into §3; new mobile-only sections incl.
wrapper checks). SECTIONS 1–5 WRITTEN (53 steps), each from
code-verified facts, wording approved and written on Patrick's go.
The doc is GENERATED by new `docs/build-mcts-test.js` — extend the
script, don't hand-edit the docx. Two app changes along the way, both
browser-verified, www/ diff-identical: default category names now
show as grey placeholder like the card rows (Claude); the Edit-modal
refusal hint restyled red/bold so it's seen (Patrick's hand). CAST
DECIDED: players go by their own short names (Patrick's family
convention) — Ann, Bob, Me, Dan. CODE-FACT correction: player-name
max is 6 (the "13" banked in #87 is the category/card limit). NEW
CONDUCT RULE in CLAUDE.md rule 2 (#88, both connected copies;
elderlyassistant + MysteryTracker copies still need it): a go exists
only after Claude asks "Go?" as its own question and Patrick answers
it. Full detail: upgrade-scope.md "Built — session #88".

**#89 (2026-07-14): SETUP COVERAGE CLOSED — sections 6 and 7 written,
71 steps.** §6 (Players & the Me Seat, 9 steps) and §7 (Card Pick,
Play Button & Messages, 9 steps — `setupUnmet`'s condition order
code-verified), each wording-approved and written on Patrick's go.
NEW APP CHANGE from Patrick's own test pass (he runs the doc on the
phone as it's written): **Clear in the player popup now clears the
"This is Me" check too** — one line in `clearPlayerInput`;
browser-verified, www/ diff-identical; THE PHONE NEEDS AN XCODE
REBUILD to get it (step 7.2 depends on it). Doc improvements, all
Patrick's asks: "Start: …" state lines in the section banners (§1–8;
a new `start` field in the script), 0.75" side margins, columns
0.45/0.45/2.58/2.58/0.94, 10pt table text, padding in the three text
columns. Turn titles renamed to the cast (§9 Ann/Bob, §10 Bob/Me,
§12 Dan). OPEN: Me's hand is a placeholder (Card 1/2/10 — the
minimum that unlocks Play); the real deal gets settled when §8–9 are
drafted, adjusting 7.5–7.9 to match. Full detail: upgrade-scope.md
"Built — session #89".

**#90 (2026-07-14): THE GAME IS DESIGNED AND §8 IS BUILT.** The whole
scripted game settled in one sitting (Patrick's calls): default card
names all around; a 21-card deck, 3 categories, 6/6/9 (the trim drops
Card 7–9 and 16–18); the deal is his FAMILY WAY — 3 in the envelope
(Card 6/15/27, the last of each category), 4 per hand, 2 face down on
the board (Card 5/26) — full ledger plus all eight turn designs in
upgrade-scope "#90", each walked against the code (round one: every
shower first-in-ring, incl. the preselect modal and the envelope
nobody-shows; round two: the guards — asker-can't-show + first
auto-❌ passers T5, must-show-first T6, no-preselect modal + the Undo
test T7, all-crossed + repeat nobody-shows T8). PREMIUM-REUSE
PRINCIPLE logged (Patrick): the free script doubles as the paid
tier's future answer key — the ledger lives in the doc, turn-end
states stay explicit; the family deal also makes card counts
derivable (the #76 open idea). §8 BUILT as "Game Prep & Layout Check"
(12 steps; the doc stands at 83): prep rebuilds the game from ANY
state (Patrick's design — no leftover-state tracking; §7's
placeholder hand stays; the #89 open item closes), then seven
look-only layout checks. 8.12 reworded from Patrick's phone run (21
rows fit his screen — no scrolling). AGREED, unbuilt: Appendix A —
the deal + turn sequence, after §25. Parked: the skip-turn and
"Prev Turn?" tests still need homes. Full detail: upgrade-scope.md
"Built — session #90".

**#91 (2026-07-15, "sections 9–12" — Patrick revised the name mid-way;
§13 moved to #92): APPENDIX A + FOUR SCRIPTED TURNS BUILT — the doc
stands at 107 steps.** Appendix A first (Patrick's call after asking
whether it would help): the deal table + the eight-turn table
rendered after §25, the tester's face-up view of the #90 designs.
Then §9–12, 24 steps — T1 Ann→Bob shows, T2 Bob→Me shows (preselect
modal), T3 Me→Dan shows (no-preselect modal, first earned ✅), T4
Dan asks the envelope→nobody shows (auto-advance) — each drafted
from code-verified facts, wording approved, built on Patrick's go,
render-checked. Doc-wording conduct (Patrick): draft steps only, no
test explanations; the Make-sure column observes, never directs.
RIDE-ALONGS: pending.txt trimmed twice (the stale web test-doc copy —
Patrick had done it; the #88 "Go?" rule into the elderlyassistant +
MysteryTracker CLAUDE.md files — checked on Patrick's ask, both
still old, FIXED on his go: all four copies now match). Conduct
notes: status reports not verdicts — Patrick decides; brevity must
not drift terse (rule 5 covers it; a sharpening line was offered,
declined). Full detail: upgrade-scope.md "Built — session #91".

**#92 (2026-07-15, "gameplay section 13"): THE GUARD TURNS ARE BUILT
AND THE SCRIPTED GAME IS COMPLETE IN THE DOC — 138 steps.**
Mid-session restructure (Patrick's call, on the web doc's precedent):
each guard turn got its OWN section, §13–16 (First Passers /
Must-Show-First / the Undo Test / the Envelope Again), the sections
after renumbered 14–25 → 17–28 (the map now runs 28 sections),
Appendix A's turn table repointed. 31 new steps, each turn
code-verified, wording-approved, built on Patrick's go, and
PHONE-TESTED by Patrick as it was written; his test-pass corrections
folded in (Card 11's doubled "?" — ask marks are permanent records;
the Undo arm/disarm split). TWO CODE ITEMS QUEUED, found by Patrick's
phone runs: the 15.5 hint-line discrepancy (showing-phase hint
survives the Shown-Me confirm; diagnostic ready) and the "checked
card" message-wording hunt. Full detail: upgrade-scope.md "Built —
session #92".

**#93 (2026-07-15, "gameplay bug fixes"): BOTH #92 CODE ITEMS ARE
CLOSED, each browser-verified by Patrick.** (a) The HINT LINE FIXED —
the #92 note's placement ("after the Shown-Me confirm") was WRONG;
Patrick's #91 report was the true one: the wrong hint appeared the
instant Me's 3rd pick was clicked, because Me's showing-phase hint
was a longer line that clipped mid-word (static hints never scroll)
— no reason for Me's wording to differ. One line in updateStageHint:
every player's showing phase now reads "Tap the column header of who
showed." (b) The MESSAGE-WORDING HUNT DONE under Patrick's rule
(stated #93): "confirmed" in words is fine as long as it's
consistent; never "checked" in place of ✅, never "cross"/"crossed"
in place of the red ❌. One change — the nobody-shows message is now
"Nobody showed — cards are ❌-ed out" (Patrick's wording); the
"confirmed card" pair and the Guide's 🏠 sentence ruled fine as-is.
www/ re-copied, diff-identical; THE PHONE NEEDS AN XCODE REBUILD to
get both fixes. Full detail: upgrade-scope.md "Built — session #93".

**#94 (2026-07-15, "gameplay sections 17, 18 & 19"): TEST DOC
SECTIONS 17–19 WRITTEN — the doc stands at 163 steps.** §17 🏠 House
Column (8 steps — both board cards checked; the exact-revert proven
on Card 5's row: the untap removes only the house-placed ❌s and
leaves Bob's passer ❌ and Me's turn-0 ❌ alone), §18 Σ Popup Picker
(8 — modal anatomy, overwrite, the two-tap Clear; ends ✕ on Card 2,
⭐ on Card 6), §19 Cell Notes (9 — Set saves in place, edit on
reopen, BOTH exits per Patrick's own run: Clear → Done and
Set-with-empty-box → Close; P5 ghost tap does nothing; the 6-char
cap stays parked for §27). Each section code-verified,
wording-approved, built on Patrick's go, render-checked, tested by
Patrick as it was written. RIDE-ALONG: the five #93 wording
alignments in already-written sections — 12.4/16.5 "cards are ❌-ed
out", 11.3/15.3 the collapsed hint, 15.5 names the waiting hint (the
#93 follow-on settled); render-verified, zero old wording remains.
No app code touched. The phone still needs the Xcode rebuild for the
#93 fixes (and #89's Clear). Full detail: upgrade-scope.md "Built —
session #94".

**#95 (2026-07-16, "gameplay sections 20 & 21"): §20 AND §21 ARE
WRITTEN — the doc stands at 180 steps — plus TWO APP CHANGES.**
Scope was §20–21 only (Patrick's call; §22 and the message
discussions moved to #96). Correction on arrival: the #94 "phone
needs the rebuild" note was stale — the phone was current and all
prior tests ran there. APP CHANGE 1 (Patrick's ask): the Notepad got
its own status strip between the 📝 title and Clear — found while
banking §20 facts: `showStatus` had NO outlet on the Notes screen,
so the Clear two-tap's "Tap again to confirm" showed nowhere;
browser- and phone-verified. §20 Notepad (9 steps) written; 8.5
reworded to name the app name in the gold header (which tops every
screen — code-verified). FINDING at §21: Undo never touched the
log — §15's sequence left two identical Turn 7 entries. APP CHANGE 2
(Patrick's design, HONEST HISTORY): the undone entry STAYS and the
Undo itself is logged — new `undo` entry type ("Turn N — ↩ Undo —
turn restarted" / "All Turn N marks removed." / "∑ marks, Player Out
records and 👋-placed marks are not undone."), in render and Copy;
the completion message is now just "∑ and Player Out marks not
undone." Browser-proven incl. Patrick's Copy paste test. §21 Log &
Log Copy (8 steps) written — the exact scripted-game log
reconstructed; 21.7 pastes the copied log into the app's own Notepad
(no outside app needed); 15.8 aligned to the new message. PHONE
STATUS: §20–21 phone-verified incl. the new strip; the Undo message
+ Log undo entries are browser-proven only (no §20/§21 step fires an
Undo — they meet the phone at 15.8 on a full pass); the phone build
stays as-is until after #96. Conduct note: "diff-identical" is
jargon — say it plainly. Full detail: upgrade-scope.md "Built —
session #95".

**NEXT SESSION'S GOAL (#96): test doc §22 Player Out, plus the three
queued MESSAGE items:** (1) status messages that duplicate what the
turn bar already says (15.5's "Ann showed you Card 2" beside "Turn 7
— Ann ... showed ✓" is the named case, from #94); (2) some red-letter
messages are hard to read (#95); (3) the Setup screen's bottom
messages should be black lettering on a light background (#95). At
listing time: confirm "Mystery Clues Track Sheet" is available. The
paid-tier design/build (upgrade-scope.md "Decided — session #76")
waits until the free product is finished.

**Commit status (#95): Patrick's commits, when ready.**
MysteryCluesTracker: mystery-clues-tracker.html + the wrapper's www/
copy (the Notepad strip + the Undo log), docs/build-mcts-test.js +
docs/mcts-master-test.docx (§20–21, 8.5, 15.8), docs/upgrade-scope.md
(#95 section), docs/pending.txt — plus the #93 pair and the #88–92
batch if not yet committed. App-Docs: this file. elderlyassistant and
MysteryTracker: CLAUDE.md (the #88 "Go?" clarification), if not
already committed.

**Loose ends:** Memory's #69 badge-reorder commit/build/phone-check may
still be pending — confirm with Patrick. The elyfont.com home card
mis-describes the web app (says book-reading; it's a board-game
companion). The 266-step test procedure as a tickable web page remains a
liked idea. App-Docs git status: a .git folder exists (verified by
looking, no git commands run) — whether the GitHub repo + first commit
happened is unconfirmed; ask Patrick. NEW (#72 second sitting):
CLAUDE.md + session-start.md now
exist in all three project folders; Patrick's opener line: "#NN — name.
Read CLAUDE.md, session-start.md, and the hand-off, then tell me where
things stand."

## At session end

Claude refreshes this file's "Where things stand" + the strategy doc's
"Next session — start here" note, and the active project's own docs.
Patrick commits (this repo and any project repos touched).
