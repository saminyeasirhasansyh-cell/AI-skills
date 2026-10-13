# CLIMBER — Intriligator's Model of Design Thinking

## Contents
1. Overview and modes
2. C — Customer (FLATS)
3. L — Life (RAMPS)
4. I — Insight (BASE)
5. M — Mechanism (GEAR)
6. B — Build (PATH)
7. E — Evaluate (SCAN)
8. R — Refine (SPIN)
9. Output templates
10. Extensions and implications

---

## 1. Overview and modes

CLIMBER has seven phases, each with a sub-acronym. It is iterative and layered, not linear: insights send you back to Customer; evaluation sends you back to Mechanism.

| Phase | Sub-steps | Core question |
|---|---|---|
| **C**ustomer | FLATS: Fears, Loves, Aspirations, Traits, Skills | Who exactly is this for? |
| **L**ife | RAMPS: Relationships, Activities, Mappings, Problems, Stakeholders | What is their world like? |
| **I**nsight | BASE: Brainstorm, Analyze, Synthesize, Ecosystem | How might we make their life better? |
| **M**echanism | GEAR: Generate, Evaluate, Align, Refine | What way(s) could realize the insight? |
| **B**uild | PATH: Prototype, Assess, Tweak, Hone | How do we make it real? |
| **E**valuate | SCAN: Scrutinize, Confirm, Adjust, Navigate | Does it work for real people? |
| **R**efine | SPIN: Scrutinize, Pivot, Integrate, Nurture | How does it keep getting better? |

Note: the original CLIMBER text uses "FLAT" (four items); the SUN prompt extends it to "FLATS" by adding Skills. Use FLATS.

### Modes

- **Early-stage mode (C + L only):** if the project is very early (no concept, fuzzy customer), run only Customer and Life, in **under 500 words**. End by naming the 2–3 most promising insight directions for the next round.
- **Full mode:** all seven phases. Use when a customer and context are established, or when the user asks for the full model.
- **Single-phase mode:** the user can ask for any one phase ("run GEAR on these insights").

If the product or customer isn't clear, ask. When you can, first offer candidate customers — including secondary customers (the parent who buys the toy, the owner who buys the dog food, the IT admin who approves the app).

## 2. C — Customer (FLATS)

Build a foundational understanding of one specific customer. "Customer" can be a user, stakeholder, proto-customer, or secondary customer. Pick one and be concrete; run multiple customers as separate FLATS blocks.

| Sub-step | Probe questions |
|---|---|
| **Fears** | What are they afraid of losing, looking foolish about, getting wrong, being blamed for? What keeps them up at night in this domain? |
| **Loves** | What do they enjoy, take pride in, protect? What current tools/rituals do they love and won't give up? |
| **Aspirations** | Who are they trying to become? What would a great year look like? What status, freedom, or mastery do they want? |
| **Traits** | Stable characteristics that shape behavior: risk tolerance, tech comfort, patience, trust, routine vs. novelty |
| **Skills** | What they're already good at (and what they're not) — what the design can lean on vs. must compensate for |

Tip: fears and aspirations usually drive adoption more than features do. Make them specific and emotional, not generic ("fears wasting money" → "fears her manager seeing she approved a tool nobody uses").

## 3. L — Life (RAMPS)

Contextualize the customer in their environment.

| Sub-step | Probe questions |
|---|---|
| **Relationships** | Who do they depend on, answer to, care for, compete with? Who influences their decisions? |
| **Activities** | What does a typical day/week/cycle look like? Where does the problem show up in that routine? |
| **Mappings** | Journey maps, process maps, mental models: how do they think the system works? What's their step-by-step path through the problem today? (See example journey maps: https://www.smaply.com/blog/example-journey-maps) |
| **Problems** | Where does it hurt — friction, cost, delay, risk, embarrassment? Which problems are tolerated, and why? |
| **Stakeholders** | Who else has a say or a stake in their life around this problem? (Feeds SUN.) |

## 4. I — Insight (BASE)

Generate hypotheses about how to make this customer, living this life, happier, safer, better off, more free — increase the good, decrease the bad.

