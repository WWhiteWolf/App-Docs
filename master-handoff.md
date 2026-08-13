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
   Y-25 (2026-08-12) put every sentence the app says to the player on
   paper, in `docs/message-map.md` — the words, the file and line, and one
   sentence saying what puts each on screen — built from a full read of
   both files. No app code was touched. Two things it settled: the engine
   holds the bulk of the talking and hands its words to the page through
   the `status` hook, and some sentences exist twice on purpose, the page
   refusing a wrong move at the front door and the engine again at the
   back, so a paired sentence must be changed in both files together.
   Patrick ruled the pass is a hunt for a few stray lines, not a mass
   edit, and that "3 or 0 should not exist"; nine candidate strays are
   listed in the project's hand-off, none ruled on. He also said he wants
   a function map of the rebuilt code, as he has for the old one — raised,
   weighed, and deliberately shelved so the wording could go first.
   Y-26 (2026-08-12) began the wording changes and settled five of the
   nine: the half-made ask now says all or none rather than "3 or 0",
   the counts refusal says the numbers do not match rather than reading
   backwards, the Undo line was removed outright as a thing said too
   often to be worth saying, the Play gate's seven refusals dropped
   their "Play needs:" prefix for "You need to", and the three
   sentences describing an empty-table ending were made to agree that
   it is a win. The ⭐ was confined to the glowing turn-bar win, which
   became "⭐ You Won!". The durable part is the standard Patrick ruled
   and had written into `docs/message-map.md`: a message earns its
   place by saying at a glance where the game stands, or why something
   was refused, and the division is by when it speaks rather than what
   it says — a line waiting on screen orients, a line firing after a
   move to restate a rule already followed does not. The same session
   got the engine's test suite running under Node in Claude's sandbox,
   so every change was tested as it was made. 179 tests, all passing.
   The phone is owed both changed files.
   Y-27 (2026-08-13) finished the wording pass. The last four strays and
   all four extras are settled: the no-show line became "No player showed
   — those cards are ❌-ed out for them", the New Game window was reworked
   whole into "Select how you want the Setup to start in the new game."
   and "The results of this game will be erased and forgotten. Your notes
   will be kept.", the Feedback window lost all four question numbers so
   its rating line stands as the fifth of five (the email it sends stays
   numbered on purpose), the board marks became "Rope is on the board"
   and "Rope board mark cleared" with the Turn Log brought into line, and
   being shown a card now names who showed it. The must-show-first
   refusal, which had been typed out twice in the engine, was made to
   live in one place — the session's only structural change, and named as
   such before it was made. Nothing in the app's own messages is
   outstanding; the Player Guide was deliberately never part of it.
   The session's other outcome was a ruling about the message map itself.
   A script found about a hundred of its line numbers wrong, and the map
   turned out to have been stale since Y-26 rather than only since that
   morning — Claude reported the damage as smaller than it was, and
   corrected itself once the script had looked. Patrick ruled that
   keeping it by number is the wrong way in the first place, a number
   being a position rather than a name, and proposed the replacement
   himself: the message map points at the function a sentence lives in,
   and the function map he has wanted since Y-25 says what each function
   does. Neither carries a number, so neither goes stale. The numbers
   were left wrong on purpose, since correcting them is work the rebuild
   throws away.
   179 tests, all passing, run in the sandbox after every change.
   Y-28 (2026-08-13) began the function map and wrote its engine half
   whole, touching no app code. The old map was read first, as Patrick
   asked, and its shape taken: lettered families of plain-English
   entries, one per function. The new one lives at
   `docs-ref/function-map.md`, carries no line numbers anywhere, and
   comes in two parts because the rebuild is two files — Part One the
   engine, Part Two the phone page, not yet written. Patrick left the
   shape to Claude, the document being for Claude's use, on the one
   condition that it stay readable by him; the engine and the page were
   kept apart so the engine half stands untouched when a second
   packaging is finally given the rebuilt page. Part One runs fifteen
   families following the engine's own section banners, with the public
   door, the hooks, the state, the storage keys and the limits ahead of
   them. Two things the reading turned up: the two private pickers'
   fallback card lists can never be reached, and turn zero is why; and
   whether "Nothing to undo" can ever fire was left open, since it
   depends on the page. The same session flipped the color hold. Patrick
   had built a tuner kit outside the project folder and sent it to his
   designer friend, so the Y-22 position reverses — she no longer waits
   on us, we wait on her. The hold on us covers anything to do with the
   colors she is working with, values as much as names, because her file
   lands as a clean replacement of the whole record; she has not
   started; she will not be changing names; and the hold lifts when she
   sends the download, which Patrick hands over to be plugged in.
   Y-28 also settled that there will be two test specs rather than one.
   The existing spec belongs to the old app and stays frozen beside
   `locked-mcts.html`; a new one gets built for the rebuilt app, over
   several sessions of its own. That overturns the Y-26 note about
   extending the one script, and it means the old spec's "drift" was
   never a fault — it and the locked HTML describe each other exactly.
   Left unruled at Y-28: the standing law in the project's `CLAUDE.md`,
   which still described extending and regenerating what is now a frozen
   document.
   Y-29 (2026-08-13) finished the function map. `mystery-phone.html` was
   read end to end and Part Two written whole — sixteen families, A
   through P, following the page's own banners, with the hooks, the five
   screens, the thirteen windows and the page's own three storage keys
   ahead of them, and each window described where its functions live.
   The thread Part One left open is closed: "Nothing to undo" cannot be
   reached from the phone page, because the page dims its Undo button
   dead on the same three conditions the engine refuses on. Patrick then
   stated the rule that governs the rest of the rebuild — the rebuild
   explains itself on its own terms, and nothing of the old build comes
   across, not in its documents, not in a sentence of comparison, and
   not as code that can no longer run. Three sentences left the function
   map under it. The old test document is not caught by the rule: it is
   kept, frozen and dedicated to the old app, and never bleeds into the
   new one's record. The Y-28 law was then rewritten into three bullets
   — the new document is generated by a script and never hand-edited,
   there are two documents each dedicated to one app, and the automated
   tests are described in the new one as well, the account of them
   rather than the test files; which moves the headless runner's recipe
   out of the churning hand-off and into the test document when it is
   built. Patrick left the generated-or-not decision to Claude. The rule
   then reached the three unreachable places Part One had recorded: the
   two private pickers' fallback lists are gone, and the "Nothing to
   undo" guard stays by Patrick's ruling, because the only reason it
   cannot fire belongs to the page and the heart never relies on a
   packaging to protect it. 179 of 179 tests pass, run after the edit
   and again after the wrapper copy; the wrapper's own engine copy was
   re-copied and verified identical, and the phone is owed the new
   engine. Found and recorded but not acted on: the Player Guide's words
   have drifted from the app in several places, which belongs to its own
   rewording session. Patrick's clean-start rule has no permanent home
   in a rules file yet.
   Next, in order: the message map rebuilt around function and window
   names; the Guide's rewording (Y-12), always its own session; and the
   new test spec.
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
