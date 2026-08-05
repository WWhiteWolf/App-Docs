# Master hand-off — cross-project state (all projects)

App-Docs (this folder) is the single home for cross-project
docs (Patrick's decision, #71). It is a git repo; Patrick makes
every commit. Keep this file to four things only: the projects
and their folders, one line of status each, what is true across
all three, and the loose ends belonging to no single project.
Session history lives in the projects' build-history files.

## The projects

1. **Mystery Tracker — web** — live at elyfont.com, Beta.
   Folder: `Projects/MysteryTracker`. Status: MT#6 is COMMITTED,
   confirmed at MT#7. MT#7 (2026-08-05) completed the mobile-v-web
   comparison (`docs/MT7-comparison.md`) and produced the rebuild
   decisions list (`docs/MT7-rebuild-decisions.md`); those docs and
   the hand-off await Patrick's commit. Working direction (Patrick,
   not yet a formal commitment): one shared game heart, separate
   mobile and web packagings, UI converged where it makes sense.
   Next: settle the decisions one per sitting, deck shape first.
   The theme work still waits behind the plan.
2. **Mystery Clues Track Sheet — mobile, App Store, FREE.**
   Folder: `Projects/MysteryCluesTracker`; read
   `docs/upgrade-scope.md` first. Status: awaiting Apple's
   answer on build 1.0 (2); the Android APK is built, signed
   and phone-proven (#155), its repo upload and elyfont.com
   download page pending. Its standing habits live in its own
   CLAUDE.md and docs/handoff.md.
3. **A Place To Remember (Memory) — iPhone** — Alpha.
   Folder: `Projects/elderlyassistant`. Status: #3-new is
   phone-verified and committed; next is #4-new — the three
   "What's Next" items in pending.txt.
4. **Memory — web** — DROPPED (#72). elyfont.com gets a pointer
   to the App Store listing only.

## True across all three

- The three chains: bare numbers or "MCTS" are the old shared
  chain, "#nn-new" is Memory, "MT#nn" is Mystery Tracker. No
  old reference is ever edited.
- The build-and-test commit rhythm: the code commit comes
  before the build, the docs commit after the device test — so
  at a session start the code should be committed but the docs
  may lag. If the docs say "awaiting test," ask how it went.
- `Publishing-Strategy.docx` is the north star for
  publishing/business sessions. It is updated only when
  something moves the strategy (Patrick, #146) — not at the
  routine refresh.
- At session end: the docs refresh gets its own rule-8 go,
  every time. Claude scripts the opener note — it begins with
  Patrick's line "#NN — name. Read CLAUDE.md and the hand-off.",
  carries the folder asks, and closes with one line of working
  rules — and hands it as its OWN message, with a commit text
  for each repo touched (summary line about 50 characters, any
  more as a body below).
- If a project's pending.txt changed, bring its header line up
  to date first, then rebuild pending.docx to match,
  machine-checked line for line (#128, #1-new).

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
