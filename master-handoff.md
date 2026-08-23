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
   Folder: `Projects/elderlyassistant`. Status: #13-new (2026-08-21)
   **made a tapped reminder land on its own item, on all five pages that have
   one.** The housing now hands the item's id to the page it opens and the page
   outlines that row. Nothing was added to the scheduler and no test changed:
   every reminder the module makes has always carried the id of the thing it is
   about, and the housing has always read it for the banner buttons — it was
   being dropped at the one place it was needed, so the tap landed on the right
   page and left Patrick to find his own item on it. **The read corrected the
   record twice.** The hand-off had named the Vault as a screen that already
   receives a value that way, and Patrick's first words were that the Vault has
   no reminders — true, and the entry had meant it only as an example of the
   mechanism. The read then found what the account had missed: the highlighted
   row those pages already draw belongs to the reorder selection, and the same
   state raises the ▲▼ arrows, so it could not simply be lent to a reminder.
   Each page got a piece of state of its own instead. **Patrick's rulings, in
   order:** Memory Test gets no highlight, only one reminder coming off that
   page; a lit row is put out by a tap, and when it was put to him that the
   same tap would then select the row for reorder, he gated it so the clearing
   tap does nothing else; and all five were built at once rather than one
   proven first, which was right for the four that share a shape, To-Do being
   held back as its own piece. **The colour work is the durable part.** He
   loaded the four reorder pages, said they all looked good, and asked for the
   light theme's outline to be half as dark. It had been borrowing
   `rowSelectedBorder` — and Shopping uses that same colour on its pale filled
   row, where the darkness is what gives it its distinction. So the outline got
   a name of its own, `rowReminderBorder`, `#6dc6e3` in the light theme with
   the dark theme's orange carried across unchanged; Shopping is untouched. He
   had already ruled the highlight is **outline only, no filled background**,
   and his reason outlives the session: two lit states differing by a thin line
   alone give the eye the hardest difference there is to catch, so reorder
   fills the row and a reminder outlines it. **To-Do took a shape of its own** —
   its cards have no selection and had no whole-card tap at all, so the card was
   made tappable for the single purpose of putting out its own highlight; and
   its background daily is about a group rather than a task, carrying the word
   `background` where an id would be, so that banner opens the background list
   instead of lighting a row. Nothing shifts when a row lights or goes out, done
   two ways because the pages differ. 146 of 146 tests pass and TypeScript
   reports only the stale generated-route error that predates this work.
   **What it has not had is a real banner tap** — To-Do was built after the
   load, and no reminder has yet been tapped to open any page. The morning
   after is still owed as well. **How the session ran:** what worked was putting
   the shared-colour finding to him with the Shopping consequence attached
   rather than changing the value quietly, which produced a separate colour name
   neither side had proposed; what did not was a miscount, five pages reported
   as four after Memory Test was ruled out, quietly dropping To-Do until he
   caught it.
   Before it, #12-new (2026-08-21)
   **built step 8 and finished the scheduler plan — all eight steps are in,
   one module owns every reminder on the phone, and the plan is no longer a
   live document.** Step 8 is the Scheduled Reminders screen,
   `app/reminders.tsx`, reached from a row of that name in Settings under the
   three reminder times. It lists every reminder the phone is holding, broken
   under Today, Tomorrow, This Week and Later, soonest first, with a plain
   sentence at the foot saying how full the phone is; a tap opens a pop-up
   carrying the item's name, its page, when it fires and whether it repeats,
   when it was last due and when it is next due, the exact heading and
   sentence the banner will show, and its buttons. **The screen Patrick
   agreed to is not the screen the plan described** — the plan asked for a
   flat list, and what he wanted was a list he could use to find the reminder
   that was not behaving and then tap for the details, which made it two
   levels rather than one and moved everything technical behind the tap. Asked
   which of the pop-up's six lines he would leave off, he answered none.
   **He asked whether it could show the last time a reminder actually fired,
   and it cannot:** iOS keeps no history an app can read once a banner is
   dismissed, and a record the app kept itself would miss the one case worth
   having, a reminder that fired while the app was closed and went untapped.
   He dropped it once the cost was named. What went in instead is free
   arithmetic — when each reminder was last due and when it is next due —
   which answers his real question by another road: a repeating reminder
   missing from the list is the problem, one sitting there properly armed
   means the app did its part, and a one-off that has gone is simply spent.
   **Timer alerts are counted but never listed, and his reason is the durable
   part:** the Timer is for short stretches, under half an hour, a pot left
   boiling on the stove — it does not go anywhere and does not need looking up
   on a quiet afternoon. **The best practice was looked up rather than
   recalled,** at his asking: Apple ships no such screen, so what was borrowed
   is the grouped-list shape, rows under a heading that gives them context
   with a footer after the last, and the writing guidance for older users —
   plain language, no jargon, no acronyms, 44-point targets — which is what
   ruled out "queue", "pending" and "scheduler" and produced the name
   *Scheduled Reminders*. The arithmetic and every sentence the screen says
   live in a new plain file, `scheduler/queueview.ts`, so Node tests all of
   it: forty-three new tests, 103 to 146. `readQueue` stopped discarding the
   item's name, its id, the banner's heading and sentence and its buttons.
   One judgment call, Claude's: the buttons are asked of the phone rather
   than copied into the screen, so the list cannot drift from what the housing
   registers. **The "Snoozed till:" line was then cured, and it took two
   reversals.** Both pages had styled it with the colour for text sitting ON a
   solid delay button — white on a white row in the light theme, near-black
   brown on a dark brown row in the dark. The first fix went to the delay
   orange, but that runs about 2.2 to 1 against a white row where 4.5 is the
   usual floor; put to him with the numbers rather than decided quietly, he
   asked for plain text and it went to the ordinary text colour. **He then
   reversed it himself and his reason outranks the number** — asked why they
   could not all be like My Week, he said he had looked at all these screens
   in both themes and it works, and that it hits on consistency. So all four
   now read identically: My Day's and Pets' snoozed lines, My Week's postponed
   line, Look Ahead's delayed line. He built it, loaded the phone, and his
   word was that everything came out very readable — the first confirmation of
   the colour work on a device. **One ruling governs the documents
   themselves:** these documents are Claude's and `pending.txt` is Patrick's,
   so a document Claude has no use for should go. `docs/scheduler-plan.md` was
   judged to have none left — its step list spent, its reasoning just as
   reachable folded in — and it is now kept whole as an appendix at the foot
   of `elderlyassistant/docs/build-history.md`. **The same ruling reshaped
   his own file.** The refresh found `pending.docx` missing, rebuilt it, and
   was chasing the wrong thing: that project's `CLAUDE.md` said there is no
   Word copy, and when the contradiction was put to him rather than worked
   around he said the format had never been the point — he wants it readable
   to him, not in a form only Claude finds convenient, and what he actually
   does is convert the txt to rich text by hand every time. So the docx is
   gone, `docs/pending.rtf` stands in its place generated from the txt and
   machine-checked against it, and the split is stated plainly in that
   project's `CLAUDE.md`: the txt is Claude's because plain text can be
   edited without mangling markup, the rtf is his, and the rtf is never
   allowed to lag. One real mistake went with it — the round-trip check was
   run in the docs folder and LibreOffice overwrote `pending.txt` with its
   own output; it was caught at once and recovered exactly from the docx,
   and the check now runs on a copy in a scratch folder. **What is still owed is a
   day:** the morning after, when an item checked off today must still remind
   tomorrow, has never happened. **How the session ran:** what worked was
   putting the contrast finding to him with its numbers instead of resolving
   it quietly, which produced a better answer than either side had alone; what
   did not was an either/or question asked against rule 4 that got back a bare
   "yes" settling nothing — the same fault recorded at #7-new — named as
   Claude's own error and asked again cleanly, which settled it in one turn.
   Before it, #11-new (2026-08-21)
   **finished step 4 and built steps 5, 6 and 7, so seven of the plan's eight
   steps were in and the plan had no open questions left.** The third
   piece of step 4 turned out to be **a removal rather than a build**:
   To-Do has no snooze anywhere and is not meant to have one, its banner
   carrying a single OK button since Patrick's own call at #56, so the
   snooze and Done code in the housing could never be reached and came
   out, along with `cancelReminders` in the To-Do screen, which had been
   kept for a snooze that could not exist and was matching on a task id
   only the old scheduling ever wrote. **Patrick's reason is the durable
   part:** a To-Do reminder is advance warning that something is coming,
   an appointment fifteen minutes out for instance, rather than a prod to
   do the task, and other reminders for the same task are still coming
   behind it — so a snooze would defeat it, the appointment not moving.
   He twice trimmed the comment recording this, saying it "doesn't need
   to say all that, just the fact that it doesn't need it". **It also
   corrects the record:** #8-new had said a To-Do banner snooze "already
   buys nothing" and was live on build 57, when in truth it could never
   be made at all. **Step 5 followed in the same session** — the Memory
   Test screen no longer arms its five-minute recall or cancels anything,
   its save asks the module to run, and its own cancelling turned out to
   be in three places rather than the two described. No test was written
   or changed; 93 still pass, TypeScript clean. **Then he rebuilt, loaded
   the phone, and three things passed** — the Memory Test's five-minute
   recall, a Pets snooze all the way through, and My Week — the first of
   the module's work ever confirmed on a device; the morning-after test,
   the one that matters, is still to come. Three things came out of the
   testing: the "Snoozed till:" line cannot be read on either theme, its
   style using the color meant for text on a solid button, white on a
   white row in the light theme; "+1 Day" has gone from every My Week
   banner, so `myweekactions` is registered but never asked for and the
   `postpone1` branch cannot fire; and he restated what he wants from a
   tapped banner, the page open and the item highlighted, no scrolling —
   which is nearer than it sounds, the id already travelling with every
   reminder and both screens already drawing a highlighted row.
   **Step 6 was then built as well**, so six of eight steps are in and
   the plan has no open questions left. A new `scheduler/warn.ts` holds
   the wording in one place and the check that decides whether to speak,
   and each of six saves hands it the module's answer; it stays silent on
   the housing's own runs, which is what makes it speak as an item goes in
   and at no other time. **The words and the placement were proposed
   rather than asked about**, which is the durable part: Patrick said
   plainly that being grilled instead of helped would be reported, and he
   was right — two of the rules that failed, the "X or Y?" question and
   asking for what could be worked out, were already written and simply
   not attended to. **His diagnosis is the one to carry:** too many rules,
   not enough paying attention to them, so nothing new was added. One
   correction went with it — step 8's home was never open, the
   pending-queue screen going into Settings since #5-new, and that
   project's hand-off had been carrying it as a question.
   **How the session ran:** it opened cleanly,
   the session number had to be asked for because the chat names keep
   being changed on him — he had retyped #5-new through #10-new by hand —
   and the one real miss was a report he could not follow, after which he
   stated the To-Do reason plainly himself and it went into the comments
   in his words. He ended by saying he would commit, load the phone with
   what is built, and test what he can.
   Before it, #10-new (2026-08-21)
   **built the second of step 4's three pieces — My Day's and Pets'
   snoozes now come from the saved data — and nothing of it has run on a
   phone.** All four Snooze buttons, the two on the pages and the two on
   the banners, now write the moment down on the item instead of putting
   a reminder straight on the phone and forgetting it. The shape is the
   postpone's copied exactly: a `snoozedUntil` field beside `completed`,
   both readers turning it back into a reminder while the moment is still
   ahead, both gaining the `now` argument that tells them whether it is,
   and `mydaysnooze` and `petssnooze` joining the owned list. One stamp
   per item means one wanted reminder under one name, so **snoozing twice
   moves the one reminder rather than leaving two** — the fault the piece
   existed to cure. **The one visible change is a line on the row**,
   "Snoozed till: 4:15 PM" under the item's name, Patrick's wording and
   the page's own clock format. **Three things beyond the described piece
   had to move with it** and were reported as such: Skip now rubs out the
   stamp rather than cancelling the reminder off the phone, which stops
   holding once the snooze is written down; the on-page Log clears it too;
   and the banner's Done now asks the module to run, having relied on the
   app coming back to the front. **One judgment call, Claude's:** a snooze
   stands on its own, so an item whose time of day is cleared after it was
   snoozed still gets its snooze, because dropping it breaks a promise the
   app already made. Twelve new tests, 81 to 93, TypeScript clean. **Found
   and left alone:** My Week's Skip no longer skips a postponed chore,
   since #9-new made the postpone a stamp and the module puts it back on
   the next run — never on a phone, and a My Week session's work. The
   third piece, To-Do's snooze, is next and is the biggest of the three;
   Patrick stopped before it on Claude's count of the session's reading.
   **How the session ran** is the durable part: it opened with the same
   false sentence caught at Y-47, SA-5, SA-6 and #7-new, and Patrick's
   words were "That is not true again" and "Just maybe stop telling me the
   untruths" — the verify-before-asserting rule applies to Claude's
   account of its own session, not only to the code. Two instructions came
   out of the misses that followed: **when a proposal is behind the
   scenes, say so up front**, and **"stamp" is jargon** — the app writes
   the moment down on the item. What turned the session was asking him
   what he meant rather than guessing a third time.
   Before it, #9-new (2026-08-21)
   **built the first of step 4's three pieces — My Week's postpone and
   Look Ahead's delay now come from the saved data — and nothing of it has
   run on a phone.** **Step 4 was split into three uneven pieces** because
   the four screens that make these one-offs were not in the same state:
   My Week's postpone and Look Ahead's delay were already written down on
   the item, and both readers already read the field and did nothing with
   it; My Day's and Pets' snoozes are written down nowhere; To-Do's is the
   one #8-new found buying nothing; Orders needs nothing. So the piece
   with the record already in place went first. The two readers now emit
   the one-off under its own long-standing source, `myweekpostpone` and
   `lookaheaddelay`, both joining the owned list, and `readMyWeek` gained
   the `now` argument it never had so it can tell whether a postpone is
   still ahead. **A snooze will be recorded on the item** — Claude's call,
   Patrick having handed the decision over — because the reader is already
   given that screen's list, so there is no new plumbing and no second
   pattern for the same idea, a snooze dies with its item instead of being
   orphaned, and the screen can show it where today it shows nothing. That
   settles the next piece's shape before it is begun. **One judgment call
   changes a banner**: the "+1 Day" banner armed `myweekactions` while the
   page's own postpone armed `routineactions`, so the same act made two
   different button sets and one reader can only send one; it went to
   `routineactions`, matching the page and the chore's own weekly
   reminder, so a postponed chore's popup now carries Done, OK, Skip and
   the three Delays and can no longer be pushed a second day from the
   banner — which a postpone made on the page never could. **The housing
   stopped arming Look Ahead as well**, its `done` handler having still
   cancelled the item's two reminders by hand and re-armed the next date;
   about twenty-five lines became one call to the module. My Week's `done`
   handler kept its snooze hunt, `myweeksnooze` not being owned yet, and
   lost only its postpone half. `cancelPostpone`, `cancelDelays` and all
   five calls to them came out, two now-unused imports with them.
   Fourteen new tests rather than a few — 67 to 81, all passing,
   TypeScript clean. Patrick called for the fresh session himself at the
   close; the next piece is My Day and Pets, needing those two screens,
   their two readers and their tests. What is owed a phone is step 3, this
   piece, and the test steps 1 and 2 have still never had — the morning
   after, when an item checked off today must still remind tomorrow.
   Before it, #8-new (2026-08-21)
   **built step 3 of the scheduler plan and took Orders out of the
   reminding for good; nothing of step 3 has run on a phone.** My Week,
   Look Ahead and To-Do no longer schedule anything themselves — each
   lost its own scheduling function and its mount-time call, and each
   save now asks the module to run, the same shape My Day and Pets took
   at step 2. Their readers already existed from step 1, so nothing had
   to be written to replace what came out. **Orders needed no new
   mechanism**, which was the session's one open question and was
   answered by reading the reconcile rather than by building anything:
   it cancels a reminder whose source the module owns and which carries
   no name of its own, so naming `orders` and `orderssnooze` as owned
   while giving Orders no reader makes every reminder that page ever set
   a leftover to be swept, and with the page no longer arming, nothing
   brings them back. **A To-Do banner snooze already buys nothing** —
   found in the housing, not acted on: it is created with `source:
   'todo'` and no name of its own at `_layout.tsx` line 230, which was
   safe when it was written and stopped being safe at step 1, when
   `todo` became owned; the module now reads it as a leftover and
   cancels it on its next run, and it is live on build 57 today. Snoozes
   are step 4, so it was left alone; #9-new settled that it is cured in
   that step's third piece. **Three things stayed that a strict
   reading would have removed**: To-Do's `cancelReminders` and Orders'
   `cancelForItem`, both matching by item rather than by source, so they
   still clear a pending snooze the module cannot see; and the cancel
   halves of Look Ahead's and Orders' cancel-then-re-arm lines, where
   only the re-arming came out. One test asserted exactly what step 3
   reverses and was rewritten, with a second added for Orders snoozes —
   67 tests now, all passing, TypeScript clean. **Step 4 was next and
   got a fresh session**, on Patrick's own question at the close: it
   lives mostly in the housing, where about six hundred of
   `_layout.tsx`'s six hundred and forty-eight lines are the seven sets
   of banner buttons and the handler beneath them, plus the on-page
   Snooze buttons in My Day and Pets, My Week's postpone and Look
   Ahead's delay. #9-new took the first third of it.
   Before it, #7-new (2026-08-21)
   **built step 2 of the scheduler plan and got it onto the phone as
   build 57, and Patrick wants the whole rest of the plan before the
   next build.** My Day and Pets no longer schedule anything
   themselves — each screen's own scheduling function is gone, its
   mount-time call with it, and its save now asks the module to run, so
   the module is the only thing arming those two screens. About
   thirty-six lines out of each of two files and two lines in.
   **The always-arm rule was already in**, applied at step 1 where both
   readers ignore whether an item is checked off, so removing the
   screens' own scheduling *is* the fix for the silence and nothing had
   to be added for it. What deliberately stayed: both on-page Snooze
   buttons, which tag themselves `mydaysnooze` and `petssnooze` and are
   not sources the module owns — snoozes are step 4 — both permission
   asks, since the module checks permission but never asks, and My
   Day's Siri publish. **The old keyless reminders take care of
   themselves**, confirmed by reading the reconcile rather than assumed:
   a reminder from an owned screen carrying no name of its own is
   treated as left over from the old way and cancelled, so the
   accumulated My Day and Pets requests are swept the first time the new
   build runs. TypeScript clean, 66 of 66 tests passing. **Step 1 was
   never separately tested on a device**, on Patrick's own ruling at the
   top of the session — step 2 first, then one phone test covering
   both — and what build 57 has not had is a day: the real test is the
   morning after, when items checked off today must still remind
   tomorrow. A fumble worth recording: the first build and submit were
   run from the `Students-Assistant` folder by mistake, so a
   Students-Assistant binary went to TestFlight, harmless because it is
   simply never distributed, and the Memory build was then made from the
   right folder. **Orders is dead to him** (his own words), so it gets
   no reader, its scheduling comes out at step 3, and its old reminders
   are swept rather than left sitting — which settles the #6-new note
   that had left them alone until the page went. **Steps 3 through 8 are
   all wanted before the next build**: told that today's untapped banner
   will still be in Notification Center tomorrow because the sweep is
   step 7, he said he needs another build anyway and wants it sooner
   rather than later, and asked how much of the plan he wants in first,
   answered "all" — one at a time, each proven before the next. Step 3's
   shape is agreed and not started: My Week, Look Ahead and To-Do move
   to the module, Orders stops with them. The session was ended on
   purpose before step 3, about four thousand lines having been read
   against more than that again ahead. Where it was thin: it opened with
   the same false sentence recorded at Y-47, SA-5 and SA-6 — that the
   rules files had not arrived on their own, when both were in front of
   Claude from the first moment — and three either/or questions followed
   against rule 4, each producing a "yes" that settled nothing, the last
   of them making Patrick point out that the session's own sequence was
   not hard to follow. He asked twice for smaller steps and shorter
   messages, and said plainly that the code detail is not what he needs
   to be told.
   Before it, #6-new (2026-08-21)
   **built the whole of step 1 of the scheduler plan, and none of it has
   run on a phone.** One module now owns every reminder: a new
   `scheduler/` folder at the project root holding the shape of a wanted
   reminder and the key that names it, six plain readers — My Day, Pets,
   My Week, Look Ahead, To-Do and Memory Test — the reconcile with its
   budget trim, one impure file that reads storage and the phone's queue
   and applies the answer, and a test setup in Mystery's shape: a
   ten-line runner, no framework, 66 tests, headless under Node in about
   a second with no build and no simulator. It went in four pieces, each
   proven before the next was started and each given its own go. **Only
   two existing files changed** — `app/_layout.tsx` gained one import and
   one small effect calling the module on launch and on every return to
   the front, reusing the AppState listener the Siri note already had, and
   `tsconfig.json` gained `"allowImportingTsExtensions": true` so Node can
   run the files without a build. No screen was touched, so both places
   still arm, which is what step 1 is meant to be: the reconcile matches
   by name, so nothing can be created twice. **Orders gets no reader** —
   Patrick is removing that page as soon as it is convenient — and the
   consequence was named rather than guessed at, since a reconcile that
   cancels anything unwanted would have killed a live page's reminders;
   the answer is that the module owns only the sources it has readers for
   and leaves everything else where it is, counting it against the room
   the phone has, exactly as the plan already treats Timer. Four decisions
   were named as judgment calls before they were agreed: the always-arm
   rule was applied at step 1 rather than step 2, because writing the two
   daily readers the old way would only mean rewriting them one step
   later; each reminder carries its own name and firing times inside it,
   so the reconcile never interprets the phone's own description of a
   trigger, which differs by kind and by version; the module checks that
   notifications are allowed but does not ask, the screens still doing the
   asking; and the ceiling is sixty-four less eight kept free for the
   Timer, the eight being Claude's number. The To-Do background daily now
   has one name, so the pile-up cannot recur. My Week's postpone and Look
   Ahead's delay are already saved and were deliberately left to step 4,
   where the plan puts them. One test failed and the code was right — a
   date already in the past, correctly dropped — and whether Metro accepts
   a `.ts` on the end of an import was checked by bundling the whole app
   rather than assumed. What is owed is a build and Patrick's phone.
   Before it, #5-new (2026-08-21)
   **found why the reminders fail and wrote the plan to fix them**,
   touching no app code. Patrick built #4-new, loaded it, and the
   notifications still did not work. He opened with questions rather
   than answers — whether an early choice between an easier road and a
   more reliable one was to blame — and no such choice is written down
   anywhere; the app has always used native local notifications through
   `expo-notifications` in real EAS builds, which is the only road on
   an iPhone that fires alarms with no server and with the app closed.
   His own answer was that he does not care why, he wants it to work,
   and he named the stake: a second app is being modelled on this one,
   and without reliable reminders there are no apps. The read he then
   asked for covered `app/_layout.tsx` end to end and the scheduling in
   all eight screens that touch notifications. **My Day and Pets
   destroy their own daily repeats** — each cancels every one of its
   reminders and re-creates them only where the item is not completed,
   so checking something off removes its repeat. **Nothing ever puts it
   back**, because only the owning screen re-arms and only while it is
   open; the housing arms nothing, the Home screen arms nothing, and
   `app.json` declares no background modes. My Week does not have the
   fault, arming every chore regardless, which is both the proof and
   the shape of the fix. **A separate, non-structural bug** in the hour
   stepper of `components/DateTimeControl.tsx` is wrong across the
   twelve o'clock crossing, so a nine o'clock morning time set by
   spinning down from the noon default is stored as 9:00 PM — Patrick's
   own symptom, seen twice. **The plan was written that session** — it
   lived at `elderlyassistant/docs/scheduler-plan.md` until #12-new
   finished it and folded it whole into the foot of that project's
   `docs/build-history.md`: one module owning the
   whole queue, readers turning each saved list into wanted reminders,
   keys that make duplicates impossible, a reconcile that leaves
   matches alone, and a budget below Apple's sixty-four — run on
   launch, on every return to the front, and after any save. Six things
   settled into it. Snoozes, delays and postpones get saved so the
   module owns them, on his own framing that a snooze is the second
   chance and its absence the least likely to be noticed. A clean slate
   every day, the midnight holdover gone in both halves, because a
   thing not done on time is of no use as a reminder — the past-day
   behavior existed for the log rather than the reminding, and a missed
   item now simply stays unchecked. The daily reset moves into the
   module. A reader stays plain — no storage, no iOS, nothing from
   React Native or Expo — so Node can run it without a build, decided
   before the readers exist because pulling the reads out later means
   rewriting all seven. The tests follow Mystery's shape, read this
   session at `engine-tests.html`: a ten-line hand-rolled runner, no
   framework, headless under Node, tests writing to their own storage
   keys; this project has no test runner and no test files at all
   today. And Timer stays outside the module as a special case, with
   Patrick noting in passing that Timer is not working right now
   either. A screen showing the pending queue goes into Settings. The
   ceiling was worked through and is pending scheduled requests for the
   whole app, a repeat costing one slot forever — Memory will not come
   near it, Students-Assistant might, and the answer there is rolling.
   The budget warning fires as an item goes in rather than when a
   reminder fails, and never for ordinary rolling. Its wording and
   placement is the plan's one open item, left until there is a screen.
   Two slips are recorded: Claude drifted into tracing the time bug
   unasked, and wrote a snooze recommendation as law, both caught by
   Patrick. Before it, #4-new
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
4. **Students-Assistant — iPhone and web** — Alpha, and it is on his
   phone.
   Folder: `Projects/Students-Assistant`; its CLAUDE.md names the
   reads, and the layout follows `MysteryCluesTracker` — `docs`
   active, `docs-ref` reference. Status: SA-15 (2026-08-23) **built the
   scheduler whole, built Backup & Restore, and gave the app its name.**
   The app is **Still To Do** on the App Store and **Still-2-Do** under the
   icon; everything else keeps the old name, the folder and the repository
   included, and `ios.bundleIdentifier` could never have moved without
   orphaning the TestFlight build. Classmate was his first answer and the
   check killed it within the hour — *ClassMate — Student Tool App* is live
   and is her field exactly — and Cue, Don't Forget, Remember, Remember To
   Do Today and Still Due all fell after it, the last two refused by App
   Store Connect itself, which is the only real check. **The scheduler
   works and owns every reminder on the phone:** three of Memory's files
   copied across, one reader where Memory has six, `scheduler.ts` rewritten
   for one storage key, and a housing that asks permission, registers the
   buttons, runs the module on launch and on every return to the front, and
   opens a tapped banner on its entry. **Two rulings shaped it.** A single
   event's banner carries Done and the three snoozes and a recurring one
   carries OK alone — drawn by whether the item recurs, never by when the
   banner fires — and permission is assumed by her use of the app, so the
   phone's own box comes up with nothing of ours around it and nothing said
   if she declines. Done from a banner marks the occurrence rather than the
   day of the tap and clears the snooze with it; a snooze is written on the
   entry and the module arms it, so a second snooze moves one reminder
   instead of leaving two. Memory's stale-banner sweep came across on his
   ruling: "We will assume it fired. Then it means she did not
   acknowledge. That does not matter. It should be taken down" — and it
   touches the banner only, never the entry. **Backup & Restore** carries
   everything the app has stored rather than a named list, because Memory's
   fixed list has quietly forgotten things before and a card's text is
   filed under its own card's id; and **the restore merges**, on what he
   had actually come to Memory needing — "restore only what is different,
   and ask whatever needs a decision" — which was reported with its cost
   attached, that a card deleted after the backup comes back. **The durable
   thing about how the session ran is the verify list**, `docs/verify-list.md`,
   which he asked for early: what needs testing and what to do to test it,
   because two thirds of the previous session was invisible to him. Every
   piece added its steps as it landed and the twenty-six cases checked
   outside the app are recorded there so nobody repeats them by hand.
   **The open list went from twenty to one.** He cleared them in a single
   pass — the back burner archived to `docs-ref/back-burner.md`, questions
   for his granddaughter that are not about the app ruled not to pertain,
   the feature draft archived unread, and the rest answered by number: no
   laptop half at all, all of her reminding is hers to set, Cancel may not
   throw her typing away on one tap, and the Scheduled Reminders page shows
   what Memory's shows. What is left is his own want from SA-14, that an
   undone past item should still hang on today. **Nothing built has been on
   a screen** and the phone needs a new build, the TestFlight one being
   from SA-8. Two faults, both loose language rather than loose work:
   setting a question aside was turned into an answer of Claude's own, and
   the scheduler being finished was reported as the app being done. He
   caught both.
   Before it, SA-14 (2026-08-23) **archived the
   Week's View, cut Today's View back to today alone, and settled what Done
   means.** The session's real work was Patrick narrowing one problem until
   what it actually was could be seen, and every step of that narrowing was
   his. Done writes the real today, so any page standing on another day can
   mark the wrong one; a one-time item cannot get it wrong, reading as done
   off any mark at all, and standing on today cannot get it wrong either —
   so the whole fault lived in one place, a recurring item tapped from a day
   that is not today. Looking back at last Tuesday from a Thursday turned out
   to do no harm, the mark landing where the item never appears, and **his
   own summary is the durable part: other than for bookkeeping it does not
   matter when the mark is recorded for, and if only looking back makes it
   matter, then we do not look back.** Claude was wrong once inside that and
   he caught it — it had been claimed she must page to another Tuesday to
   reach the item, where the week page shows all seven days at once. **After
   a night's sleep he decided the Week's View is not needed and Today's View
   does not step forwards or backwards**, which cures it completely because
   she is then only ever standing on the day the mark is written on. Its
   cost is her looking ahead, and his answer to the cost is that looking
   ahead was never what kept her from missing things — the reminders are.
   The page is archived rather than deleted, at `archive/week.tsx`, out of
   the routes and out of the type checker. **The card page was not cured by
   any of that, and his correction of the framing settled the rest:** on a
   card there is no day to be standing on, so she is not opening Tuesday's
   item but an item set to fire next Tuesday, and **for a recurring reminder
   Done is for the next single occurrence only, Delete being the only final
   done, while for a one-time reminder Done is done.** The consequence made
   the build small: because the answer is always the next occurrence, the
   day she was standing on never has to travel anywhere, so the plumbing
   proposed at the top of the session was not needed and the row no longer
   takes a day from anybody. Two tidy-ups followed at his ask, and the first
   was not the harmless clutter it had been called — turning a repeating
   item into a one-time one would have left old marks behind and had it
   arrive already finished. Doing it turned up a fault that would have been
   silent: reading a stored day back the obvious way is a day out here, a
   written-out date being read as a moment in Greenwich, so every Tuesday
   would have come back a Monday and the pruning would have discarded
   exactly the marks it was meant to keep. Both the occurrence arithmetic
   and the day-parsing were checked with a scratch script rather than in the
   head. **Nothing from the session has been run**, and neither has SA-13's
   `completedDays` change; he chose not to load. One want of his is recorded
   and unbuilt, and it matters more now that the looking-back is gone: an
   undone past item should still hang on today and be tappable, and nothing
   delivers that. **The session opened with three failures and a close
   call**, all named by him before any work began — the same false sentence
   about the rules files not having arrived that is recorded at Y-47, SA-5,
   SA-6, SA-7 and #10-new; a second ask stacked onto one turn; a question
   re-asked that he had answered at the close of SA-13 and answered often
   enough to end that session over; and the running reported off the
   hand-off when that very file says to ask him. He came within a sentence
   of quitting and asked outright whether Claude could handle the session.
   What turned it was reading the conversation back rather than defending,
   and afterwards going at his pace — single questions, no jargon, and two
   thoughts he held aloud read back to him before anything moved. He ended
   by taking the scheduler, which is the next build and whose read is
   already done, into a session of its own.
   Before it, SA-13 (2026-08-22) **built piece
   three, read Memory's scheduler whole, and turned the done-day into a
   list of days.** Piece three finishes SA-12: the two views are read-only
   now, a tapped row pushes the card page carrying the card's id and the
   entry's, and the card page opens that entry. **Every road out returns
   her to the view she tapped on** — Patrick's own settling of what SA-12
   had left open, "It should take her back to wherever she came in from" —
   while a pop-up opened by ＋ Add on the card page still closes in place.
   He ran it: "Nice and clean." **The record was wrong about the running,
   and nobody had asked.** This file and the project's own said nothing
   from SA-12 had been on a screen, and that was reported back to him as
   fact; he has been verifying in the simulator all along, and said so —
   "You just haven't asked." A document is not a verification.
   **Memory's scheduler was read in two halves**, the core and then the
   housing, so no session reads it again. Three files copy across
   untouched — the shape of a wanted reminder, the reconcile with Apple's
   sixty-four ceiling, and the near-the-ceiling warning; `scheduler.ts`
   gets rewritten for one storage key; one reader replaces Memory's six,
   modelled on its To-Do reader, which already holds her nine presets and
   reads the three Settings times this app already writes. The housing
   collapses to one button set, one handler branch, and a banner tap that
   pushes the card page by the road piece three just built. **The weekly
   repeat is not used, on Patrick's own proposal:** each reminder is a
   date alarm aimed at the next occurrence and the module works the whole
   set out afresh on every run, which also dissolves *Week* and *Month*,
   sayable as a moment but not as a weekly repeat. Its cost was named —
   a week she never opens the app arms nothing for the week after — and
   his ruling outlives the mechanism: "If she doesn't open up for a week,
   then she doesn't need it." A banner's Done marks the day and time it
   fired. **The done-day became a list on his own find:** `completedOn`
   held one day, so a weekly entry marked two Tuesdays running kept only
   the second and paging back showed the first undone — every week before
   the most recent one reading as not done. `completedDays` replaces it,
   with entries already on the phone brought forward, so no reset is
   owed. **What is open and stopped the session** is which day Done counts
   for. It marks today and always has, the form never knowing which day
   she was standing on; piece three widens that, the entry now opening on
   the card page. His design is recorded and unbuilt — every road leads
   into the one modal and the decision is hers there, the modal asking
   "Mark Tapped today?" — and it has not been reconciled with his earlier
   word that Done should not be tappable in the future or the past.
   **The session ended early**, on "Lets end this session. before I lose
   my mind." Two failures of the same shape: the hand-off's line about the
   running was asserted instead of asked, and then his question to her was
   converted into a fixed law that Done always means today, taking the
   decision away from her — the invented-ruling fault Y-38 recorded,
   reached by collapsing a question into a statement, and not seen even
   after "That was a question??????????????????????????"
   Before it, SA-12 (2026-08-22) **gave the
   Week's View everything Today's View had, turned the Courses page into
   the place entries are made, and built Done.** The Week's View now
   carries the week offset, the swipe, the wall, the away shades, the
   pulse and the *Back* pill, all copied from Today's View so the two
   behave alike. **How far it reaches is the semester and nothing else**
   — it walls at the week holding the start date and the week holding
   the end, off a new `constants/Semester.ts`; and **with no dates set
   it does not move at all**, which was Patrick's correction of a
   proposal that would have let her page freely until they existed.
   **The session's longest stretch was working out what "the Entry page"
   was**, a page the record had never named. Claude did not know,
   searched the docs and the previous transcript, found nothing, and
   asked again after he had told it to look the thing up itself — which
   drew "I really dislike this adversarial attitude you have developed
   these last two sessions". What it turned out to be is the **Courses
   page**: one page and not two that look alike, its name settleable
   later, with the semester's dates at the top and cards under them. The
   entry modal comes off the two views onto it, the views become
   read-only lists, and **every entry lives in a card** — anything
   outside her courses gets a card of its own, "to keep it organized".
   **Tapping a row on a view opens that item on the card page**, because
   a row that does nothing reads as broken and the alternative makes her
   find the item again when she was looking straight at it; closing goes
   back to the view, which costs nothing since the view is still on the
   stack. Three pieces were built: the cards became hers, saved under
   `sa_cards` and seeded once from her five real courses, with ＋ Add and
   **a left swipe uncovering Edit and Delete** on a *Sure?*; entries moved
   onto the card page, whose header took a third button and put its title
   on a line of its own; and **the card page was trimmed to his own list**
   — meeting lines gone, Office hours onto the class-name line, Schedule
   gone as the class times, Materials and Grading side by side in a box
   each, and Assignments and Important dates gone "because that is what
   she will enter the way she wants". **A row now names its reminders
   rather than counting them** in his own abbreviations — 30m, 1h, 2h,
   Mof, DB, NB, 2DB, W, M — all of which fit, "there is enough room".
   **Done closed the question SA-11 asked three times.** He said a weekly
   entry's Done should repeat automatically, "how it is done in My Day,
   Pets Day, and My Week", and the read of Memory's `dailyreset.ts` found
   a whole-list sweep at the roll of the day. **That does not carry
   across, and the reason is this app's own: the views look backwards.**
   A swept list would show last Tuesday's reading as not done when she
   pages back to last Tuesday, so an entry remembers the day it was
   marked instead — `completedOn` replacing the old true-or-false — which
   also needs nothing to run, so a week with the app closed cannot leave
   a stale checkmark. Done sits in the entry pop-up, asks first, and undoes
   on one tap; **it lives in the notification banners too**, which waits
   on the scheduler. Left for a fresh session: piece three, the views
   routing a tapped row to the card page and closing back. **Nothing built
   this session has been run** — not the swipe, not the two new pop-ups,
   not the semester line, not Done — TypeScript is clean, and nothing has
   gone to TestFlight. An entry already on the phone carries no card and
   no `completedOn`, so it shows in the views but on no card page; Reset
   All Data is the cure. His verdict on the building was "Everything looks
   excellent. Good job"; the cost of the session was all in the talking,
   where Claude flagged his reversal of an agreed decision as a conflict
   ("SO WHAT?") and quoted the rules at him mid-session ("Stop telling any
   rules if you cannot control yourself").
   Before it, SA-11 (2026-08-22) **finished
   the shared pieces, built the Week's View, and gave Today's View a way
   to thumb through the days.** The row and the form that SA-10 stopped
   mid-stream are now `components/EntryRow.tsx` and
   `components/EntryForm.tsx`, so neither page carries a copy of its own;
   `app/today.tsx` went from 537 lines to 181, and the form holds its own
   draft, never touches storage, and hands a finished entry back. The row
   turned out not to be half-written at all — it already matched what the
   page drew inline, value for value, plus the date line the wider windows
   need. **The Week's View is `app/week.tsx`**, the calendar week she is
   standing in, Sunday through Saturday, whole; and it is **the same page,
   not a new shape** — Patrick's own "I don't understand why it cannot be
   the same", and he was right, the row's `showDate` having been built for
   exactly this. Claude had put it to him as a choice when the answer was
   already sitting in the code. **The session's largest piece began with
   the long look and replaced it.** He first doubted a semester view, then
   named what actually matters — her priority, and maybe the only thing
   she wants from the app, is not to miss anything important, and she has
   other resources for the longer looks — and then proposed the answer
   himself: let Today's View page to tomorrow. It swipes seven days either
   side of today and stops at **a wall**; the title becomes the day's name,
   the pill becomes *Back*, and the header and ground take **away shades**,
   two new colour names in both themes that hold their darkness because
   the header's text and pills are painted on them. A **pulse** of three to
   five seconds runs once when she leaves today and once when she returns,
   never on every swipe. The day and date heading was made present after
   his own "that is so unnoticeable I didn't see it" — it was 15-point
   muted grey carrying the only statement of which day was on screen. The
   pages are now **Today's View and Week's View**, *Tasks* struck from both
   headers and both tiles, and the Course page's clipping pill became
   *Back*. His verdict on the day-stepping: "I like it. It's easier and
   smart." **The durable ruling is the confirmation rule's refinement.**
   Done belongs in the entry pop-up and takes two taps; Claude called that
   an override of Patrick's own Y-34 rule and was wrong. His correction:
   Done is not a constructive action, it wipes away important information
   with costly consequences, the confirmation costs one tap where the loss
   is a missed due date and a failed test, over-use is no risk in an app
   that barely confirms anything, and her missing something is why the app
   exists. So an action counts as undoable only when undoing it puts back
   everything it took, consequences included. **How the session ran is the
   part worth carrying.** Claude then argued the point after he had ruled,
   holding his own decision up against his own rule — "there are a dozen
   ways I do not agree with you, and I know what the rule means", and
   "there are more than one rule against arguing with me, especially about
   rules." He ended the session tired and then asked for the docs refresh.
   The lesson is his: the rules are for how Claude works, not a standard to
   hold Patrick's decisions against. Also: the same weekly-repeat question
   was asked three times in three phrasings and never landed, and it is
   still open — `completed` is one true-or-false, so Done on a weekly entry
   would mark it done forever. Nothing marks an entry done yet, the Week's
   View has none of the day-stepping work, and none of it has been built to
   TestFlight.
   Before it, SA-10 (2026-08-22) **settled
   what an entry is and built Today's Tasks.** The work went backwards
   from the firing, which was Patrick's instruction — settle what a
   reminder needs before deciding what she types. **Only work reminds:**
   a class repeats, so its reminders look as though they should repeat
   with it and they do not, each meeting carrying its own thing to do;
   and he went further, that she needs no reminder for the class at all,
   only for assignments, tasks and due dates. **An entry says when in
   one of two ways** — a date for something that happens once, or a
   weekday for something that happens by day rather than by date, which
   comes back every week — and either may carry a time and reminders or
   neither. A date is required, a time is not, and with no time set
   nothing fires and the entry simply sits in her list for that day.
   That closes the SA-9 question of what an entry holds and how a repeat
   is expressed. **Her presets are Memory's To-Do nine unchanged** and
   the banner carries the standard 15, 30 and 60 snoozes; a due date
   gets several reminders between now and then rather than one, and
   which she ticks is her choice. The read behind it found that only six
   of the nine work without a time — three are offsets counting back
   from the time, six are clock reminders counting back from the date —
   so a timeless entry can still take Week or Day Before, and taking a
   time away takes any ticked offsets with it. **The durable ruling is
   the consistency one.** The date and weekday pickers were first built
   with a switch above them, and Patrick asked why a switch rather than
   just putting the day row on the page; the reason given was that an
   entry is one or the other in the data and the choice was made visible
   rather than inferred, and he pointed out that inferring it from a
   touch is exactly what the time half already does. The cost was named
   before it was built — the time half can do without a switch because
   it has an asleep look and the date stepper had none — and both
   pickers now sit on the form with the last one touched live and the
   other dulled at the same 0.4 opacity, still tappable, which is how
   she switches back. Built: `constants/Entries.ts` holding the pool
   under one storage key so all three pages read the same one, and
   `app/today.tsx`; a Today's Tasks tile on the home page; and **＋ Add
   as the round pill in the right of the header**, opposite Home, which
   he called simple and elegant and made the pattern for all three
   pages. A row with no time says "Anytime" on his ruling, because the
   row is telling her when and anytime is a real answer. TypeScript is
   clean and he verified in the simulator as the session went. Left
   unfinished: the shared row and form were agreed and then stopped,
   `EntryRow.tsx` written and unused and `EntryForm.tsx` refused
   mid-write; a weekly entry's reminders need a weekly trigger and the
   scheduler is not built; nothing marks an entry done; and Cancel still
   throws typing away on one tap, still unruled. **How the session ran
   is worth carrying.** Its worst miss was reporting Patrick's own
   sentence about the snoozes back to him as a discovery and then
   dressing it as a collision he was asked to resolve — nothing was in
   collision, and he named it exactly. Twice he said the messages were
   too long, and an empty "I'll wait" drew the right rebuke since he had
   been verifying all along. What worked: reading Memory's code rather
   than trusting the hand-off's line about it, naming the cost of the
   consistency ruling before building it, and reading his double
   negative back to him instead of picking a side of it.
   Before it, SA-9 (2026-08-22) **cut the app
   back to what it is really for and built its Settings page.** Patrick
   opened by saying he had gone after the wrong pages first: Courses and
   its cards go to the back burner, not thrown away, and the heart of the
   app is Today, This Week and This Semester, which his granddaughter
   fills in herself, with Home and Settings for support. All three come
   from Memory — Today from My Day, This Week from My Week, This Semester
   from Look Ahead — and he set the order himself, Settings being the
   easiest. **The session's largest outcome is that the three pages are
   not three kinds of thing at all.** They are three window sizes onto one
   pool of entries she has made: Today shows what falls on this date, This
   Week these seven days, This Semester the whole stretch, and whether a
   thing repeats belongs to the entry rather than to the page. That
   replaced a split Claude proposed between a day's repeating part and its
   one-off part, and his reason for rejecting it is the durable part — the
   days are as consistent as the weeks and the weeks as inconsistent as
   the days, so the split buys nothing; consistency is not a property of
   the time unit. His own note as the session closed is that it reshapes
   all three pages, which also makes the My Week and Look Ahead reads
   still to come reads for their furniture rather than their shape.
   **Settings is built** — five sections after he struck Memory's Security
   with it, this app having no Vault — with the three reminder times
   saving under Memory's own storage keys so the scheduler will find them,
   the gear on the home page wired to open it, and Memory's shared date
   and time control brought across for the time pop-up. Two rows are drawn
   without a tap because their pages do not exist. TypeScript is clean and
   nothing has been run on a phone. The build order from here was handed
   to Claude and is Settings, then the three pages, then Memory's
   scheduler module last, because a reminder is about a task and there are
   no tasks for it to be about until those pages exist. **Siri is deferred,
   not dropped**: Memory's `app-group` module turned out to be Siri
   listening rather than speaking — she speaks, an App Intent writes a
   note into a shared box, the app applies it on its next return to the
   front — which is the opposite of what he had assumed. **The name hunt
   was real and is shelved.** Classmate, Classpanion, Class-panion and
   HEY! were weighed; HEY! went because a well-known email app carries it
   and because a shout collides with an app whose reminder is never
   demanded, and Classpanion went on a finding the search produced rather
   than reasoning — no app uses that exact word, but Class Companion is a
   live education product for schools, and Classpanion is a contraction of
   exactly that phrase in exactly that field. The app stays
   Students-Assistant and nothing in the code depends on the name.
   Before it, SA-8 (2026-08-22) **made the
   first real build and put it on his phone through TestFlight,** and
   settled four things that had been standing in front of the work.
   **The road to a phone is EAS to TestFlight**, settled not by what is
   easiest but by what he wants — his granddaughter must be able to
   load it on her own phone in the easiest way, and only TestFlight
   reaches her at all. Nothing in the record had ever ruled on this;
   the hand-off's `npx expo run:ios` line was a description of what
   existed. Build 3 shows "Ready to Submit", which means Apple has
   finished and it has not been sent for the external review he has
   never had to do for Memory; nothing appeared in TestFlight at first
   because his own box in the internal group was unchecked, and he
   found it himself. Adding his granddaughter is parked — either as an
   internal tester, which needs no review but puts her on his developer
   account, or as an external group, which needs the review.
   **The app has an icon**, drawn this session after the read found it
   had none at all. His idea was a happy face with a graduation cap; it
   follows Memory's own shape, where the whole square is one colour and
   the drawing sits on it as line work with no backdrop, and every
   colour comes out of `constants/Themes.ts`. Expo 54 takes `ios.icon`
   as an object of `light`, `dark` and `tinted`, confirmed from its own
   v54 reference. One correction the work turned up: Memory's *header*
   icon is not its app icon but a transparent silhouette painted with
   `tintColor`, so nothing blends — and Memory's field `#eec55a` and
   its dark header `#f0a83a` are near but not equal, which Patrick said
   he cannot see and does not care about.
   **The pages carry Memory's headers**, home and sub-page both, with
   `Bridge` copied across. The read found a real bug with them: the old
   "Courses" title was painted `titleText`, white in the light theme,
   sitting on the pale page background instead of on a teal bar. The
   gear is drawn for balance with no tap at all until Settings exists.
   **The page list is settled** — home with tiles, Courses, what sits
   behind a card, Today's Tasks, This Week's Tasks, Reminders and
   Settings; This Semester a maybe; travel, gap filling, calendars and
   maps out for now. Reminders sits inside Settings and Settings behind
   the gear, which is his own observation and briefly collapsed the
   home page before the two Tasks pages brought the tiles back.
   **A card opens as its own page**, closing what SA-6 settled and SA-7
   reopened. Both were built and compared, and his own question decided
   it: which is easier for entering data, that being the main purpose.
   A page sheet can be swiped away mid-typing — the same fault he
   flagged in the Mystery app's Edit pop-up — the structure is three
   levels deep so a page opens another page naturally, and the keyboard
   is easier on a page. Behind each card are six sections, all
   enterable and all saved on the phone, which he will fill in from the
   syllabus. Two things left unruled: Cancel throws typing away on one
   tap, named to him rather than cured by invention; and whether
   calendars are dropped or only deferred, which collides with SA-6.
   **How the session ran is the part worth carrying.** The first half
   hour was lost entirely to Claude asking the same question four times
   when Patrick had answered it in his first reply — "no you can not
   follow a simple conversation" and "why do I have to lead you
   around" were both his. He then asked in plain words that Claude stop
   asking more than one question at a time, after a message ended in
   two and his "No" answered neither clearly. A permission dialog for
   deleting one file asks for deletion rights across a directory, and
   he read it as a request to delete his project folder and refused it;
   he was right to, deleting is his, and the file was wanted again an
   hour later.
   Before it, **the leave-by alert is
   dropped** (Patrick, #5-new, in Memory's session) — not deferred,
   dropped, because travel is already handled by the bus route apps
   she has, so the app has nothing to add there. That overturns SA-2's
   "not abandoned" and SA-5's "survives the ruling intact", and it is
   recorded in that project's `docs/app-structure.md` above the
   superseded paragraphs and in its `docs/handoff.md`. What it leaves
   unasked, and Patrick will take up in that project's next session:
   the travel time is still entered at the first sitting and nothing
   now consumes it. Before it, SA-7 (2026-08-20) **started
   the build**, and the project stopped existing on paper only. The
   Expo project was written by hand rather than created by Expo's own
   command: the sandbox can run it — Node, npm and the registry all
   answer — but Memory's `node_modules` is 404 megabytes across 39,969
   files, and every one would cross the mount for an install only ever
   used on Patrick's Mac, so Claude writes the project's files and he
   runs `npm install`. **It starts on Memory's versions rather than the
   current release** — Expo 54.0.33 against 57.0.15 — because code is
   going to be copied across and a version gap turns every copy into a
   compatibility question. Memory's dependency list came across whole,
   `expo-dev-client` with it, which is why the QR code and Expo Go are
   both dead ends and `npx expo run:ios` is the road; the phone still
   has no build on it. **The card's face is built and seen** in the
   simulator, five courses with one, two and three meeting lines
   underneath, `constants/Themes.ts` wired in through its own
   `ThemeProvider` and the palette's keys — `card`, `cardBorder`,
   `cardTitle`, `mutedText` — agreeing with the project's language
   without renaming. The page list did not block any of it, because
   SA-6 had settled that a card belongs to no single page. Four things
   Patrick settled with it. **The home page carries tiles**, called
   tiles in what is said and in the code alike, which came out of his
   own question about how "badge" is used — everywhere else it means
   the notification count on an app icon or a small pill attached to
   something, and an app leaning this hard on reminders would have both
   meanings live at once. **Office hours live behind the card, not on
   its face.** **Whether a card opens as a modal or as its own page is
   reopened** — the card is not in question, the opening is — so the
   tap is unwired and `docs/dictionary.md` carries the entry as
   reopened. The same session corrected how that file works: **Patrick
   decides what goes in it and Claude does the writing**, which is not
   what "nothing is added except by him" had been taken to mean. And
   **reminders are the priority while travel and gap
   filling go to the back burner**, which he brought back from talking
   with his granddaughter mid-session; they are held as deferred rather
   than deleted, the squeeze warning stays live as pressure rather than
   gap filling, and Travel comes off SA-6's proposed page list. The
   session also read a real UNL syllabus template he downloaded,
   `docs-ref/Syllabus_template_2025July18.docx`, which corrects three
   suppositions: the syllabus header carries no meeting time or room at
   all, so the card's face is part syllabus and part class schedule;
   office hours are real, in an instructor block of their own; and the
   dated schedule is optional and instructor-discretion, so the app can
   never count on one existing — his own SA-6 ruling that she enters
   the tasks herself, arriving with more force. Confirmed as supposed:
   the grading breakdown with weights, and repeated small assessments
   counted as one item. Named and not proposed: UNL's attendance policy
   carries a countable threshold. His one complaint is now rule 25 in
   `Projects/CLAUDE.md` — Claude writes far too much for him to read,
   and length is its own fault independent of quality.
   Before it, SA-6 (2026-08-20) started a
   dictionary and settled that **the syllabus is the structure**,
   touching no app code and never beginning the build its opener had
   named. Patrick's own words were that it is there for us already
   and there is no need to reinvent the structure: the card's face is
   the syllabus header, the modal behind it is the rest of the
   document, the dated schedule is already the task list and arrives
   flat rather than nested, and the grading breakdown is the
   grouping. **It can arrive as a download — can, not does**, his own
   correction, since she can enter all of it herself and may have to;
   the app fills in the overhead it can read and **she enters the
   items and tasks as she sees them**, which he said she actually
   should, the bite being a judgment about her own working that no
   parser can make and the squeeze warning firing as she enters, so
   her entering is the mechanism working rather than overhead. The
   dictionary is his own — `docs/dictionary.md`, ten definitions in
   his words, and from SA-7 he decides what goes in it while Claude
   does the writing — and it moved a
   word: **a course is a card and not a tile**, a tile being the pad
   an icon sits on, and **a card opens as a modal**, which closes
   both of the things the hand-off had carried as standing in front
   of the first buildable piece. **There is one top card**, with how
   many levels sit below it expressly undecided. **The card is the
   room** — doors let her in, windows let her view, buttons live at
   the window and editing happens inside — so a room has several
   doors and windows and belongs to no single page, which makes the
   card one piece written once with several ways in. **She sees three
   calendars, Day, Week and Month**, the same three on both devices
   with the laptop showing more of each; a course can be opened from
   the calendar, and a list is a second way in, the calendar being
   the time door and the list the thing door. The session's one code
   read found Memory's housing far smaller than its line count: only
   the last 22 lines of `_layout.tsx` are the frame, the other 608
   being seven sets of banner buttons and one handler beneath them,
   which is the reminder structure Patrick asked to borrow and which
   lives in the housing rather than in the pages. Also settled: **the
   word we say and the name in the code are the same word**, with the
   code following the language because this app has no code yet and
   his words are already in the documents — now a working note in the
   project's `CLAUDE.md`. The session opened badly for the third time
   running, with the identical false sentence about the rules files
   not having arrived on their own, followed by proposing a Memory
   read before opening this project's own structure file and by
   manufacturing a naming conflict Patrick said did not exist. He
   said he was really uncomfortable with the performance and offered
   an outage as the cause; it was declined as untrue, elevated error
   rates making requests fail rather than making sentences false.
   What turned it was his asking where it was best to start and being
   given a reason rather than a question, and his saying that he
   would rather Claude work things out with him than sit asking what
   he wants.
   Before it, SA-5 (2026-08-20) settled
   more structure than any session before it and left the project
   one small answer away from a first buildable piece. **An item
   holds information and a task is an action** — Patrick's own
   realization, and the line SA-4's structure had been missing —
   with due dates recorded as boundaries to the actions rather
   than facts sitting inside an item. **A course is a tile**, its
   identifying title on top with the room numbers, days and times
   underneath and everything else behind it when it opens, and
   what is in the tile is what the app runs on: the calendar, the
   warnings, the notifications and the travel calculations are all
   derived from it. The session's largest change narrows SA-3's
   self-contained ruling, which had been this project's biggest
   structural decision: **the app pulls information in but never
   lets anything of hers out.** His own argument closed it — she
   signs in to the school's site and hands it her identifying
   information anyway, so the app takes what is already on her own
   device and never holds credentials, never makes a handshake and
   never meets anybody's IT department. What survives of the old
   reasoning is shape rather than permission, since whatever she
   hands across has a format the school can change. **It lives on
   both her devices, and the phone is the brain** — the laptop is
   for the convenience of typing and viewing, the phone holds the
   real copy and does all the working-out. He first proposed
   targeting the laptop and pulling the phone in later; the
   collision with SA-1, that the whole reason for a native build is
   local alarms and a reminder has to find her with the laptop shut
   in her bag, was put to him and he settled the division instead.
   Three roads to the Mac were read and the third taken: an iPhone
   app runs natively on an Apple Silicon Mac but in a phone-shaped
   window; a real Mac app is off Expo's supported path, desktop
   being expressly not a priority; and web is Expo's own third
   platform from the same codebase, giving a real laptop-sized
   layout on any Mac. Whether her Mac is Apple Silicon is unknown —
   Patrick said only that it is newer than his. AirDrop carries the
   data with nothing in the middle, and he demonstrated it
   mid-session by AirDropping the bus email from his phone to his
   Mac; sending is clean through `expo-sharing`, receiving is two
   taps because Apple deliberately changed iOS 17 so an AirDropped
   file lands in Downloads. **The bus question closed in writing.**
   The City of Lincoln replied by email that the public GTFS feeds
   can be used and there are no federal terms for app developers,
   contradicting the StarTran telephone call recorded at SA-1;
   Patrick's correction of the framing is the part to keep, that it
   is a confirmed viable option rather than merely an unlocked
   door. **"Where is my bus at right now?" is a feature** — his own
   rephrasing, which resolves the collision with his SA-2
   observation, since it is her question asked when she wants it
   and sits underneath the reminder rather than in place of it; and
   his one-sentence collapse of a Claude objection is worth
   keeping, that it only needs to fetch one particular thing at one
   particular time. **None of Memory's pages come across**, closing
   a question open since SA-2, though the look still does. The
   session also cured a commit complaint that turned out to be no
   fault at all: VS Code's Source Control panel had its
   Repositories list switched off, so it showed only the selected
   repository. Two things were found while looking — the
   `.gitignore` item carried since SA-1 was already done, and
   neither `Students-Assistant` nor the root `Projects` repository
   has a remote, so this project's history exists only on Patrick's
   Mac. He chose to publish after the refresh rather than before.
   The session opened badly and it is recorded in the project's
   build history: Claude's first sentence was false in the same way
   Y-47's was, four actions followed without asking, and Patrick
   said he was not sure he could trust the session. He refused the
   suggestion that he work around it, asked for slowing down, and
   the rest of the session held to short turns and gos asked for by
   name. Before it, SA-4 (2026-08-19) settled
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
   close. That question stopped blocking at SA-3, the app then
   taking nothing from outside itself, and it was answered
   outright at SA-5: the City of Lincoln replied in writing that
   the feeds can be used as described and that there are no
   federal terms or conditions for app developers. The telephone
   claim was wrong.
   `Projects/.gitignore` already carries `Students-Assistant/`, on
   line 20. That was verified at SA-5; the item had been carried as
   outstanding since SA-1 and was simply stale.
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
  rather than the other way about. Memory's own pending list really is
  `docs/pending.txt`, opened and read at #8-new, so the Y-22 doubt
  about it is closed.

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
