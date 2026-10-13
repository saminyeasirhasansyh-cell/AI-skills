---
name: partha-brain-strategy-presentation
description: Consolidated consulting-craft skill set — covers (1) MBB/McKinsey cover letters, (2) consulting-style strategy decks and presentation storylines (SCR, strategy house, action titles, avoiding the "AI-generated" look), (3) Partha Ghosh & Katrina Pugh's 15 management-consulting analytical tools (Five Forces, Pareto, gap analysis, Monte Carlo, etc.), and (4) professional/academic writing (memos, reports, executive summaries, BLUF structure). Use this any time the task is a cover letter, a strategy/business deck, a named analytical tool ("do a Pareto analysis," "map the five forces"), or a memo/report/executive summary — even if the user doesn't name the framework, just says "make this McKinsey-level," "make this board-ready," "make this not look AI-generated," or "tighten this writing." Always route to the relevant reference file below and apply its rules rather than improvising generic advice.
---

# Partha's Brain — Strategy & Presentation

One consolidated skill covering the consulting-craft toolkit: how to argue (analytics), how to
write it up (professional writing, cover letters), and how to present it (deck storyline). Each
domain lives in its own reference file — **read the one that matches the task before producing
output**; don't try to hold all of them in working memory at once.

## Shared spine — applies across every domain below

Every one of these sub-skills is a variation on the same McKinsey-style discipline. Hold this
regardless of which reference file you're using:

1. **Answer first, evidence second (BLUF).** State the conclusion/recommendation before the
   supporting detail — in a cover letter's opening, a slide's action title, an executive summary,
   or a memo's first paragraph. Never bury the point in the middle.
2. **Every claim needs a receipt.** A quality, a conclusion, or a recommendation asserted without a
   specific, quantified example or source is a claim not yet earned — flag the gap and ask for the
   missing data/example rather than papering over it with generic language.
3. **Insight-bearing, not descriptive, headers/titles.** "Costs grew 10%/year, double revenue
   growth" beats "Historical Cost and Revenue Trends" — this rule applies to slide titles, section
   headings, and analytic tool write-ups alike.
4. **Structure before content.** Sketch the argument/outline/storyline before drafting prose or
   building slides. Don't let "generate the whole thing" collapse structuring and drafting into one
   step — that's where genericness and hallucination creep in.
5. **Subtractive editing.** Cut anything that doesn't serve the stated conclusion. Move cut-but-
   maybe-useful material to an appendix rather than deleting it outright.

## Routing table — which reference file to load

| Task looks like... | Load |
|---|---|
| A McKinsey/BCG/Bain application cover letter; "why consulting" paragraph; critiquing/scoring a cover letter draft | `references/cover-letters.md` |
| A strategy deck, business case, or consulting-style presentation; deck storyline/SCR/strategy house; action titles; executive summary slide; recommendation slides; "make this board-ready" or "this looks AI-generated" | `references/presentations.md` (its own sub-reference `references/presentation-assets/ai-tooling-landscape.md` covers tool/template comparisons — load only if asked about tool choice) |
| A named analytical tool (Five Forces, value chain, trend analysis, gap analysis, system dynamics, Pareto, leading/lagging indicators, trade-offs/equilibrium, portfolio mapping, root-cause/fishbone, regression, elasticity/sensitivity, clustering, decision trees, Monte Carlo) or "which framework fits this problem" | `references/analytics-tools.md` |
| A memo, email, report, academic paper, or executive summary; making writing "more professional," "concise," or "executive-ready"; framing/prioritizing/synthesizing an argument before writing | `references/professional-writing.md` |

Several of these commonly chain together in one task — e.g., run an analytics tool
(`analytics-tools.md`) → write up the finding in memo form (`professional-writing.md`) → turn it
into deck slides (`presentations.md`). Load each reference file as you reach that stage of the
work; don't try to pre-load all of them for a single-domain request.

## Cross-domain conventions worth carrying everywhere

- **The analytics write-up convention** (What is it? / When to use it? / What data is needed? /
  What's a typical conclusion?, then the analysis, then a bolded plain-language "so-what") from
  `analytics-tools.md` is the same underlying discipline as an action title in `presentations.md`
  and a topic sentence in `professional-writing.md` — all three are "state the insight before the
  evidence," just at different units of granularity (tool write-up / slide / paragraph).
- **The mistake-checklist habit.** Every reference file ends with (or should be read alongside) a
  concrete checklist to run the draft through before calling it done — cover letter mistakes,
  slide/deck self-checks, doc review checklist, writing self-editing passes. Always run the
  relevant checklist explicitly rather than eyeballing "does this look done."
- **Don't cross-apply firm/audience-specific rules.** McKinsey/BCG/Bain differ in cover-letter
  purpose and length (see `cover-letters.md` §2); an academic reader expects scholarly sourcing
  that a business memo doesn't (see `professional-writing.md`). Check which audience/firm applies
  before reusing rules from one context in another.
