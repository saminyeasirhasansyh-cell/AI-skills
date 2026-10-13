# SUN Analysis — Stakeholders, Users, Needs

## Contents
1. Purpose
2. Inputs and preconditions
3. Procedure (5 phases)
4. Stakeholder vs. user: how to tell them apart
5. Output template
6. Quality checks
7. Common failure modes

---

## 1. Purpose

SUN produces a ranked map of everyone who touches, pays for, approves, maintains, or is affected by a system, what each of them needs, and which of them the team must interview first. It is the backbone deliverable of early design research: the persona deck, the interview guide, and the feature priorities all descend from it.

SUN uses two lenses throughout: **CLIMBER** (FLATS for each person, RAMPS for their context — see `climber.md`) and **MTA/TTA** (task breakdown across many dimensions and across actors — see `mta-tta.md`). Read both before running a full SUN.

## 2. Inputs and preconditions

Required: a project description detailed enough to know what the system is and roughly who it serves. If absent, ask for a detailed description and stop.

Helpful: client brief, stage, constraints, geography, known competitors, prior research. If missing, state assumptions in a line and proceed.

If the project is very early (no concept, no clear customer), recommend running CLIMBER C+L first (under 500 words) and offer the full SUN as the next step.

## 3. Procedure

### Phase 1 — Explore and enrich the project space

Do this thoroughly *before* summarizing. The goal is to discover stakeholders and needs that aren't in the brief.

- **Restate the goal** in one sentence, then list the implicit goals behind it (financial, reputational, regulatory, mission).
- **Analogous projects**: name 3–5 related products, services, or programs (including from other industries) and what each teaches about who matters and what goes wrong. If web search is available, use real examples and cite them.
- **Brainstorm actors widely**: list every human, organization, machine, tool, and subsystem that interacts with the system across its lifecycle — design, procurement, installation, onboarding, daily use, maintenance, failure, repair, disposal. Include the people affected by the system who never use it.
- **Cluster** the actors into 4–7 groups (e.g., payers, operators, end users, maintainers, regulators, affected bystanders).
- **Enrich**: for each cluster, ask what would make them block, champion, or quietly abandon the system.
- **Summarize** in 3–5 sentences: what the project is, its goals, and its core challenges. This summary opens the output.

### Phase 2 — Identify key stakeholders

Stakeholders influence, fund, approve, operate around, or are affected by the system, but are not the primary hands-on users. For each (aim for 5–8):

| Field | What to capture |
|---|---|
| Role | Position and relationship to the system |
| Goals | What success looks like to them (incl. incentives and metrics they're judged on) |
| Main tasks | Key activities and responsibilities that touch the system |
| Pain points | Current frustrations, risks, costs |
| Dream features | What they'd ask for if anything were possible |
| Issues to explore | Open questions, conflicts, unknowns to verify |
| FLATS snapshot | One line each for Fears, Loves, Aspirations, Traits, Skills that matter here |
| Influence / interest | High/Med/Low on each — used for ranking |

**Rank** by importance to project success. Give one line of reasoning per rank. A common useful tiebreaker: who can kill the project, and who has to live with it longest.

### Phase 3 — Identify key users/customers

Users interact with the system directly, or are the primary beneficiaries/consumers. Include primary and secondary customers (the dog eats the food; the owner buys it). For each (aim for 4–7):

| Field | What to capture |
|---|---|
| Role | Who they are, in a concrete moment of use |
| Goals | What they hope to achieve with the system |
| Tasks | Step-by-step interaction with the system (use MTA) |
| Pain points | Where current solutions fail them |
| Dream features | Ideal capabilities |
| Issues | Unknowns, edge cases, conflicts with other users |
| Interaction description | 2–3 sentences: when, where, how often, with what, under what constraints |
| FLATS + RAMPS snapshot | Key fears, aspirations, relationships, activities |

**Rank** by importance. Prefer frequency × consequence: who uses it most, and whose failure costs the most.

Include at least one **edge user** (low literacy, disability, low bandwidth, non-native language, high stress, first-time user) — or run Persona Multiplication (`persona-multiplication.md`) as the follow-up.

### Phase 4 — Apply MTA and TTA

For the top 2–3 users, run a compact MTA on their core task across at least these dimensions: physical, cognitive, emotional, decisional, informational, attentional — plus any of material, sustainability, profitability, risk, complexity, investment that matter here. Present as a table (task steps × dimensions), flagging the hot spots.

If multiple actors (people, machines, software, organizations) hand work to each other, run TTA: map the handoffs, who holds what information at each point, and where coordination breaks. See `mta-tta.md`.

### Phase 5 — Synthesis and recommendations

- **Top 5–7 areas for exploration**, ranked. Each: a headline insight (a claim, not a topic), 2 sentences of reasoning, and the evidence that would confirm or kill it.
- **3–5 priority interviewees** (stakeholders or users). For each: why they matter now, and 3–4 **interview themes** designed to reveal constraints and opportunities. Themes should be open, behavior-focused ("walk me through the last time…") rather than feature-focused ("would you like X?").
- **How might we** statements: 3–5, derived from the top areas.

### Phase 6 — Matrix and visualization

Build at least one matrix:

- **Persona × needs × features**: rows are stakeholders/users, columns are needs or candidate features, cells mark importance (●●● / ●● / ● / —) or conflict (⚠).
- Optionally, a **power/interest grid** (influence vs. interest quadrants) and a **dependency map** showing which personas depend on which features or on each other.

Call out conflicts explicitly: where one persona's dream feature is another's pain point.

## 4. Stakeholder vs. user: how to tell them apart

- Touches the system directly and regularly → **user**
- Pays, approves, regulates, maintains, or is affected without direct use → **stakeholder**
- Some people are both (e.g., a clinic manager who also uses the dashboard). List them where their primary influence sits and note the dual role.

## 5. Output template

```
# SUN: [Project] — [one-line headline finding]

**Bottom line:** [2–3 sentences: the most important insight, the persona who matters most, the first interview to run]

## Project in brief
[3–5 sentence summary: goal, context, core challenges]

## Enrichment highlights
[Analogous projects and what they teach; clustered actor map]

## Stakeholders (ranked)
[Ranked table: rank, stakeholder, influence/interest, why ranked here]
[Per-stakeholder detail blocks]

## Users/customers (ranked)
[Ranked table + per-user detail blocks]

## Task analysis (MTA / TTA)
[MTA table for top users; TTA handoff map if multi-actor]

## Top areas for exploration
[5–7 ranked insight headlines with reasoning and evidence needed]

## Who to interview first
[3–5 people, why, and interview themes]

## How might we…
[3–5 HMW statements]

## Persona × needs × features matrix
[Table; conflicts flagged]

## Verify with real people
[3–5 hypotheses, with whom, cheapest method]

**Next method:** [e.g., Persona Multiplication to find who this map is missing]
```

## 6. Quality checks

Before sending, check:

- Does the ranking have reasons, and would a client agree with the top 2?
- Is there at least one stakeholder the brief didn't mention?
- Is there at least one edge user?
- Are the "areas for exploration" claims rather than topics?
- Are interview themes behavioral and open, not leading?
- Is every unverified claim marked as a hypothesis?
- Does the matrix show at least one conflict? (If none, look harder — real systems have them.)

## 7. Common failure modes

- **Everyone ranks equally** — forces the user to do the prioritization.
- **Users are job titles, not moments** — "teacher" instead of "substitute teacher with no login on day one."
- **Dream features are just the product brief restated.**
- **Missing the maintainers, the disposers, and the bystanders.**
- **Invented statistics.** If you cite a number, source it or mark it as an estimate to verify.
