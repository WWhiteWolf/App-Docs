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
   the phone: the engine complete at 179 tests, both themes
   settled (Y-6), and every screen of `mystery-phone.html` built
   and phone-verified through the wrapper, which opens the
   rebuilt page (Y-9). Y-14 (2026-08-09) installed Patrick's
   tuned palette through the record, the page and the wrapper.
   Y-15 (2026-08-10) settled the color-naming law and the names
   on paper without touching the page. Y-16 (2026-08-10) closed
   the docs gap, so `docs-ref/build-history.md` now runs unbroken
   from #73 through Y-17 and `docs/handoff.md` carries continuity
   only. Y-17 (2026-08-10) checked the naming record before
   building on it and corrected it — twenty-six new names, not
   twenty-two, taking the app from seventy-five to a hundred and
   one — and settled that no further color list is wanted: the
   values are recorded permanently in `docs/palettes-tuned.css`
   and the names, purposes and grouping in `theme-tuner.html`.
   No names were applied. Y-18 (2026-08-11) went entirely to the
   session tooling — the rules moved to the `Projects` root and the
   opening became two folder asks — and did not touch the app.
   Y-19 (2026-08-11) applied the naming pass whole — all twenty-six
   names into the page, the record, the wrapper and the tuner,
   verified row for row, nothing changed to the eye by design.
   Y-20 (2026-08-11) built the feedback popup behind the Guide's
   Suggest button and woke the button, cured the tuner's download
   of its two dropped names, and reordered the ruling record, the
   page's palette blocks and the wrapper copy into the tuner's
   output order so downloads land line-identical.
   Y-21 (2026-08-11) passed that phone test with one wrinkle, cured
   the same session: the Log's status strip never took itself down
   and covered the footer buttons, because `statusTokens` carried no
   `log` or `notes` key. Then the cross-cutting colors were split on
   Patrick's ruling — `--lines` and `--faded` retired, fourteen
   per-section names in, fifty CSS spots repointed, 101 names to 113
   — the tuner was grown to show the side pages and the feedback
   popup and given a four-section chooser so all 111 pickers finally
   paint something, eighteen tuned light colors were installed, the
   tuner's embedded defaults were brought up to the record (closing
   the standing lag note), and the Setup seats lost their redundant
   third line. `theme-tuner-kit.zip` went by email to a designer
   friend of Patrick's, who is tuning the colors.
   Y-22 (2026-08-12) began the layout polish, to the standard Patrick
   named out loud — he wants the app to look and feel smart. The Setup
   seats went from three rows of two to two rows of three, same height
   and narrower, in one CSS rule. The card counts now carry through a
   New Game when Same Players and Same Deck are both chosen, on
   Patrick's reversal of his own earlier rule: the counts belong to the
   group and its deck rather than to the deal, while the hand still
   starts empty because a fresh shuffle really does change it. The
   "Where are the cards?" button borrows the card chips' picked colors
   to show when the counts are set, so no new color name was added and
   the designer's file still installs as a clean replacement. The suite
   is at 179 tests, all passing. One wrinkle was found in the browser
   and deferred by Patrick: the highlight outlives a close and open of
   the app, and his rule is that the set condition survives a New Game
   only.
   The detail lives in the project's own docs.
   Also settled at Y-22: the designer waits on us now rather than the
   other way about. She has been asked to hold until the layout polish
   is finished, so that one kit is built once after the page has stopped
   moving. He then deleted every copy of `theme-tuner-kit.zip`, the
   tracked one included, so no kit is kept in the repo — it is rebuilt
   from the project's own files when there is something to send, and the
   recipe is recorded in the project's hand-off.
   Y-23 (2026-08-12) cured the counts wrinkle and settled the rule
   behind it after two reversals: the counts' numbers carry through a
   New Game when Same Players and Same Deck are both chosen, the
   settled flag does not, and tapping Done is what settles them — so
   nothing can return from a close and open claiming to be answered
   for. The numbers are saved because they hold how a table plays,
   spares in a house or dealt round the players, which no guess can
   know; a first game gets the guess, an even share to the players and
   the leftovers to House, always offered. The same session set the
   Game grid's default column order to Cards, ∑, 🏠, then P1 through
   P6, and raised the Next button into one tall block standing at the
   right of both bars, its outline shared from `--turn-bar-text` on
   Patrick's ruling — so the app stays at 113 names and the designer's
   file still installs clean. 179 tests, all passing; both Game-page
   changes seen and approved in the browser.
   Y-24 (2026-08-12) made the Game grid's lines uniform, which turned out
   to be a phone problem rather than a color one: the browser had always
   looked right. Every cell now draws only its own right and bottom line
   and the table no longer collapses touching edges, so no two cells share
   a line for a dense screen to round two different ways. The stage bar
   keeps the top edge, the left edge is closed at the card column, and the
   category banners draw the line beneath themselves. The ∑ and 🏠 shade
   Patrick had already tuned was written into the files, keeping the name
   alive so the app stays at 113. He loaded it and confirmed the grid and
   the Setup are both where he wants them, so the phone is current and no
   device is owed anything.
   Next, in order: the message-wording pass (Y-10), which Patrick called
   at Y-24 and deliberately left for a stronger model; the Guide's
   rewording (Y-12); the generated master test document, unchecked
   against Y-23 or Y-24; and then the rebuilt kit to the designer and her
   palette back.
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

- **Where the session rules live, settled at Y-18.** The conduct
  rules are `Projects/CLAUDE.md`, at the root of the parent folder.
  That location is the whole point: a `CLAUDE.md` arrives on its own
  only when it sits at the root of a *connected* folder, and the old
  `App-Docs/CLAUDE.md` sat a level below and so never did. Each
  project keeps its own `CLAUDE.md` for its own laws, and none of
  them is duplicated at the root. `App-Docs/CLAUDE.md` is deleted.
  The `Projects` root is a git repository of its own, added at the
  end of Y-18 so the rules file keeps a version history.
  `Projects/.gitignore` lists all four project folders, each already
  a repository, so the root one tracks only the loose files at its
  own level and never nests.
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
  project's pending list updated (Patrick, MT#7) — pending goes
  stale on major decisions and new docs files, not just code
  changes. If yes: header line first. The pending.docx reading
  copies are retired (Y-1) — the pending list is Patrick's direct
  read, shown large. **Settled at Y-22:** in `MysteryCluesTracker`
  that file is `docs/pending.rtf`. Rich Text is deliberate, because
  RTF stores the font size inside the file so the large type travels
  with it, where plain text leaves the size in TextEdit's own
  preferences. Patrick ruled that the docs change to match the file
  rather than the other way about. Whether Memory's own pending list
  is `.txt` or `.rtf` is unchecked — that folder was not connected
  at Y-22, so the reference to it above still reads `.txt`.

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
