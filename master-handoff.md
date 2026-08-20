# Master hand-off — cross-project state (all projects)

App-Docs (this folder) is the single home for cross-project
docs (Patrick's decision, #71). It is a git repo; Patrick makes
every commit. Keep this file to four things only: the projects
and their folders, one line of status each, what is true across
them all, and the loose ends belonging to no single project.
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
   paper, in what is now `docs-ref/message-map.md` — the words, the file
   and line, and one sentence saying what puts each on screen — built
   from a full read of
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
   and had written into `docs-ref/message-map.md`: a message earns its
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
   Y-30 (2026-08-13) rebuilt the message map around names and touched no
   app code. Every line number is gone from it: two scripts located every
   message and named the function enclosing it, and mapped the markup so
   each piece of fixed text points at the window or screen box it sits
   in, so no pointer rests on an inference. The engine speaks
   thirty-eight times and the page fifteen, all inside named functions.
   An index at the foot reads the map the other way round, from a piece
   of code to what it says. The names showed things the numbers had
   hidden: the ask countdown is one sentence reached down two roads
   rather than two sentences, "Log copied!" is the same story, and
   "Select a card" is two homes rather than a line pair. No line-number
   pointer survives and all eighty-six names were checked against the
   source. Patrick then ruled that both maps are reference files, so
   `message-map.md` joined `function-map.md` in `docs-ref`; he made the
   move himself and five live pointers were repointed across three files,
   the build history's seven left untouched as history.
   The session's other outcome was the new test spec's shape, settled in
   outline by Patrick with not one step of it written: a new document in
   `docs-ref` beside the frozen old one, generated by a script and never
   hand-edited; the test steps a headed section standing empty; the
   message map's index in but not the map entire; the function map out
   altogether and referenced rather than copied; a test coverage map as
   an index of its own, pointing at both maps; the account of the
   automated tests in, which is what finally takes the headless runner's
   recipe out of the churning hand-off; and no color list, since a
   generated one would be the third list Y-17 ruled against. Everything
   in it is generated from its sources, so nothing copied can drift from
   what it was copied out of. `docs-ref/test-spec-styling.md` was read as
   reference only, and the rebuild gets a styling document of its own:
   its craft carries across, but its color claims cannot be true of an
   app with two themes and 113 names, and its shape is the old
   procedure's.
   Y-31 (2026-08-13) began the Player Guide's rebuild and touched no app
   code. What had been carried since Y-12 as a rewording turned out not to
   be one: Patrick ruled at the top of the session that the existing Guide
   is never edited, but left frozen where it already sits inside
   `Projects/locked-mcts.html` and used only as a reference while a new
   Guide is written from nothing. That was verified before anything rested
   on it — the Guide in the locked file and the Guide in
   `mystery-phone.html` are identical word for word, 117 lines of visible
   text each, so nothing is lost when the new one replaces the working
   copy. Everything about the rebuild lives in `docs/guide-rebuild.md`, a
   working file that moves to `docs-ref` when the Guide is finished. The
   standard is Patrick's and outranks the rest: a Guide a player wants to
   keep reading, with a thing earning its place by what the player
   actually needs rather than by what is true of the app — the same shape
   as the standard governing the app's messages, so the app now judges its
   words the same way in two places. Two sections are finished and agreed:
   the opening, which the old Guide never had and whose absence Patrick
   said had flown right over his head, and Setup entire. Both were written
   from the app as it is, every claim checked against the page and the
   engine first, which corrected several things the old Guide had said —
   the play gate has seven conditions and not five, ▶ Play sits at the top
   right, turn order is seat order, and marking a seat as Me discards the
   name. A quick road Patrick had proposed was withdrawn by him once the
   read showed the shipped deck is placeholders. Three rules came out of
   the session: show the whole screen before walking through any part of
   it; the Guide names a genre and never a game, a publisher or a
   character; and the Guide names colours plainly, dealing with the
   designer's tuning if and when it changes them. The working method
   changed mid-session as well — the opening was built a phrase at a time
   and Patrick said that at that rate the Guide would take dozens of
   sessions, so Claude now drafts a section whole and he reacts to it.
   Y-32 (2026-08-14) settled the Guide's section order and wrote the
   Game screen, touching no app code. Patrick ruled that the old Guide's
   section layout is good all the way through, so it is adopted whole —
   shape, which Y-31 had already set aside from the clean-start rule. It
   was read out of the locked file before anything rested on it, and it
   answers two Y-31 questions at once: the Game screen is two sections
   rather than one, and the Log and the Notepad fall near the end as the
   Setup introduction promised. What was adopted is the order, not the
   heading wording — those names are the old app's and are decided one
   at a time as each section is written. Patrick then noticed the layout
   covers no theme button, the old app having had no themes, so a short
   theme note now stands between the opening and Setup: the app arrives
   dark and one tap changes it. It is deliberately not a numbered
   section, being a comfort setting rather than a game instruction, and
   it goes up front because a first-time reader is looking at a dark
   screen they never chose. The Game screen itself was written whole to
   a goal Patrick set — the player should recognise the sheet from the
   ones the game manufacturers put in the box — and to an order he set
   with it: recognition first, then comfort, then instruction. That
   overturned the adopted layout's own sub-order, moving the grid from
   seventh to first with the marks beside it, since the grid is the
   thing the player recognises. The read forced three corrections: the
   marks are a plain ✓ and ✗ rather than the old Guide's ✅ and ❌; Undo
   wipes the whole turn rather than the last tap; and the player never
   marks a ✓ themselves, but names who showed and has the rest written
   for them. No colour is named anywhere in the section, because those
   values were never checked and the Guide's rule is to name a colour
   plainly or not at all. The Guide now has four agreed pieces — the
   opening, the theme note, Setup and the Game screen — and Taking a
   turn is next, the first section that has to teach rather than orient.
   Y-33 (2026-08-14) read the turn cycle end to end and drafted Playing
   a turn whole, touching no app code. The read covered both files and
   the ∑ and 🏠 columns with them, and its account is recorded so no
   session repeats it; it corrected four things a remembered draft would
   have got wrong, among them that a ! never lands in a box already
   holding a ✓ or a ✗, and that Undo is not the only road back after a
   show — a show between two other players can be taken back by tapping
   that name again, until Next ▶ is tapped. The draft is recorded and
   **not agreed**: it was stopped rather than finished, on Patrick's
   word that he was tiring of reading it and that a player would tire
   faster. Three rulings stand from it — pop-up is the Guide's word for
   these rather than window or modal, with three agreed lines changed to
   match; House comes before Summary, reversing the adopted layout,
   because the Summary cannot be reached without knowing what is on the
   board first; and a thing may be described by what it is not whenever
   that helps the reader, but the Guide never measures one part of the
   app against another. A fourth, that headings end with a colon,
   collides with every heading written before it and was left unruled.
   The session's last thought is its biggest: most players will not read
   the Guide first and will not read it long, coming to it mid-game
   wanting one specific thing, so the first part would explain the steps
   quickly with links down to the full explanations — which reaches back
   over every section already written. Nothing was decided. Links were
   checked and are possible by the page's own tap-and-scroll road rather
   than an `href`, untested on the phone.
   Y-34 (2026-08-14) settled the Guide's shape and wrote Setup's short
   pass, touching no app code. Patrick opened by saying that what was
   being built had become the chore he set out not to write, and named
   what he wants instead: a warm document that walks a new player
   through quickly, and that lets them find one specific thing fast
   when they need it. That is two jobs, and it closes the Y-33
   question in the affirmative — the Guide has a short walkthrough on
   top, carrying the same opening and the same order of things in far
   less space, pointing down to the long sections already written, most
   of which become that lower layer unchanged. Setup's short pass is
   written and agreed: five numbered steps holding the order of work
   and the must-haves, ending at ▶ Play, and deliberately not listing
   the seven conditions behind it. Its first draft was right in size
   and shape and wrong in tone — Patrick said it read like a checklist
   — so it was rewritten warmer at the same length. Checking it against
   the long Setup section produced five corrections: the step labels
   were changed to the headings they point down to, so a reader lands
   on a name they recognise; step two now names the Save inside the
   Edit pop-up, which a player could otherwise rename past and lose;
   step four names Done, which is what settles the counts; step one
   puts "This is Me" before Confirm; and the long introduction lost the
   opening sentence the short pass had taken over. Its next line was
   reframed as well, on Patrick's point that saving is about keeping up
   to four decks and loading one back rather than about never doing the
   work again. The Edit pop-up's Close was read from the page and is
   now named in the Cards part — a plain word in the title bar, doing
   exactly what Cancel does. One piece of future app work came out of
   it and sits at item 5 of `docs/pending.rtf`: both of those buttons
   throw the whole edit away on a single tap, which Patrick confirmed
   on the phone, and they should take two — but only when something has
   been typed, and only in that pop-up, the others costing seconds to
   redo where this one can cost the ten minutes. The general rule
   behind it was talked through and is the settled one: confirm what
   cannot be undone, never confirm a constructive action, and prefer
   undo to a confirmation where undo exists.
   Y-35 (2026-08-14) gave the Guide a reading copy, finished the
   walkthrough, and reversed the shape of the long layer. No app code was
   touched. Patrick asked for somewhere to read what was being written, so
   a script now lifts the Guide's words out of the working file and builds
   a Word document from them, generated and never hand-edited, which cannot
   drift from its source. Word itself would not open or save on his Mac and
   he gave up on it; the drafts were read in the chat instead. He read the
   walkthrough whole for the first time and changed six things across the
   opening, the theme note and the short Setup pass — the theme note is now
   one line, its second paragraph and the glyph fact in it cut on purpose —
   and the short game pass was drafted and agreed with one change of his,
   which also closed the Y-34 question about step three. The durable ruling
   is the reversal: the long layer is no longer to be cut, because it is
   where a reader arrives looking for one particular thing. Things are
   broken apart rather than tied together, each gets a heading so it can be
   found, and each is explained fully — running long is not the fault, a
   reader finding their part and still not being told what they needed is.
   It does not have to read as one flow, and he meant the whole Guide
   rather than one section. Playing a turn was rewritten whole under it and
   is not agreed; its second half has never been in front of him. Three
   smaller things settled: US spelling throughout the Guide, section
   boundaries that must read clearly on the phone by styling or indents,
   and the "Where are the cards?" button filling green once Done is tapped,
   which the Guide had never mentioned and now does. Found and not acted
   on: the Game screen section was written under the old shape and packs
   several things under one heading, and both bars are now described in two
   places.
   Y-36 (2026-08-15) finished Playing a turn — the first Guide section
   agreed entire since Y-32 — and settled the form the long layer takes,
   touching no app code. Under each sub-heading the paragraphs now stand
   as bulleted items, with a bridge sentence above the list and a closing
   sentence below where each is wanted. Patrick's reason is the durable
   part and outranks any rule of thumb about length: his mind sees the
   forest and immediately knows how to work its way through the woods,
   so the shape tells a reader how to walk through a piece before they
   have read a word of it. What forced it was the opposite experience —
   the headings were vanishing into the prose, and he read two
   sub-sections as one without ever seeing the second heading. A heading
   followed by a bare paragraph is therefore what to avoid even when the
   paragraph is short. The section was read one piece at a time, the
   second half first and then the first half brought into the same form.
   One claim was cut after his eye caught it and the engine bore him out:
   the bullet saying no ! is written for a card already confirmed as
   someone's was a repeat, because a confirmed card already puts a ✗ in
   every other box and the engine refuses a ! there — which overturns one
   of the three things Y-35 had let in under the explain-fully rule and
   vindicates the Y-33 judgment that the player cannot see the
   difference. That read is recorded so no session re-argues it, and it
   turned up one thing about the app that nothing is proposed about: the
   guard in `markShower` looks as though it can never bite. Shorthand
   became a Guide rule as well as a chat rule, three phrases that told
   Patrick nothing being written out in full. Settled for a later session
   and belonging to the app rather than the Guide: the two Me pop-up
   headers go into the past tense, reaching the page, the message map,
   the Guide text that quotes them and the wrapper copy, which then owes
   the phone a test. Two new open items were named at the close — Setup
   and the Game screen want the same form, which Patrick asked to be its
   own session, and the short walkthrough is still not linked down to the
   sections it points at. The stale note telling the next session to come
   to Playing a turn with cutting in mind was closed, the Y-35 reversal
   having overtaken it. And `docs-ref/build-history.md` was found to end
   at Y-33, neither Y-34 nor Y-35 having a section of their own; both were
   written this session from the records made at the time, alongside
   Y-36's.
   Y-37 (2026-08-15) finished Setup in the new form and touched no app
   code. It is the first section reshaped backwards under the Y-36
   ruling, all six parts carrying their colon, their bridge sentence
   and their bullets, and a seventh part added: Patrick said categories
   wanted a sub-section of their own, so the single Cards part became
   Cards, Categories and Rename → Edit, with deleting a category
   described once instead of twice and two facts the Guide had never
   carried — a thirty-card deck ceiling and card names unique across
   the deck — read from the engine and taken in. Three rulings of his
   came out of it. Every sub-heading ends with a colon, closing a
   question open since Y-33, and his reason is the durable part: a
   short line followed by a colon tells him it is about to be explained
   below. The capitalized section names take none, and "Where are the
   cards?:" takes one after its question mark, two marks of punctuation
   being the accepted price of a promise a question mark cannot make.
   No specific color is named any more, which narrows his own Y-31
   ruling, with three standing exceptions where the color is the app's
   only signal that a tap took — the card chip, the counts button after
   Done, and the count of your own cards. And the Guide never assumes
   when the game is played, so "tonight" and "the evening" both left
   agreed text. A Game page layout note was written and agreed for the
   top of the walkthrough's game pass, introducing New, Out, ⭐ Accuse,
   the theme button, ↩ Undo and Next ▶ — his instruction being that the
   reader should meet the page before the turns begin, and his first
   correction being that it is the Game page and nothing else, ▶ Play
   and Setup struck from the draft. The session's largest outcome is
   open rather than closed: **all the pop-ups need explaining**. It
   began with New, whose Y-32 exemption the note reverses, and Patrick
   widened it to every pop-up in the app; where that explaining lives
   was asked and not answered, and thirteen windows are in scope. One
   thing worth carrying: when the Y-35 reversal was applied backwards
   only its form came with it, and nothing swept the earlier sections
   for what they had left out under the older standard — New is the
   first item found in that gap and probably not the last. Left owed:
   the Game screen's own reshaping, the ruling on two bars described in
   two places, a verification pass over the reshaped Setup, and
   "memorise" sitting twice in agreed text against the Y-35
   US-spelling ruling.
   Y-38 (2026-08-15) produced nothing and left no record anywhere, so
   no docs refresh happened and Y-37 remained the true state. What
   went wrong in it is recorded at Y-39 because it is durable: a
   placement instruction of Patrick's — say what is needed here, the
   detail goes elsewhere — was converted into a ruling that Next ▶
   need not appear in the Guide at all, and once that invented ruling
   was in, every later answer was given against it. The rules were
   then pared back on the suggestion that they were the obstacle, and
   with fewer of them in the way the very things they guard against
   happened; Patrick restored them all and ended the session. Y-39
   settled what that says about model settings: a missed connection
   does improve with more effort, while an invented ruling does not
   and can get worse, a stronger model defending a wrong premise more
   fluently.
   Y-39 (2026-08-16) wrote the Guide's structure down for the first
   time and built the first section under it, touching no app code.
   The structure had been changed when Patrick abandoned the old
   app's shape and explained at the time, but never recorded — so the
   file still carried the Y-34 two-layer plan while the work was
   being done to a three-part one, and he raised it himself on
   noticing that "Details section" was a phrase with no home in the
   notes. It now heads `docs/guide-rebuild.md`: an introduction; a
   walkthrough of Setup then the Game page, enough to get started
   without reading the whole Guide; and the details, following that
   same flow in full and finishing with a section for each individual
   modal, button and feature. Those come last because a player with
   the basics leaves, which is the point, and returns later with one
   specific question — the two flows answer most of those and the
   trailing run catches the rest. Features is a catchall for whatever
   is neither a modal nor a button. That closes the Y-37 question of
   where the pop-ups get explained, and the Y-34 two-layer note is
   marked superseded rather than deleted. Two rulings came with it,
   both reaching every section: the whole story of each modal lives
   in the details part while other places may still mention it
   briefly, with one last pass over the finished Guide deciding what
   those brief mentions keep — and a placement instruction is never
   permission to leave a thing out; and a section is organized around
   its own subject, in Patrick's words, "the aim is to imagine how
   the user will expect, need, or want it." The Next ▶ section was
   then drafted and agreed entire, the first built under the new
   structure. It had never been unwritten, only un-gathered — all
   four of its behaviors already sat scattered across four
   sub-sections of Playing a turn, which stay put until the last
   pass. Next ▶ opens no pop-up at all, established before a word was
   drafted, and the read behind the section is recorded so no session
   repeats it. Rule 8 was narrowed for reads on Patrick's word: an
   essential read that is not humungous is simply done rather than
   asked about.
   Y-40 (2026-08-16) gave the trailing run its names and its order,
   built Seat to agreed, and drafted two more sections, touching no
   app code. The durable ruling is how a section is named: a button
   or a pop-up is named by the name the reader will be looking for
   rather than by what it does — Patrick's own sentence, rejecting a
   working list that had described each of the thirteen windows by
   its function. He then named all fifteen sections himself and set
   their order, which follows the Guide's own earlier parts, each
   thing placed where it first matters as the Setup flow and then
   the Game flow run. Three changes of his shaped it: ▶ Play had
   been missed altogether and is a button, so it closes the Setup
   group; New moved to the foot of the Game group, a player needing
   it only once a game has ended; and Feedback groups with ← Setup
   and Game →, which the page bore out, the Guide's footer carrying
   all three with Feedback between the two. Two of his names landed
   on each other's rows and the untangling produced its own ruling —
   💾 Save Card Deck is the name of both the Setup button and the
   pop-up it opens, so one section covers both, and the window
   reached by tapping a saved deck's chip is called the saved deck
   chip rather than Saved Deck, that being the name the Guide has
   already taught. Patrick then raised, unsure, that Close might be
   explained once rather than in every section; the read bore him
   out, all thirteen carrying a Close in the title bar and ten a
   Cancel, every one of them calling the same one-line `closeModal`
   that only hides the window, so both are explained once at the
   head of the modals. A caveat Claude raised about the ∑ picker was
   invited back for a rethink rather than corrected outright, and
   withdrawn — and Patrick then corrected the rethink as well, the
   picker closing the moment a pick is made, with ⭐ Solution? the
   one exception. Names in the Guide's text are now italicized,
   buttons above all, because without it the sentence reads wrong to
   him; that reaches backwards over Seat and Next ▶ and the pass has
   not been made. Seat was pared in three passes and agreed entire,
   what came out mattering as much as what stayed. ＋ Add Category
   and Rename – Edit are drafted and not agreed, the second having
   gone from seven sub-headings to four on his reaction that just by
   looking at it the reader is scared off, and the first having been
   broken out of it because adding a category is something the Setup
   page does rather than that pop-up. Where deleting a category is
   told was settled and reverses Y-37: the whole story goes in
   Rename – Edit, the Categories bullet standing as a brief mention
   until the one last pass. Two things about how the work is done
   came out as well — a bare session label like "the Y-37 ruling"
   tells Patrick nothing and the ruling must be named in plain
   words, and narrowing the ask-before-acting rule for reads cost
   him his view of the load, so the size of a read is named before
   it is done. Both of them thinned late in the session and Patrick
   called it first, saying he should have called it over when he
   first noticed.
   Y-41 (2026-08-17) settled how the work is done from here and built
   one section under it, touching no app code. The largest outcome is
   Patrick's ruling that the modals contain everything, no matter what
   is said elsewhere — which sharpens Y-39 rather than replacing it: a
   modal's section is complete in itself, and the question of whether
   a thing is already said somewhere else has no say at all in what
   goes into it. His image is the durable part, that even though it is
   the trailing section it is like a foundation, the walkthrough and
   the two flows standing on it as summaries; what happens when a
   summary and a modal disagree was not raised. Its one recorded
   consequence is that the one last pass now only ever looks at the
   other places and never at a modal. Alongside it came a way of
   working that carried one subject across three layers at once,
   since replaced at Y-43 — how the work is done now is stated in the
   project's `docs/guide-rebuild.md` and is not restated here. A
   first draft is now drafted trimmed rather than pared afterwards,
   to his own limit of trimmed without being short-changed. He
   tested the method on 💾 Save
   Card Deck, which is agreed entire — the fourth of the fifteen
   trailing sections and the second to reach agreed — and he changed
   one word in the whole of it, "opens a pop-up" becoming "opens as a
   pop-up". Two facts went in that the Guide had never carried: the
   three refusals, and that a saved deck is a copy frozen at the
   moment of saving with no update door at all. Four observations were
   recorded for the one last pass. The session ended on a miss worth
   keeping: opening the next bite, Claude sorted the facts by whether
   the Guide already said them and proposed a section shaped around
   the gaps, which is the very question the ruling had abolished
   hours earlier — Patrick named it and closed the session. Also
   settled: the italics pass waits, and when it comes it is one pass
   over the whole Guide rather than a section at a time. Three things
   he set aside unruled: the read-backs of ＋ Add Category and
   Rename – Edit, and the Close and Cancel note.
   Y-42 (2026-08-17) built the saved deck chip section and agreed it
   entire — the third of the fifteen trailing sections to reach
   agreed — and touched no app code. Patrick narrowed the bite at the
   top of the session to the complete modal and nothing else, so
   neither the walkthrough nor either flow was opened; that was an
   instruction for one piece of work rather than a new standing rule
   at the time; at Y-43 it became the standing method. The section runs
   four sub-headings, with the two-tap mechanic given one of its own
   rather than told twice under Load and again under Delete, and it
   answers the Y-41 note asking it to collect the two Setup bullets
   that describe the Saved Deck window. The drafting was shown to be
   right by a check worth carrying: a section built from the modal's
   own subject must repeat things the summaries above it already say,
   so overlap is the sign of health and a section with no overlap is
   the tell — four of this one's facts are told elsewhere and stayed
   in. Patrick rewrote Loading a deck over four passes, his verdict
   being that it did too much repeating, and the settled bridge
   sentence is his; three word choices inside it are his as well, and
   four single-word completions were Claude's, marked as such before
   he agreed them. One fact went in that the Guide had never carried
   anywhere: a category left empty when a deck was saved does not come
   back when it is loaded, and if that would leave none at all the app
   substitutes its own starting categories. The session also struck a
   sentence from rule 22, recorded below. Its last outcome is a
   record rather than a build: a session between Y-41 and this one was
   deleted and left nothing, having failed the same way Y-41 failed at
   its close — the Y-41 text establishing the modals ruling was pasted
   in, acknowledged, and then the same error made again and not seen
   even after Patrick pointed the fact out. Stating a rule and
   building under it are separate acts, and being able to state it
   correctly is worth nothing as evidence. This session had its own
   early miss too, before anything was thin: a pronoun slip in one of
   Patrick's sentences was read one way, treated as fact, and three
   paragraphs built on it before he stopped it.
   Y-43 (2026-08-17) replaced the three-layer method and began writing
   the rules as one current form, touching no app code and never
   beginning Rename – Edit, which its opener had named. The session
   opened with Claude asserting the Y-41 three-layer method as
   standing; Patrick said flatly that it is not a current ruling, and
   the files bore Claude out only in the sense that they were the
   thing that was wrong — this project's hand-off carried it as live
   and this file said in two places that Y-42 had not overturned it.
   What stands now is one modal at a time: the modal is the unit, a
   modal's section carries everything about it no matter what any
   other section says, the walkthrough waits until everything else is
   written, and the two flow sections are left as they are. **How the
   work is done is stated in the project's `docs/guide-rebuild.md` and
   in no other file**, both hand-offs pointing at it rather than
   restating it, which is the whole point of the change. Patrick's
   complaint is the durable part — he spends the beginning of every
   session correcting how the rule is made — and he named the
   compounding cost himself, that these conversations are as thinning
   as reads, which is Y-42's own finding turned back on us. The
   diagnosis settled on is the form rather than the count: rulings are
   recorded as a chronological stack, each dated note sitting on the
   last, so a session has to work out what stands and the working-out
   is where it fails. His own statement of the fix is the one to
   carry: keep the rule, but the correct one only, with the superseded
   wordings living on in the build history. It is expressly not Y-38,
   which removed whole rules and failed; this removes only their older
   drafts. Asked whether each entry should say if it is a rule or a
   guide, he declined to decide and gave his preference instead —
   the files are Claude's to construct as they best serve it, and if
   it were up to him they would all be guides applied with common
   sense — so no labels were added, but his name stays on the entries
   that record his decisions rather than craft. He then stopped the
   wholesale rewrite, worried about a mass changing and asking for one
   or two entries targeted at the most benefit, so exactly one was
   rewritten: the entry that had broken the session. He will not read
   it and will judge it by how well the next session works. Two
   findings came out of the read that nothing was done about: a
   heading in the working file claims live agreed Guide text is
   superseded, and five judgment calls written down for him have no
   answer recorded anywhere. And Claude leapt twice the same way,
   asserting the method off a stale file and then turning a "yes"
   about wording into a scheduled project — the same fault Y-42
   recorded, filling a gap with an assumption instead of asking.
   Y-44 (2026-08-17) built the Edit section and agreed it entire — the
   fourth of the fifteen trailing sections to reach agreed — and touched
   no app code, though it produced a one-line change to the app that is
   owed. Patrick opened the work by renaming the button: it should read
   *Edit* only. The page still says *Rename → Edit*, checked that day,
   so his sentence was a decision about the app rather than a correction
   of the record, and the section took the new name with it under his
   own Y-40 rule that a thing is named by the name the reader will be
   looking for. The button and the pop-up then carry one name between
   them, the shape 💾 Save Card Deck already had. The app change was
   deliberately kept out of the drafting bite because it is code and
   belongs with the commit rhythm — `mystery-phone.html` line 1388, then
   the wrapper copy and a phone test — so the Guide is ahead of the page
   until it is made, and the rename also reaches three places left
   untouched: Setup's agreed sub-heading, its two Categories bullets,
   and the last bullet of the ＋ Add Category draft. The session's one
   new fact about the app is Patrick's own find, raised before any
   drafting began and verified rather than taken on memory: a Save with
   nothing typed in clears the card counts, because `editCategory` calls
   `clearCounts()` unconditionally and the page falls back to each box's
   placeholder, so an untouched pop-up hands the engine a full set of
   rows that look like edits. The entered flag goes back to false — one
   of the seven things ▶ Play waits on — and the "Where are the cards?"
   button loses its green with it. It is the one fact in the section the
   Guide had never carried anywhere, and it closes the Y-40 note that
   had pushed clearCounts out to the counts section, a judgment made a
   session before the ruling that a modal's section carries everything
   about it. One ruling of his governs the section's language: the hand
   is not spoken of in it, his words being that the deck and your hand
   are the same but this is about editing the deck — checked in the
   engine before it was applied, and nothing is lost, the hand following
   the deck in all three operations there. The section runs four
   sub-headings in the order he set at Y-40, he made four wording
   changes, and three judgment calls were named to him before he agreed
   it and all three let stand. The session's other outcome is a record
   rather than a build. Patrick said two-thirds of the way through that
   nothing had been accomplished yet, and he was right: the heavy read
   was over early and what consumed the session was questions. One was
   asked about sequencing while a substantive one stood unanswered three
   turns back, and one finding was reported as new when Claude had
   quoted it from the Y-31 record himself before going to look. Blank
   bullets in his edit list were also read as deletions when they were
   spacing. What worked was naming judgment calls before he reacted and
   verifying his counts claim in the code rather than agreeing with it.
   Next, in order: Where are the cards?, next in the run's own order;
   the one-line button rename in the app, with its wrapper copy and
   phone test; the rest of the trailing run; the read-back of ＋ Add
   Category and the Close and Cancel note, both set aside unruled;
   whether the rules rewrite is carried past its one sample entry; the
   live material stranded under a superseded heading; the italics pass
   over the whole Guide; the Game screen brought into the new form; the
   rest of the Guide; and the new test spec, several sessions of its
   own.
   Y-45 (2026-08-17) replaced the Y-40 draft of ＋ Add Category whole
   and agreed it entire, touching no app code. It is the fifth of the
   fifteen trailing sections to reach agreed and it completes the
   first five of the Setup group in the group's own order, so only
   Where are the cards? and ▶ Play now stand between the Guide and a
   finished Setup group. The session began by asking rather than
   guessing: Patrick's opener named "＋ Add Card", which is not one of
   the fifteen, and the page carries both that button and ＋ Add
   Category as different things. His goal for the section is the
   player's side rather than the app's — to be able to use the app for
   a game that requires four categories, and to delete one so as to
   play a two-category game — and although the goal names deleting,
   he kept deleting out of the section entirely, the whole story
   staying in Edit where Y-40 put it, along with the one deleting fact
   that belongs to this button, that deleting brings ＋ Add Category
   back. The collision between his goal and that agreed text was
   flagged and put to him rather than resolved quietly. The durable
   part of the session is four facts Claude reported and Patrick
   corrected, every one wrong the same way: a true line of code read
   and reported as though it were what the player meets. The counts is
   the one to carry. `clearCounts` really does zero the numbers, and
   that is where the reading stopped, but `openCounts` then finds no
   numbers carried and fills the boxes from the app's own suggestion,
   which is worked out from the deck and the seats, neither of which
   an empty new category changes — so the player never sees a zero,
   and one who took the suggestion sees the same numbers come back.
   His correction was exact: the set condition is cleared, not the
   count. The other three were the mid-game refusal, which cannot be
   reached from the page and so earns no place in the Guide; "the only
   thing that happens", which was untrue and whose missing half he
   supplied himself; and his own word "pop-up", which was queried
   rather than accepted or contradicted and produced "Good point, it
   is a button". He also asked directly whether there is useless code
   in the app, and the answer is his own Y-29 ruling — the
   `setupClosed()` guard in `addCategory` cannot fire from the phone
   page, but a guard stays when the only reason it cannot fire belongs
   to the page, because the engine never relies on a packaging to
   protect it, and nothing is proposed about it. One thing is now
   owed: a short caution in the Guide's Where are the cards? section,
   and expressly not in the app, saying that Setup changes made after
   the counts are settled un-set them and that a player who set the
   numbers by hand loses them. Next, in order: Where are the cards?,
   which carries that caution; ▶ Play, which finishes the Setup group;
   the one-line button rename in the app at `mystery-phone.html` line
   1388, with its wrapper copy and phone test; the rest of the
   trailing run; the Close and Cancel note, still set aside unruled;
   whether the rules rewrite is carried past its one sample entry; the
   live material stranded under a superseded heading; the italics pass
   over the whole Guide; the Game screen brought into the new form;
   the rest of the Guide; and the new test spec, several sessions of
   its own.
   Y-46 (2026-08-17) did the whole-code read behind Where are the
   cards? and drafted nothing, touching no app code. Patrick ruled
   the read must be both files end to end because the counts feed
   decisions throughout the game — 3,990 lines, the heaviest read
   the project has had — and its account now stands in
   `docs/guide-rebuild.md` in the run's own order, directly after
   the saved deck chip with ▶ Play to land behind it, so no session
   reads that code again. The governing ruling came after the read:
   the counts are not for the players, who already know who has how
   many cards — the count is for the app, which cannot see the deal;
   what the player gets back is the app's only cross-check on the
   tapped hand that founds the whole sheet at turn zero. The read's
   one real surprise: stepping House refills every player row, so
   the window expects House first, players after. Also recorded: the
   counts never show on the Game screen and cannot be looked up
   mid-game; any real seat change clears them, a rename included;
   New Game with both choices Same carries the numbers but never the
   settled flag; and the 🏠 marks do not have to match the House
   count, stated plainly with Patrick's reason — you mark only the
   board cards you see yourself, since other players' peeks are
   their own. Patrick switched the model to Fable 5 for the read
   after the mid-session switch was checked in Anthropic's
   documentation — the conversation carries across whole, and it
   did. The section itself is next, drafted from the account, and
   the caution Y-45 placed in it now has its full material gathered
   there.
   Y-47 (2026-08-18) drafted Where are the cards? and agreed it
   entire — the sixth of the fifteen trailing sections and the sixth
   of the Setup group in its own order, built from the Y-46 account
   without opening any code, so only ▶ Play now stands between the
   Guide and a finished Setup group. The Y-45 caution is delivered
   inside it. The session's first sentence was false and Patrick
   caught it: it said the two rules files had not arrived on their own
   and had been read by hand, when both had arrived on their own and
   were in front of Claude from the first moment. He said he had been
   suspect from that sentence onward and the first draft then
   confirmed the doubt — his verdict on it being that it was too
   mechanical and carried too much irrelevant material, an hour or
   more of editing, and it ran roughly twice the size of the agreed
   section sitting next to it in the run. The irrelevant part was the
   app's machinery, turn-zero marks and the sheet's reasoning, where
   what he wanted was the plain thing: the app knows the players
   already know who holds how many cards, and it is the app that needs
   the count, to catch mis-taps on the small phone screen and other
   mistakes costly to correct later. That was already in the Y-46
   account almost word for word and had been read and converted into
   machinery, which is Y-42's finding again — having the right material
   is not the same as recognising which of it is the point. He nearly
   closed the session and tried it instead, and he raised the model as
   well, having left it at Fable 5 on maximum effort from the Y-46
   read; he switched to Opus on extra mid-session and the conversation
   carried across whole for the second confirmed time, and what was
   established is that a draft's standard is the register of the agreed
   sections themselves rather than any model's voice. Two rulings of
   his outlive the session. The 🏠 mismatch goes to the House column
   section rather than this one, because that is where the question
   comes up — the Y-41 modals-contain-everything ruling was raised with
   him rather than worked around, and the answer is that the mismatch
   is the column's subject, so this is a determination and not an
   exception; his own Y-46 wording is recorded verbatim as owed to that
   unwritten section, and Where are the cards? carries a stated fact
   and a pointer only. And bold is a label, never emphasis: it stands
   at the head of a bullet and never inside a sentence, used only where
   a bullet carries a subject a returning reader hunts for. That one
   came out of a length problem he refused to solve by cutting — the
   section is very good as it is, he wants nothing removed, and a trim
   would cost more than it saved, so the answer to length is
   findability. It reaches the whole Guide and is one pass, likely the
   same trip as the italics pass, and the check behind it is that bold
   in the agreed sections is structural only, so mid-sentence bold
   would be the first that does not mean "here is a heading". Two
   smaller things settled: sub-sub-bullets splitting what does and does
   not clear the counts, which he called excellent and which any
   dividing list may now use, and judgment calls belonging at the top
   of a message rather than the foot, because he reads top to bottom.
   The committed Store version stays shelved
   byte-identical at `Projects/locked-mcts.html`. The Android
   legs wait until the merged app is done, and `wrapper-android`
   has never been given the rebuilt page.
3. **A Place To Remember (Memory) — iPhone** — Alpha.
   Folder: `Projects/elderlyassistant`. Status: #4-new
   (2026-08-18) fixed the three notification defects and is
   written but unbuilt — six files changed, TypeScript clean,
   nothing on the phone. Patrick redirected the session to them
   because he now uses Memory daily and the notifications are his
   biggest gripe, and because a new app he wants will lean on
   reminders heavily. The three defects came from a read-only
   review made in a web session, saved at
   `docs/ElderlyAssistant-notification-findings.md`; all three
   were verified against the code before anything was changed,
   and two of the document's claims were corrected. My Day's and
   Pets' banner Done no longer destroys the daily repeat and now
   sweeps up the item's pending snoozes, and all five routine
   screens — My Day, Pets, My Week, Look Ahead and Orders — now
   re-read storage when they regain focus and when the app
   returns to the front, so a banner's check-off is visible
   instead of being overwritten. The standing Look Ahead
   banner-delay bug was probably cured with it. What is owed is a
   build and a week of Patrick living with it; the three
   "What's Next" items in pending.txt are untouched. The other
   thing that session produced is a feature draft for a college
   student's assistant, which would live on the web first. It and
   a copy of the chat behind it now sit in a folder of their own
   at `Projects/Sudents-Assistant` — `college-app-draft-v1.md`
   and `Campus travel.rtf`. That folder name went in misspelled;
   Patrick renames it to `Students-Assistant` next session. The
   new app got its own session and its own chain at SA-1
   (2026-08-19); see project 4 below.
4. **Students-Assistant — iPhone** — paper only, no code.
   Folder: `Projects/Students-Assistant`; its CLAUDE.md names the
   reads, and the layout follows `MysteryCluesTracker` — `docs`
   active, `docs-ref` reference. Status: SA-4 (2026-08-19) settled
   what an individual item is and what a reminder is for, and took
   Memory's whole look across. **An item is the class with all its
   information under it** — its full name, the times it meets, its
   place or places, its books and syllabus, its due dates, an
   estimate of size and time for a whole thing, and the pieces it
   breaks into with their own sizes and times. Five courses means
   five items rather than fifty, there are three levels with
   sub-items under assignments, and the item is not a schedule but
   feeds the Day and Week schedules and the travel warnings. The
   session's harder half was the reminders, and Patrick sharpened it
   himself by asking what a reminder is for: **they are a call to
   action**, which gives the test that at the moment one speaks she
   must be able to act on it. The six kinds of reminding the record
   had committed to were listed in one place for the first time, and
   two things fell out of the list — only the due-date warning is a
   setting she makes, the other four being worked out from what the
   item already holds, and **Done is a call for inaction, to relax**,
   which was Patrick's correction of Claude's claim that it stood
   outside the family. That folds the spine into one mechanism with
   two directions; he called the reading a start rather than the
   answer. He then corrected a proposal that would have hidden the
   reminder option: **it is never demanded, but always presented**,
   and entering asks nothing of her at all — she taps Done and fills
   in later, the setting sitting at the top and falling downward with
   a default underneath that makes her silence safe. To-Do's reminder
   row is the model for how it looks, minus its ask on Save; which
   lead times belong on it is not settled. Last, he asked for
   something more general and took Memory's palette, styling and
   buttons whole, fitting this app into that format. A three-search
   look-up found the palette lifts cleanly as one file,
   `constants/Themes.ts`, 337 lines, about sixty keys named by
   meaning rather than by color, two themes, and the hook sixteen
   screens read. Memory has no shared button component; Patrick
   ruled that here a button doing the same job on two pages is one
   shared piece. Before it, SA-3 (2026-08-19) read the
   university's campus map and closed the app off from outside data,
   which is the largest structural decision the project has made.
   The app is self-contained — no syllabus import, no course system,
   no bus feed, no automated travel — and everything in it is
   entered by her. Patrick had hoped the syllabus could come off the
   school's website and put that down himself rather than take on
   importing and handshakes; his reason is the benefits of staying
   self-contained. Three standing items fall away with it: the
   StarTran legal question that has blocked since SA-1 no longer
   blocks anything, the Canvas five-system merge cannot break what
   the app does not use, and how the syllabus gets in is answered.
   The leave-by alert survives, running on the travel time she
   entered rather than on where a bus is. The session also gave the
   app its first self-firing behavior, the squeeze warning: whenever
   a squeeze occurs the app warns her, as she enters and on Save,
   checked against everything already in, however many there are,
   and not only at the start of a semester — and it is useful from
   the second item on, since one item cannot conflict with anything,
   so there is no complete setup to get through before the app pays
   off. Patrick's own campus map PDF, dropped into `docs-ref`
   mid-session, resolved all six building codes in her schedule and
   showed that three of her five days cross between City and East
   Campus, with the ten-minute Tuesday and Thursday gap running East
   to City — which the map's own directions make a ride rather than
   a walk. That collided with SA-2's ruling that the campus split
   does not matter yet; put to Patrick rather than worked around, he
   narrowed it himself: it is guidance and not a wall, and it was
   for the travel effort, where this is scheduling. Two smaller
   things settled: a task is entered by the size of its bite, some
   fixed and some variable with reading cut to whatever the gap is;
   and the first sitting is the beginning of a semester, its
   contents recorded, with his own word on the list being "for
   starters." The next subject is his: the structure of an item as a
   whole and as pieces, opened and not started. He also asked
   whether Fable 5 would suit this work better and had to ask twice,
   the first answer being the record instead of an answer; the
   answer is no while there is no heavy read in front of us.
   Before it, SA-2 (2026-08-19) checked
   the name against the app stores and settled the app's shape; the
   working file for that is `docs/app-structure.md` and it is the
   one to open when the structure question comes up again. The name
   survives the check — nothing exists on the Apple App Store or
   Google Play under "Students Assistant" or "Students-Assistant",
   though the singular shelf is crowded with planners and trackers,
   and Student-Aid is worse ground, that phrase belonging to
   federal financial aid. Patrick's own verdict closed it: none of
   those apps have the reminder features he wants, which is why he
   built his own.
   The session's real work was the shape. Its turn was his sentence
   that there are bus route and time sites, organizers and
   calendars, and not one reference among them to helping remember
   to get it done, go to class, catch the bus — a live bus map
   being useless at the moment that matters, because that moment is
   a few minutes earlier when she should have left. He added the
   half nobody builds because it looks like nothing: the app does
   not only remind, it reassures that a thing has been done. So the
   spine is remind before, reassure after, and Memory already does
   the second half three ways, My Week's self-clearing tick being
   the purest. The focus is knowing where to focus now, other
   features may or may not come later. The ordering came out of his
   cooking analogy, read back and confirmed: she sequences by what
   must happen before what rather than by what is due soonest, she
   works the dead time while something else runs itself, and the
   comfort is in being able to put everything else down — with his
   one correction, that she still needs the due dates, so the date
   is what the app reasons with rather than what she reads. He
   added expected work and time as a required ingredient, which is
   what makes the rest computable. The first concrete rule is the
   gap rule: given a gap, offer what fits inside it, soonest due
   first — not the most urgent thing overall but the most urgent
   thing she can actually clear. And he corrected a sentence Claude
   had written saying she wants one answer: she does not, the app
   offers several annotated options and she chooses, never deciding
   for her, with a separate running-out-of-time warning that a due
   date alone can never produce.
   Two other things settled. A thing Patrick sets aside as "adjust
   later" is written down as settled rather than carried as open —
   he does not want to be reminded that something he has already
   put down is still open — and that is now a working note in the
   project's `CLAUDE.md`. And travel drops down the list: he is
   less concerned about it than she was and says the live feeds
   cover the Omaha campus, though SA-1's record covers Lincoln only
   and says nothing about Omaha. The leave-by alert is not
   abandoned; it is the spine applied to a bus.
   Two new working files: `docs/app-structure.md` and
   `docs/student-needs-research.md`, the second holding published
   survey findings with every one graded strong, fair or weak,
   because the wayfinding material and every criticism of Canvas
   turned out to be published by companies selling the remedy. Its
   strongest finding is that the most-wanted tool students name is
   the one Patrick has already built — more than two in five chose
   combining different syllabi into one set of deadlines, the top
   answer of eight.
   Her class schedule arrived as a screenshot at the end of the
   session and is written into `docs/app-structure.md`. Five
   courses, Monday to Friday with Tuesday and Thursday identical,
   the day headings never actually seen. It settles that a course
   is not one weekly item, that a place belongs to a meeting rather
   than to a course, and that My Week's one-weekday-per-item limit
   is a real obstacle rather than a theoretical one.
   Before it, SA-1 (2026-08-19) opened the project and its chain.
   The folder rename from the
   misspelled `Sudents-Assistant` was already done. Patrick
   settled five things: the build platform is a native iPhone app
   using Expo like Memory, which overturns the "web first" line
   the Memory hand-off had carried and rests on the draft's F-5,
   that only a native build can schedule its own local alarms; the
   chain is "SA-##"; the file layout follows
   `MysteryCluesTracker` with a Rich Text pending list; the app
   reaches the public from elyfont.com as Memory does, with what
   that means in practice not worked out; and the name is
   Students-Assistant, a short badge name left for later. The
   folder's documents were all built this session —
   `CLAUDE.md`, `docs/handoff.md`, `docs/pending.rtf`,
   `docs-ref/build-history.md` and a stub `docs-ref/ROADMAP.md` —
   beside the two files it arrived with,
   `college-app-draft-v1.md` and `Campus travel.rtf`.
   The session's real finding is that F-2's dependency is
   verified and open. StarTran's timetable and its live bus
   positions are both public and need no key, the addresses are
   recorded in the project's build history, and the crossing
   between UNL's campuses runs on ordinary StarTran routes that
   sit inside those same feeds — Route 24 Holdrege joins the
   Nebraska Union to seven named East Campus stops. Route 23 is
   UNL's own van and is outside them.
   One question is live and blocks building on that data: a
   StarTran staff member told Patrick by telephone that federal
   law forbids using their data in an app because StarTran is
   federally funded, and did not know the details. Everything in
   the public record runs the other way — GTFS reporting to the
   National Transit Database is now mandatory for federally
   funded fixed-route agencies, those feeds enter the public
   domain, and the FTA has said riders should be able to rely on
   third-party apps — and no StarTran or Connexionz terms of use
   could be found at all. An email asking StarTran directly is
   drafted and Patrick has the address; it was unsent at the
   close. That question stopped blocking at SA-3, the app now
   taking nothing from outside itself, and whether he still wants
   an answer for some later thing is his.
   `Projects/.gitignore` needs `Students-Assistant/` added to it.
5. **Memory — web** — DROPPED (#72). elyfont.com gets a pointer
   to the App Store listing only.

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
  `Projects/.gitignore` lists all four project folders, each already
  a repository, so the root one tracks only the loose files at its
  own level and never nests.
- **Rule 22 no longer names Patrick's usage percentage (Patrick,
  Y-42).** Its closing sentence — "Patrick reports his usage
  percentage at checkpoints; fold it into stop-or-continue advice" —
  was struck from `Projects/CLAUDE.md`. His usage is a budget meter
  and not a quality one, and it is not the gauge for whether Claude's
  checking is thinning. He was sure the old meter goes, said he is not
  yet sure what replaces it, and asked for no placeholder. The rest of
  rule 22 stands untouched.
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
