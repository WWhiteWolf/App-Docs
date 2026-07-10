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

## Where things stand (updated 2026-07-10, session #72)

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
   held — the toolchain is ready.
3. **A Place To Remember (Memory) — iPhone** — Alpha, mostly built.
   Project: `Projects/elderlyassistant` (its own session docs:
   docs/handoff.md, pending.txt, parked-items.md, session-start.md).
   Store prep comes after the Mystery rehearsal. Android version
   eventually, after the iPhone build (decided #72).
4. **Memory — web** — DROPPED (decided 2026-07-10, session #72): no web
   version. The app is built around the rich reminder scheme, which the
   web can't carry. elyfont.com gets a pointer to the App Store listing
   only.

**NEXT SESSION'S GOAL (end of #72): the mockups.** Configurable setup
(1–4 categories, 1–30 cards, player-named), ✓/✗ cell tinting, the 🏠
column (manual marks only), tier-gate removal (auto-Σ comes OUT with
it — no-thinking directive), and the portrait/landscape question —
all in upgrade-scope.md.

**Commit reminder (Patrick, #72):** commit BOTH repos (App-Docs and
MysteryCluesTracker). At commit, delete the three dead files in
MysteryCluesTracker: `clue-manifest.json`, `static/clue-icon.png`,
`static/service-worker.js`. (Keep `MysteryTracker.html` — that's
Patrick's original hand-built Clue sheet, a keepsake.)

**Loose ends:** Memory's #69 badge-reorder commit/build/phone-check may
still be pending — confirm with Patrick. The elyfont.com home card
mis-describes the web app (says book-reading; it's a board-game
companion). The 266-step test procedure as a tickable web page remains a
liked idea. Patrick still owed: git init + GitHub repo + first commit for
THIS folder.

## At session end

Claude refreshes this file's "Where things stand" + the strategy doc's
"Next session — start here" note, and the active project's own docs.
Patrick commits (this repo and any project repos touched).
