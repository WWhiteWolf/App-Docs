# Master hand-off — cross-project state (all projects)

App-Docs (this folder) is the single home for cross-project
docs (Patrick's decision, #71). It is a git repo; Patrick makes
every commit. Keep this file to four things only: the projects
and their folders, one line of status each, what is true across
all three, and the loose ends belonging to no single project.
Session history lives in the projects' build-history files.
This file is brought current at every session's docs refresh and
is never left to lag — a project's own docs hold the detail, and
this one holds where everything stands (Patrick, Y-15).

## The projects

1. **Mystery Tracker — web** — live at elyfont.com, Beta.
   Folder: `Projects/MysteryTracker`. Status: ARCHIVED (Y-1,
   2026-08-07) — the finished archive of the old web app, its
   docs untouched, opened only when something needs tracing.
   The MT chain is closed as history; the rebuild lives in
   `Projects/MysteryCluesTracker` under the Y chain. The live
   site stays as it is until the rebuilt web page replaces it.
   The MT#6 theme colors still wait behind the plan.
2. **Mystery Clues Track Sheet — mobile, App Store, FREE — and
   the rebuild's home.** Folder: `Projects/MysteryCluesTracker`;
   its CLAUDE.md names the reads (`docs` is the active set,
   `docs-ref` the reference set). Status: LIVE on the App Store
   since 2026-08-06 (#157), and the Y-chain rebuild is whole on
   the phone: the engine complete at 177 tests, both themes
   settled (Y-6), and every screen of `mystery-phone.html` built
   and phone-verified through the wrapper, which opens the
   rebuilt page (Y-9). Y-14 (2026-08-09) installed Patrick's
   tuned palette through the record, the page and the wrapper.
   Y-15 (2026-08-10) settled the color-naming law and the names
   on paper without touching the page. Y-16 (2026-08-10) closed
   the docs gap, so `docs-ref/build-history.md` now runs unbroken
   from #73 through Y-16 and `docs/handoff.md` carries continuity
   only. The detail lives in the project's own docs.
   Next, in order: applying the settled color names, then the
   feedback popup behind the Guide's sleeping Suggest button
   (Y-13), then the Guide's rewording (Y-12).
   The committed Store version stays shelved
   byte-identical at `Projects/locked-mcts.html`. The Android
   legs wait until the merged app is done, and `wrapper-android`
   has never been given the rebuilt page.
3. **A Place To Remember (Memory) — iPhone** — Alpha.
   Folder: `Projects/elderlyassistant`. Status: #3-new is
   phone-verified and committed; next is #4-new — the three
   "What's Next" items in pending.txt.
4. **Memory — web** — DROPPED (#72). elyfont.com gets a pointer
   to the App Store listing only.

## True across all three

- The chains: bare numbers or "MCTS" are the old shared chain,
  "#nn-new" is Memory, "MT#nn" is Mystery Tracker. "Y-n" (no
  "#" before numbers) is the converged Mystery rebuild, begun
  Y-1 (2026-08-07); the MT and MCTS chains are closed as
  history. No old reference is ever edited.
- The build-and-test commit rhythm: the code commit comes
  before the build, the docs commit after the device test — so
  at a session start the code should be committed but the docs
  may lag. If the docs say "awaiting test," ask how it went.
- `Publishing-Strategy.docx` is the north star for
  publishing/business sessions. It is updated only when
  something moves the strategy (Patrick, #146) — not at the
  routine refresh.
- At session end: the docs refresh gets its own rule-8 go,
  every time. Claude drafts nothing at session end — no opener
  note and no commit texts; Patrick writes his own (Y-1).
- At session end, always ask Patrick whether he wants the
  project's pending.txt updated (Patrick, MT#7) — pending goes
  stale on major decisions and new docs files, not just code
  changes. If yes: header line first. The pending.docx reading
  copies are retired (Y-1) — pending.txt is Patrick's direct
  read, shown large by TextEdit's plain-text font setting.

## Loose ends belonging to no single project

- The Cowork "Projects" feature: explored, then parked; an
  accidental "App-Docs" project sits harmless in the panel, and
  whether a chat inside a project can connect a second folder
  is untested.
- elyfont.com home page: add a Mystery Clues Track Sheet card
  linking privacy-policy.html and support.html — both pages
  live, unlinked (deferred by Patrick, #130).
- The 266-step web test procedure as a tickable web page
  remains a liked idea.
