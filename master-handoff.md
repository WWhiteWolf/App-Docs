# Master hand-off — cross-project state (all projects)

App-Docs (this folder) is the single home for cross-project
docs (Patrick's decision, #71). **The Reminder Engine's picture and
document no longer live here** — they moved to
`Projects/Reminder Engine/docs` at Reminder Engine 1, which is now that
project's home. It is a git repo; Patrick makes
every commit. Keep this file to four things only: the projects
and their folders, one line of status each, what is true across
them all, and the loose ends belonging to no single project.
Session history lives in the projects' build-history files.
This file is brought current at every session's docs refresh and
is never left to lag — a project's own docs hold the detail, and
this one holds where everything stands (Patrick, Y-15).

## The projects

1. **Mystery Tracker — web** — live at elyfont.com, Beta. Folder:
   `Projects/MysteryTracker`. Status: ARCHIVED (Y-1, 2026-08-07) — the
   finished archive of the old web app, opened only when something
   needs tracing. The Beta site stays as it is until the rebuilt web
   page replaces it.
2. **Mystery Clues Track Sheet — mobile, App Store, FREE — and the
   rebuild's home.** Folder: `Projects/MysteryCluesTracker`. Status:
   LIVE on the App Store since 2026-08-06, with the Y-chain rebuild
   whole on the phone at 179 tests; the live work is the Player
   Guide's rebuild, at Y-47 (2026-08-18).
3. **A Place To Remember (Memory) — iPhone** — Alpha, and it is on his
   phone. Folder: `Projects/elderlyassistant`. Status: the reminder
   engine is whole and live across the one saved list, 459 tests. Daily
   through Options are built. The automated load is built (#44-new,
   2026-08-31); the simulator sitting is done. Two engine Fails from
   that sitting (Daily after Done, named zone) are #45-new. He is
   living with the #37-new build on the phone.
4. **Students-Assistant — iPhone and web** — Alpha, and it is on his
   phone. Folder: `Projects/Students-Assistant`. Status: the new
   reminder engine is in and the live path goes through it (SA-21,
   2026-08-27), with 61 of 61 tests passing and `tsc` silent.
5. **Memory — web** — DROPPED (#72). elyfont.com gets a pointer to the
   App Store listing only.
6. **The Reminder Engine — not an app.** Folder: `Projects/Reminder
   Engine`, with a space. It holds the reminder design the two apps
   share by each having a copy, and there is no code in it and there
   is not meant to be. Status: Reminder Engine 4 (2026-08-28) settled
   the calendar fields and wrote the Memory build sheet; Cursor then
   built that sheet into Memory's scheduler, 413 of 413 tests.
   Students-Assistant's copy has not had this change.

## True across them all

- **Where the session rules live, settled at Y-18.** The conduct
  rules are `Projects/CLAUDE.md`, at the root of the parent folder.
  That location is the whole point: a `CLAUDE.md` arrives on its own
  only when it sits at the root of a *connected* folder, and the old
  `App-Docs/CLAUDE.md` sat a level below and so never did. Each
  project keeps its own `CLAUDE.md` for its own laws, and none of
  them is duplicated at the root. `App-Docs/CLAUDE.md` is deleted.
  The `Projects` root is a git repository of its own, added at the
  end of Y-18 so the rules file keeps a version history.
  `Projects/.gitignore` lists all five project folders, each already
  a repository, so the root one tracks only the loose files at its
  own level and never nests.
- **The root folder and its repository have different names
  (Patrick, SA-5).** The folder on the Mac is `Projects` and always
  will be, because both rules files, the session-opening procedure
  and every hand-off name it. Its repository on GitHub is
  `Build-root`, private, published at SA-5. Patrick chose that name
  because placeholders already named "Projects" sat in the account
  and had confused him once; the name says the place rather than the
  contents, since the repository holds only `CLAUDE.md`, the
  `.gitignore` and the few loose files at the root level. Nothing
  requires the two names to match.
- **Every project now has a remote (SA-5).** `Build-root` and
  `Students-Assistant` were the two without one, so until that
  afternoon their whole history existed only on Patrick's MacBook
  Air. Both are private. `Students-Assistant` could not be published
  from VS Code because an empty placeholder of that name already
  existed on GitHub, so it was connected to that placeholder from the
  terminal instead — thirty-one objects, `main` tracking
  `origin/main`.
- **Rule 22 no longer names Patrick's usage percentage (Patrick,
  Y-42).** Its closing sentence — "Patrick reports his usage
  percentage at checkpoints; fold it into stop-or-continue advice" —
  was struck from `Projects/CLAUDE.md`. His usage is a budget meter
  and not a quality one, and it is not the gauge for whether Claude's
  checking is thinning. He was sure the old meter goes, said he is not
  yet sure what replaces it, and asked for no placeholder. The rest of
  rule 22 stands untouched.
- **Rule 1 no longer tells Claude to report when a rules file did not
  arrive on its own (Patrick, #21-new).** Its closing sentence — "If a
  rules file did not arrive on its own, say so plainly before the
  status report instead of covering the gap quietly (SA-20)" — was
  struck from `Projects/CLAUDE.md`. The session had opened with exactly
  that report and it was false: both files had arrived and were in
  front of Claude from the first moment. Patrick said the same false
  sentence has appeared a dozen times in Students-Assistant, and his
  own argument closed it — reading a file by hand and having it arrive
  amount to the same thing once it is read, and how the file got there
  is plumbing he never asked to be kept posted on. The rule's own
  defence does not survive that: in a session where Claude never thinks
  to read the file it also never thinks to report, so the warning can
  only fire in sessions where nothing is wrong, and a warning that
  fires at random teaches him to stop reading it. **The two folder asks
  and the reasoning behind them stand unchanged** — the asks are what
  make the files arrive, and only the reporting went.
- **The opening asks for two folders, not one (Y-18, overturning
  MT#5).** The parent `Projects` folder first, then the folder of the
  session's goal, so that project's own `CLAUDE.md` arrives on its
  own as well. The first connection has to come from Patrick's opener
  note, since nothing is connected before it. His opener now needs
  only the two folders and the chain name and goal.
- The chains: bare numbers or "MCTS" are the old shared chain,
  "#nn-new" is Memory, "MT#nn" is Mystery Tracker. "Y-n" (no
  "#" before numbers) is the converged Mystery rebuild, begun
  Y-1 (2026-08-07); the MT and MCTS chains are closed as
  history. "SA-n" is Students-Assistant, begun SA-1
  (2026-08-19). No old reference is ever edited.
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
  project's pending list updated (Patrick, MT#7) — pending goes
  stale on major decisions and new docs files, not just code
  changes. If yes: header line first. The pending.docx reading
  copies are retired (Y-1) — the pending list is Patrick's direct
  read, shown large. **Settled at Y-22:** in `MysteryCluesTracker`
  that file is `docs/pending.rtf`. Rich Text is deliberate, because
  RTF stores the font size inside the file so the large type travels
  with it, where plain text leaves the size in TextEdit's own
  preferences. Patrick ruled that the docs change to match the file
  rather than the other way about.

  **Memory is now the exception, at Patrick's word (#31-new).** Its
  reading copy is `docs/pending.docx` again — a Word copy is what he
  wanted originally, one existed at session 0, and the rtf that
  replaced it at #12-new is retired to history. It is generated by
  `docs/make-pending-docx.py`, which proves it matches the txt word
  for word, and **it is generated when he asks for it, not on a
  schedule**: regenerating a file whose source has not moved is
  useless work. Memory's own source list is still `docs/pending.txt`.
  The Y-1 retirement of docx copies does not apply there.

  **His ruling behind that is general and worth carrying: write the
  condition, not the ceremony.** A rule saying what to perform does
  the work whether or not it is needed and fails silently the once it
  is skipped. A rule saying what must be true can be checked.

- **Sessions can run in Cursor as well as the Claude app (#30-new).**
  Cursor has the assistant built into the editor and the model is
  chosen per chat from the picker beside the message box, so one chat
  can be Claude and the next one Grok. The two folder asks and
  everything else in the opening procedure are unchanged. The detail,
  including which model suits which kind of work and how the two
  billing pools differ, is in `Projects/My-Tools-and-Extensions.md`.

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
- **This file was trimmed back to the four things its own header
  names** (Reminder Engine 3, 2026-08-28), from 3,003 lines to its
  present length. The check came first: every session named in the
  Mystery Clues, Memory and Students-Assistant entries was confirmed
  to have its own section in that project's build history before a
  line was cut. Two known gaps are recorded rather than lost —
  Memory's #14-new and #15-new have no build-history sections and
  live in `elderlyassistant/docs/reminder-rebuild.md`, and the App
  Store go-live date of 2026-08-06 lives in
  `MysteryCluesTracker/docs-ref/ROADMAP.md`. The pointers to each
  project's own CLAUDE.md and reads were dropped from the entries at
  Patrick's ruling.
