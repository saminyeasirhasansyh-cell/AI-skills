# MTA and TTA — Multidimensional and Teamwork Task Analysis

## Purpose

Traditional task analysis looks at physical steps (what the hands do) or cognitive steps (what the mind does). **MTA** runs the same step-by-step breakdown across many more dimensions, so hidden burdens (emotional strain, attention overload, cost, risk) become visible. **TTA** extends it to systems with multiple actors — people, robots, machines, software, organizations — and focuses on the handoffs between them.

## MTA procedure

1. **Pick the core task** for a specific user in a specific moment ("night-shift nurse administering a 2 a.m. med dose").
2. **Break it into 5–10 steps**, from trigger to completion (include setup, recovery from error, and cleanup).
3. **Pick dimensions**: always the core six, plus any extended ones relevant to the project.
4. **Fill the grid**: for each step × dimension, note the demand or burden in a few words. Mark hot spots (high burden, high risk) with ⚠.
5. **Read across rows** (which steps are hardest overall?) and **down columns** (which dimension is the hidden burden?).
6. **Derive design implications**: for each hot spot, one design lever.

### Core dimensions

| Dimension | Question |
|---|---|
| Physical | Movement, force, posture, dexterity, reach, fatigue, environment (light, noise, temperature) |
| Cognitive | Memory load, calculation, comprehension, learning, mental models |
| Emotional | Stress, fear, embarrassment, frustration, pride, trust |
| Decisional | Choices made, uncertainty, stakes, reversibility, who is accountable |
| Informational | What info is needed, where it comes from, its quality and timeliness, what's missing |
| Attentional | Competing demands, interruptions, vigilance, multitasking, alerts |

### Extended dimensions (use those that fit)

Material · Sustainability · Profitability · Risk (safety, legal, financial) · Complexity · Investment (time, money, training) · Social (who's watching, norms) · Temporal (time pressure, frequency, timing) · Spatial · Regulatory · Ethical/equity · Maintenance · Accessibility

### MTA output template

```
Task: [user] doing [task] in [context]

| Step | Physical | Cognitive | Emotional | Decisional | Informational | Attentional | [Extended…] |
|---|---|---|---|---|---|---|---|
| 1. … | | | | | | | |
| 2. … | ⚠ … | | | | | | |

Hottest steps: …
Hidden burden (dimension): …
Design implications: [hot spot → lever]
```

## TTA procedure

Use when two or more actors interact with or through the system.

1. **List the actors**: humans (by role), machines, software/subsystems, organizations.
2. **Map the workflow** as a sequence of handoffs: who does what, then passes what to whom.
3. **For each handoff**, capture:
   - What is transferred (object, information, authority, responsibility)
   - Channel (verbal, written, system, physical)
   - Shared awareness: what does each side know / not know at that point?
   - Timing and synchronization needs
   - Failure mode: what gets lost, delayed, misunderstood, or duplicated?
   - Accountability: who owns the outcome if it fails here?
4. **Identify coordination breakpoints**: handoffs with high failure probability × high consequence.
5. **Derive design levers**: shared displays, confirmations, checklists, automation of transfer, role clarity.

### TTA output template

```
Actors: [A, B, C…]

| # | From → To | What's handed off | Channel | Shared awareness gap | Failure mode | Owner |
|---|---|---|---|---|---|---|

Coordination breakpoints (ranked): …
Design levers: …
```

## Quality checks

- Steps include error recovery and cleanup, not just the happy path.
- At least one non-obvious dimension (emotional, attentional, risk) has a hot spot.
- TTA includes non-human actors where they exist.
- Every hot spot maps to a design implication.
