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

## Where things stand (updated 2026-07-12, session #78 — the pre-wrapper decisions session)

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

**NEXT SESSION'S GOAL (#81): the www folder-reference fix** —
Patrick quits Xcode; Claude moves `www/` beside the .xcodeproj and
hand-edits project.pbxproj to add it as a structure-preserving
folder reference; Patrick reopens and runs; the lettering gives the
verdict, and the temp diagnostic comes out of ContentView.swift once
fonts load. After that, in order: the data-safety bridge, then
dressing (display name "Mystery ✓", portrait-only lock, icon), then
phone + dictation checks. At listing time: confirm "Mystery Clues
Track Sheet" is available. The paid-tier design/build
(upgrade-scope.md "Decided — session #76") waits until the free
product is finished.

**Commit reminder (#80): commit App-Docs (this file +
CLAUDE.md) and MysteryCluesTracker (CLAUDE.md + docs/upgrade-scope.md
— the #80 doc updates). Everything else from #79 and earlier
is committed. (Keep `MysteryTracker.html` — that's Patrick's
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
