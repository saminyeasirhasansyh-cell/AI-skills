# Tooling landscape for consulting-grade decks

Loaded by `SKILL.md` when the user is choosing between (or asking about) template libraries,
PowerPoint add-ins, AI slide generators, or generic template marketplaces for a specific deck. Use
this to give scenario-specific tool guidance rather than a generic "it depends."

## The five categories

### 1. Libraries of real cases and technique guides
What they are: collections of actual past consulting decks (or close approximations) plus
written guides on the underlying techniques (action titles, SCR, storylining).

- **Strength.** Written guides explain the *why* behind a technique in detail; real-deck libraries
  are often the fastest way to internalize a standard, because seeing a real worked example teaches
  pattern recognition faster than a description of the pattern.
- **Limitation.** Genuine client-engagement decks are scarce publicly — most of what circulates is
  dated, or is a promotional/marketing deck rather than an actual internal analytical deliverable,
  which understates how dense and data-heavy real client work is.
- **Best for:** learning the standard itself, or finding a sequencing precedent for an unfamiliar
  deck type before drafting.

### 2. Consulting-grade strategy/case templates
What they are: a complete deck skeleton — storyline, slide layouts, and (in the better products)
full worked examples — built specifically to the MBB standard, as opposed to a blank layout pack.

- **Strength.** The storyline and standard come pre-built, so the job becomes adapting a proven
  structure rather than inventing one from nothing — this is the fastest route to a deck that is
  structurally sound on day one.
- **Limitation.** A template does not do the thinking for you. It supplies structure, not the
  strategic choices, the specific data, or the judgment calls the deck actually needs to be right
  for this situation — those still have to come from the person (or from the human-owned steps in
  §7 of SKILL.md).
- **Best for:** board/leadership strategy decks, a first strategy deck for someone new to the
  format, 100-day plans for incoming leadership, or any deck where getting the deck-level structure
  right matters as much as the individual slides.

### 3. PowerPoint add-ins (charting/formatting tools)
What they are: in-app tools that automate chart-building (waterfalls, automatic CAGR lines, etc.)
and deck-wide formatting sweeps.

- **Strength.** Large speed gains on the mechanical, repetitive parts of slide production —
  especially useful on a deck with many charts (market sizings, roadmaps) or when reformatting an
  existing deck to new branding.
- **Limitation.** An add-in has no opinion about deck quality — it makes a well-structured deck
  faster to build *and* makes a badly structured deck faster to build. It supplies zero storyline,
  zero strategic structure, and zero worked examples; it is purely a production accelerant layered
  on top of a storyline that has to already be right.
- **Best for:** a deck where the structure is already locked and the remaining work is producing a
  large number of charts, or a pure reformatting/rebranding pass on an existing deck.

### 4. AI presentation generators
What they are: tools that produce a visual draft deck from a short text prompt (or an uploaded data
set) in minutes.

- **Strength.** Genuinely fast first visual drafts, and reasonable for low-stakes internal updates
  where polish matters less than speed.
- **Limitation, in detail:** for a genuine strategy/consulting deck specifically, these tools tend
  toward generic, "sales-y" output; hallucinate numbers with enough confidence that fact-checking
  becomes a real time cost; lack the messaging discipline and visual balance that come from an
  actual review cycle; and — most importantly — cannot make the hard strategic trade-offs a real
  deck requires, because that judgment isn't something a single prompt can supply. A deck generated
  this way tends to look finished at first glance and fall apart on closer inspection (the "70%
  version that takes more time to fix than to build correctly" problem).
- **Best for:** fast first-draft scaffolding at the slide-stub stage (see step 3 of the 6-step
  process in SKILL.md §7), low-stakes internal drafts, or promotional/externally-facing decks where
  the bar is different from an internal analytical deliverable — paired with strict human fact-
  checking and visual control in every case.

### 5. Generic template marketplaces
What they are: broad marketplaces of visually polished, inexpensive, strategy-themed slide
templates not built by consultants.

- **Strength.** Low cost (often free) and wide visual variety — useful for graphic inspiration on
  how a concept could be represented visually.
- **Limitation.** Measured against the consulting standard, these are decorative rather than
  structural — e.g., a slide titled "Our Strategy" with five colorful pillar icons but no storyline
  connecting aspiration → choices → initiatives → KPIs. They were designed by graphic designers for
  visual appeal, not by consultants for argument structure, so they lack the depth and slide
  discipline this skill is built around.
- **Best for:** visual/graphic inspiration only — never as the actual slide content or structure for
  a genuine consulting-grade deliverable.

## Matching category to scenario

| Scenario | Best-fit category |
|---|---|
| Annual or 3–5 year strategy deck for the board | Consulting-grade template (category 2) |
| First strategy deck for someone new to the format | Consulting-grade template + real deck examples (categories 1 + 2) |
| 100-day plan for incoming leadership | Consulting-grade template with a leadership-transition variant |
| Deck structure is already locked; many charts to build | Charting/formatting add-in (category 3) |
| Quick internal strategy update, low stakes | AI generator, fed the prior deck plus new data, action titles rewritten by a human afterward |
| Reformatting an existing deck to new branding | Add-in formatting sweep (category 3) |
| Strategy offsite pre-read | Consulting-grade template, condensed storyline |
| Weekly deck production across many concurrent projects | Template library combined with a charting add-in |
| Condensed overview deck for internal/external promotional use | AI generator, with strict fact-checking and visual control applied afterward |

## The general recommendation across categories

For most recurring strategy/consulting work, the most effective setup combines: a consulting-grade
template for deck-level structure, one charting/formatting add-in for slide-level production speed,
and an LLM used specifically for storyline sparring (per the 6-step process in SKILL.md §7) — not
for single-prompt deck generation. Feed the LLM real past-case material and the technique guidance
in this skill rather than asking it to generate from a bare topic prompt; the quality of what it
returns is bounded by the quality and specificity of what it's given.

Regardless of which combination is used: sanity-check everything before it ships. Does each slide
make sense on its own? Does the data check out against a real source? Does the deck read as
balanced when flipped through top to bottom?
