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
- Patrick leads; Claude doesn't steer. No urgency — his pace.

## Where things stand (updated 2026-07-10, session #72 second sitting — scope + mockups)

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
   finished — ships portrait-only).
3. **A Place To Remember (Memory) — iPhone** — Alpha, mostly built.
   Project: `Projects/elderlyassistant` (its own session docs:
   docs/handoff.md, pending.txt, parked-items.md, session-start.md).
   Store prep comes after the Mystery rehearsal. Android version
   eventually, after the iPhone build (decided #72).
4. **Memory — web** — DROPPED (decided 2026-07-10, session #72): no web
   version. The app is built around the rich reminder scheme, which the
   web can't carry. elyfont.com gets a pointer to the App Store listing
   only.

**NEXT SESSION'S GOAL (end of #72 second sitting): START THE BUILD.**
Scope is complete; upgrade-scope.md holds every decision. Build ONE
change at a time, each with Patrick's explicit go. A build order to
discuss with Patrick (his call): tier-gate removal (auto-Σ out),
asking auto-check removal, 🏠 column, ✓/✗ tinting, then the
configurable structure (setup screen, then in-play).

**Commit reminder (Patrick, #72):** commit BOTH repos (App-Docs and
MysteryCluesTracker). At commit, delete the three dead files in
MysteryCluesTracker: `clue-manifest.json`, `static/clue-icon.png`,
`static/service-worker.js`. (Keep `MysteryTracker.html` — that's
Patrick's original hand-built Clue sheet, a keepsake.)

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
