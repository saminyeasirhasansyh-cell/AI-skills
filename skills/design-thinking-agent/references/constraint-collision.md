# Constraint Collision

Use to kill concepts before a client does it for you.

## Input

3–5 candidate concepts. If the user hasn't listed them, ask. If concepts are vague, restate each in one sentence and confirm.

## Procedure

1. **Collide each concept with these constraints** (add project-specific ones if relevant):
   - Certification or regulation
   - Manufacturing
   - Unit cost
   - Weight or size
   - Cleaning and maintenance
   - Repairability
   - Accessibility
   - Supply chain
   - **The client's own capacity to maintain it after we leave**
2. **Score each collision:** Survives / Wounded / Dead, with **one line of reasoning**.
3. **Recommend one hero concept and one wildcard.** The hero is the best bet; the wildcard is the high-upside option worth keeping alive.
4. **State what evidence would change your mind** about the recommendation.

A single "Dead" on a hard constraint (regulation, client capacity) usually disqualifies a concept unless a design change clearly resolves it — say so.

## Output template

```
# Constraint Collision — Hero: [concept]; Wildcard: [concept]

| Constraint | Concept A | Concept B | Concept C |
|---|---|---|---|
| Certification/regulation | 🟢 Survives — … | 🟡 Wounded — … | 🔴 Dead — … |
| Manufacturing | | | |
| Unit cost | | | |
| Weight/size | | | |
| Cleaning/maintenance | | | |
| Repairability | | | |
| Accessibility | | | |
| Supply chain | | | |
| Client capacity post-handoff | | | |
| **Tally** | x S / y W / z D | | |

**Hero:** [concept] — why
**Wildcard:** [concept] — why keep it alive
**What would change my mind:** [specific evidence]
**Fixes for wounded collisions on the hero:** …
```

## Quality checks

- Every cell has a reason, not just a score.
- "Client capacity" is taken seriously (staff, budget, skills, spare parts after handoff).
- Evidence that would change the recommendation is specific and obtainable.
