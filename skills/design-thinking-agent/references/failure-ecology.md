# Failure Ecology

Ask this early; it changes what you design.

## Procedure

1. **List 25 ways the product fails in the real world** — not in a lab. Cover the full ecology:
   - Misuse (used wrong, used for something else)
   - Disuse (bought, never used)
   - Abandonment (used, then quit — and when)
   - Discomfort (physical, sensory, emotional)
   - Embarrassment (social visibility, stigma)
   - Cost (price, running costs, hidden costs)
   - Theft, loss, damage
   - Repair friction (no parts, no one to fix it, voided warranty)
   - **Failures that show up only after months of use** (wear, drift, habit decay, data rot, changing life circumstances)
   - Plus: failures for edge users, environmental failures, failures in handoff between people
2. **Group into 5–7 families.** Name each family.
3. **For each family:**
   - The design lever that would reduce it
   - What that lever would cost us elsewhere (money, complexity, weight, another user's experience, aesthetics, time to market)
4. **Name the failure a user would never report** to us, and why (shame, blame, didn't notice, thought it was their fault, no channel, already abandoned).

## Output template

```
# Failure Ecology: [Product] — [headline: the family that matters most]

## 25 real-world failures
1. … (tag: misuse / disuse / abandonment / …)
[…25]

## Families
| Family | Failures (#s) | Design lever | What the lever costs elsewhere |

## The failure no one would report
[Failure] — why it stays hidden, and how we could detect it anyway (telemetry, returns data, observation, proxy interviews)

## Verify with real people
…
```

## Quality checks

- Exactly 25, specific enough to picture ("strap chafes after 3 hours in summer", not "uncomfortable").
- At least 4 are long-horizon (months of use).
- Every lever has a real trade-off; "no downside" is a red flag.
- The unreported failure comes with a detection idea.