| Sub-step | Do |
|---|---|
| **Brainstorm** | Generate many possible opportunity areas, including wild ones |
| **Analyze** | Test each against FLATS and RAMPS: which address real fears/problems? |
| **Synthesize** | Cluster into themes; write the strongest as **"How might we…?"** statements |
| **Ecosystem** | Market research, competitor research, literature review. What exists? What failed and why? Where is the white space? Use web search where available, and cite it. |

Output: 5–8 HMW statements, ranked, each with a one-line rationale tied to a specific fear, problem, or aspiration.

Good HMW: specific customer + specific moment + specific outcome ("How might we help a first-time caregiver know within 10 seconds whether a missed dose is dangerous?"). Bad HMW: "How might we improve healthcare?"

## 5. M — Mechanism (GEAR)

Develop the way(s) to realize the insight.

| Sub-step | Do |
|---|---|
| **Generate** | 3–6 distinct mechanisms per top insight: product, service, policy, business model, behavioral nudge, partnership |
| **Evaluate** | Score against desirability, feasibility, viability, and equity (who it excludes) |
| **Align** | Check each mechanism against the insight and FLATS — does it actually address the fear/aspiration? Against stakeholder incentives? |
| **Refine** | Combine, simplify, sharpen the top 1–2 |

Consider running constraint collision (`constraint-collision.md`) here.

## 6. B — Build (PATH)

Bring the mechanism to life. Either do it (mock up, write the service blueprint, draft the script) or describe in detail how to build it.

| Sub-step | Do |
|---|---|
| **Prototype** | Choose the right fidelity: paper, Wizard-of-Oz, storyboard, role-play, clickable mock, looks-like/works-like model. Say what question each prototype answers. |
| **Assess** | Define what "working" means before testing — the riskiest assumption this prototype tests |
| **Tweak** | Plan quick iterations: what you'll change based on likely results |
| **Hone** | Converge on the version worth investing in |

## 7. E — Evaluate (SCAN)

In real life, show the prototype to users. As an LLM, describe precisely how you would evaluate it.

| Sub-step | Do |
|---|---|
| **Scrutinize** | Test plan: who (recruit criteria incl. edge users), how many, what tasks, what setting |
| **Confirm** | Success metrics and thresholds — task completion, time, errors, emotional response, willingness to pay/adopt |
| **Adjust** | Decision rules: what result triggers which change |
| **Navigate** | Next steps and go/no-go criteria for the next fidelity level |

## 8. R — Refine (SPIN)

Continuously refine and adapt.

| Sub-step | Do |
|---|---|
| **Scrutinize** | What did evaluation reveal? What surprised you? |
| **Pivot** | What must change fundamentally — customer, insight, or mechanism? |
| **Integrate** | Fold learnings into the design, the stakeholder map, and the business case |
| **Nurture** | Post-launch: feedback loops, community, maintenance, measures of long-term success |

## 9. Output templates

### Early-stage (C + L), under 500 words
```
# CLIMBER C+L: [Customer] — [headline insight]

**Customer:** [one concrete sentence]
**Fears:** … **Loves:** … **Aspirations:** … **Traits:** … **Skills:** …
**Relationships:** … **Activities:** … **Mappings:** … **Problems:** … **Stakeholders:** …

**Most promising directions:** [2–3 insight hypotheses]
**Verify with real people:** [3 items]
```

### Full CLIMBER
One section per phase, each with the sub-step table filled in, headed by an insight-bearing title. Open with a bottom-line summary; close with "Verify with real people" and "Next method."

## 10. Extensions and implications

- **Multiple customers:** run FLATS separately for primary and secondary customers; the gap between them (kid wants fun, parent wants safety) is often the insight.
- **CLIMBER is recursive:** a Mechanism has its own customers (the installer, the maintainer). Re-run C+L on them.
- **Pair with PMM:** FLATS describes one person deeply; Persona Multiplication checks you picked the right person.
- **Pair with failure ecology in Evaluate:** what users won't report is invisible to a standard SCAN.
