# Persona Multiplication (PMM)

Source: Pearl & Intriligator, *Persona Multiplication: A Method to Avoid Designed Injustice*.

## The problem it solves

When a team writes three or four personas, they nearly always describe the same person wearing different jobs. Age and occupation change; the body, the budget, the language, the bandwidth, and the household stay the same as the designers'. Everyone the product will fail is missing — and the team can't see who is missing, because the personas *look* varied.

## The method

Name the **dimensions** along which users actually vary first, then **multiply** along them, instead of inventing a handful of people.

## Precondition

**Ask for the product and any constraints before starting.** If the product is already clear from the conversation, confirm constraints in one line (market, geography, budget, regulatory context) and proceed.

## Procedure

1. **List 8–12 dimensions of real variation** for this product. Go past age and gender. Candidates:
   body size and strength · dexterity · vision and hearing · language and literacy · cognitive load and attention · money · time · housing · transport · care responsibilities · documentation status · digital access and data cost · trust in institutions · health conditions · shift work/schedule · neighborhood safety · social support · …and whatever else this product touches.
   Choose the dimensions the product is most sensitive to; say why each matters in a few words.
2. **For each dimension, name the two ends and the awkward middle** — not the average. The awkward middle is often the most neglected (e.g., "reads English well but not legal/medical English"; "has a smartphone but a prepaid plan that runs out mid-month").
3. **Generate 10–14 personas** by combining ends of *different* dimensions. Deliberately include combinations that are uncomfortable or inconvenient for the design.
4. **For each persona, exactly three lines:**
   - Who they are
   - What they need from this product
   - How the current design fails them
5. **Order:** put the uncomfortable personas first.
6. **Sort into three groups:**
   - **Designing to win for** (3): the ones the design must work for, and why
   - **Knowingly not serving**: who, and the concrete consequence for them (be honest — this is a design decision with ethical weight)
   - The rest: served adequately, or open questions
7. **The three we'd miss**: list the three personas the team would have missed entirely with four ordinary personas, and what each would have told us.

## PM Stage 2: complication matrix

Personas/groups across the top, scenarios down the side (default: hear about → find/obtain → set up → use → outcome). For each cell ask whether this group can do it and whether the design unfairly disadvantages or advantages them. Mark ✔ / ⚠ / ✘. Every ✘ is designed injustice to fix or declare. Audit the final set with `dotmet.md`.

## Output template

```
# Persona Multiplication: [Product] — [headline: who the current design fails most]

## Dimensions of variation
| # | Dimension | End A | Awkward middle | End B | Why it matters here |

## Personas (uncomfortable first)
**1. [Name/label]** — [dimension combo]
- Who: …
- Needs: …
- Current design fails them by: …
[…10–14 total]

## Sorting
**Designing to win for:** [3, with reason]
**Knowingly not serving:** [who → consequence]

## The three we'd have missed
[persona → what they would have told us]

## Verify with real people
[where to find each uncomfortable persona; cheapest method to reach them]

**Next method:** …
```

## Quality checks

- At least half the dimensions go beyond demographics.
- Every dimension has an awkward middle, not just two ends.
- At least 4 personas are genuinely inconvenient for the design.
- "Fails them by" names a specific design element, not a vague "may struggle."
- The "not serving" group names a real consequence (cost, exclusion, harm, workaround burden).
- Personas are respectful: specific circumstances, not stereotypes or caricatures.
