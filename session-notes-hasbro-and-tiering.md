# Session notes — Hasbro decision + tiering decision
*From a "business side" chat, 2026-07-11. Carry into the next MysteryCluesTracker coding session.*

## 1. Hasbro Spark submission — DECIDED: not pursuing

Explored submitting Mystery Tracker / a "Clue Tracker" concept to Spark Hasbro (spark.hasbro.com). Researched their actual terms and the market before deciding. Findings:

- **The deal is "hand over the idea," not "adopt the app."** Spark's Concept Disclosure Agreement treats a submission as a concept/information Hasbro can develop (or not) using their own team — not as a codebase they'd deploy as-is. A working prototype counts as proof-of-concept evidence, not a deliverable they commit to using.
- **Compensation is capped low and not guaranteed.** If Hasbro chooses to license the concept, the royalty is capped at 1.5% of net sales of the product/service using it, for up to 12 years — and that's only if they decide to license it at all. (This is a secondhand-quoted figure from a designer who read the agreement, not verified against the live document text, which loads via JS and couldn't be fetched directly.)
- **Hasbro already has an official Clue Companion app** (Marmalade Game Studio) — but it's a controller/notepad that pairs with the *digital* console/Steam edition of Clue via a 4-digit code, not a tracker for the physical board game. It's free, ~190–200K downloads, ~2.4–2.6★ rating, with review complaints about connection bugs.
- **Estimated Clue revenue** (soft, order-of-magnitude only — Hasbro doesn't break this out): ~3M units/year, likely $25–40M/year net sales worldwide. Not something to plan around.

**Decision:** Given the real engineering work already in Mystery Tracker (spec, flow diagram, 266-step test procedure, working app) versus Spark's "give us the idea, we decide what to do with it" structure and negligible realistic payout — not worth pursuing. Closed.

**Still worth doing regardless:** fix the stray Clue reference ("Plum, Rope and Hall", ~line 4032 of MysteryTracker.html) — already flagged in upgrade-scope.md's legal-caution section. To be handled in the regular code chat stream, not here.

## 2. Monetization interest — open, separate thread

Raised independently of Hasbro: interest in "a little extra income" from Mystery Tracker, since living on Social Security. Initial idea was a one-time price.

**Market research findings:**
- Comparable apps (board game score trackers, deduction/companion apps) are overwhelmingly **free-to-download with an optional premium/IAP unlock** — not one-time-paid upfront. Examples: Board Game Now, Cluso, the official Clue Companion itself.
- True one-time-paid niche companion apps were hard to find — most monetization in this space is free + $2.99–$4.99 "pro unlock."
- Realistic reach for a solo-built, non-branded tracker is small — likely well under the ~190–200K the *official, Hasbro-branded* Clue Companion managed.
- **Money mechanics** (Stripe for web vs. Apple IAP cut, tax implications) still marked "Not started" in Publishing-Strategy.docx — deliberately not gone into yet.

**No decision made yet** on pricing model. Next step when picked back up: decide free-plus-premium vs. something else, informed by the above.

**Visibility note (Patrick, #76):** while researching competitors, Patrick found these apps genuinely HARD TO FIND in the store — the whole category (deduction notepads / board-game companion trackers) has a discoverability problem: poor ranking on generic searches, no featuring, and the one app with real downloads (official Clue Companion) got them from the Hasbro brand, not findability. Implication for us, both directions: our app won't be found easily either, AND the store listing's name/keywords/screenshots are the highest-leverage marketing surface we have. Carry this into the Publishing-Strategy work when the listing is prepared. (Competitor addendum, same session: `Clue Solver: Detective Notepad` — the closest cousin, rebuilt 2026, entirely FREE including a full deduction engine, only 3 ratings — plus a cluster of Clue-notepad apps, none prominent. Confirms the small-market realism; differentiators we keep: generic player-named structure, works for variants, web+mobile pair.)

## 3. Tiering — DECIDED: bring it back into the current rebuild, now

- Ironic wrinkle surfaced: the original mobile app had tiering/premium logic built in. (Corrected #76: this line first said "web app" — wrong; the web app has no tiering, code-verified.) The new iOS rebuild (MysteryCluesTracker) explicitly **removed** it per the "NO-THINKING" directive in upgrade-scope.md (auto-Σ premium came out; per-turn auto-cross kept as plain bookkeeping).
- Rebuild is only ~2 days old — low sunk cost, good moment to fold this back in rather than bolt on later.
- **Decision:** do both — ship a free app either way, but put the tiering *hooks* back into this same clean rebuild now (using the Spec, the flow diagram, and the existing code as reference), rather than treating it as a separate future project. A full clean rebuild from those three sources was already a long-term goal; now's the time to incorporate it.

**Next step:** this needs to be scoped and built in the actual coding session where the MysteryCluesTracker project/repo is connected — not in this chat. Per standing rules: one step at a time, discuss before building, wait for Patrick's explicit "go."
