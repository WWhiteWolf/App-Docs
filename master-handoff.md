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

## Where things stand (updated 2026-07-11, session #77 — the Guide editing session)

**The products, all to be published (decided #71; Memory-web dropped #72):**

1. **Mystery Tracker — web** — live at elyfont.com, Beta. Project:
   `Projects/MysteryTracker` (its own session docs: SESSION-HANDOFF.md
   etc.).
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
3. **A Place To Remember (Memory) — iPhone** — Alpha, mostly built.
   Project: `Projects/elderlyassistant` (its own session docs:
   docs/handoff.md, pending.txt, parked-items.md, session-start.md).
   Store prep comes after the Mystery rehearsal. Android version
   eventually, after the iPhone build (decided #72).
4. **Memory — web** — DROPPED (decided 2026-07-10, session #72): no web
   version. The app is built around the rich reminder scheme, which the
   web can't carry. elyfont.com gets a pointer to the App Store listing
   only.

**NEXT SESSION'S GOAL (#78, named at #77's close): THE ROAD TO THE
STORE** — the Guide editing pass is done (#77), so the free-version
queue moves to the Xcode + WKWebView wrapper and the data-safety
bridge (upgrade-scope.md "The route to the store"). Patrick drives
Xcode, Claude assists; the toolchain has been ready since #72
(Xcode 26.6, Apple ID signed in, Dev account held). At listing
time: confirm the "Mystery Tracker" name is available (fallbacks
in upgrade-scope.md). Patrick confirms or redirects at #78's
start, as always. The paid-tier design/build (seven helpers, count
inference, gate mechanics — upgrade-scope.md "Decided — session
#76") waits until the free product is finished.

**Commit reminder (#77): commit App-Docs (this file) and
MysteryCluesTracker — this time the app itself changed:
`mystery-clues-tracker.html` (the Guide pass + feedback repairs)
plus docs/upgrade-scope.md. Still pending from #76 if not yet done:
MysteryCluesTracker docs (CLAUDE.md, pre74-tiering-reference.html
if kept) and elderlyassistant (CLAUDE.md + docs/session-start.md
tone rules). (Keep `MysteryTracker.html` — that's Patrick's
original hand-built Clue sheet, a keepsake.)

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
