# Partha's Analytics — Strategy Analytics (15 Tools)

Source: Partha S. Ghosh & Katrina Pugh, "Introduction to Management Consulting: Art & Science of
Problem Solving — Fifteen Analytical Tools" (TGI 193/15). Use this skill whenever a task calls for
picking, applying, or presenting one or more of these 15 analytics.

## Core idea

Every analytic tool is really a choice of **cause (X-axis) and effect (Y-axis)** applied to a
**scope**: the ecosystem (industry/environment), the focal point (what to prioritize), or the
decision (what choice to make). Before reaching for a tool, ask:

1. What stage of the MC project framework am I in? (Naming Purpose/Scoping → Data
   Collection/Analysis → Findings Interpretation → Strategy/Solution Design → Implementation →
   Measurement/Continuous Improvement)
2. Which of the three scales does the question live at?
   - **Forces at Work (#1–5)** — understand the dynamics of an industry/ecosystem
   - **Focal Points (#6–10)** — narrow down and prioritize what to focus on
   - **Decisions (#11–15)** — structure a choice or make a smart decision
3. What are my cause (X) and effect (Y) variables, and what insight am I actually chasing?

Combine multiple tools rather than picking just one — that's the intended use. It's fine to invent
a new analytic if none of these fit, but check this list first.

## How to apply a tool

For every tool below: state **What it is**, **When to use it**, **What data is needed**, and
**What a typical conclusion looks like** — then show the analysis itself (chart/table/diagram) and
close with an insight-bearing, plain-language takeaway sentence (this deck's own convention: a bolded
italic "quote" summarizing the so-what). This mirrors Samin's preferred McKinsey-style structure —
answer first, evidence second, insight-bearing titles.

---

## Forces at Work — understand ecosystem dynamics (#1–5)

**1. Forces at Work.** What: identify and measure the relative impact of factors influencing an
industry/domain (regulatory changes, geopolitical/geoeconomic shifts, technology substitutes,
supplier-driven forces, competitors, changing ecosystems in adjacent industries). When: isolating
factors by magnitude, velocity, or risk before diving deeper. Data: economic, industry-trade, and
performance data. Typical conclusion: scope/focus on a segment or product to capture "white space."
Common variant: **Porter's Five Forces** (rivalry, threat of entrants, buyer power, supplier power,
threat of substitutes) — use the determinant checklists (concentration, switching costs, brand
importance, barriers to entry/exit, etc.) to structure the questions for each force.

**2. Flow / Value Chain Analysis.** What: understand how value is added or subtracted across a flow
of tasks (primary activities: inbound logistics → operations → outbound logistics → marketing/sales →
service; support activities: infrastructure, HR, technology, procurement). When: finding relative
gaps, strengths, or interdependencies among components of a firm, or comparing cost structure
customer-by-customer or vs. competitors. Data: internal/external budget, staffing, materials
(annual reports, supplier data). Typical conclusion: find differentiation/leverage points between
client and ecosystem (e.g., align investment with what each customer segment actually values).

**3. Trend Analysis.** What: understand inter-temporal changes in outcomes and their likely drivers.
When: a technology or market may follow a recognizable pattern (S-curve, hockey stick, boom-bust,
Moore's Law). Data: buyer demand, stock price, system performance, tariff impacts — any time series.
Typical conclusion: scope further study based on analogous systems; distinguish substitution effects
from genuine demand growth.

**4. Comparative / Gap Analysis.** What: compare performance to a baseline, competitor, or business
unit to isolate causes of performance differences. When: fierce competition, contested positioning,
or price sensitivity is affecting financial performance; also useful as a "laboratory" for finding
ideas/vulnerabilities via benchmarking. Data: qualitative + quantitative — reports, observation,
interviews. Typical conclusion: reposition, pilot new features/campaigns, or flag an infrastructure/
capacity gap that will widen if trends continue.

**5. System Dynamics.** What: view interdependencies holistically by modeling forces, feedback loops,
delays, and nonlinear interactions (reinforcing "R" loops amplify change; balancing "B" loops seek
equilibrium). When: uncertain which force or flow will dominate, and when. Data: historical data on
price shocks, pressures, information gaps — used to calibrate initial stocks, flows, and lags; test
scenarios systematically. Typical conclusion: the system may overshoot or oscillate unexpectedly
(due to time-lagged adjustments) — plan for that. Diagram convention: causal links marked "s" (same
direction) or "o"/"−" (opposite direction); clouds = system boundary; accumulators = stocks.

---

## Focal Points — decide what to prioritize (#6–10)

**6. Pareto Analysis.** What: measure the causes of a discrete event/feature/condition and check
whether ~20% of observations drive ~80% of cost or revenue (the 80/20 rule). When: narrowing the
area of investigation or getting a "good enough" answer fast. Data: discrete/countable observations
(failures, complaints, attritions, defect types). Typical conclusion: focus effort on the 20% of
causes with outsized impact — and watch for a "small count, big cost" category the org is
under-weighting (e.g., info/process errors vs. logistics failures).

**7. Leading and Lagging Indicators.** What: map two or more macro/micro trends together over time
to see which one moves first. When: trying to predict a variable's direction or inflection point by
watching a companion "leading" indicator. Data: time-series over a long enough window to see
historical cycles (often macroeconomic). Typical conclusion: focus forecasting effort on the lagging
system, since it will likely follow the known/leading variable — but check whether the lead/lag
relationship itself has flipped over time.

**8. Trade-offs / Equilibrium Points.** What: assess two variables that are mutually exclusive or in
tension (e.g., guns vs. butter production-possibility frontier; accuracy vs. interpretability in ML
models; supply vs. demand curves). When: there's an opposing-outcomes or market-clearing question —
different players/countries choosing different points on a frontier. Data: information on player
positions from public sources, or supply/demand data. Typical conclusion: identify the new clearing
point (price, feature set) that would render a hard choice unnecessary, or explain why two parties
sit at different points on the same frontier.

**9. Portfolio Mapping.** What: map choices as "coordinates" across two important, independent
dimensions (e.g., competitive advantage vs. market attractiveness; feasibility vs. impact) to
visualize a portfolio of alternatives. When: juxtaposing a firm's competitive advantage against
market attractiveness for segment selection, or scope options against feasibility for a project.
Data: qualitative or quantitative scores per option. Typical conclusion: focus on a specific
segment, project scope, or product feature that sits in the high/high quadrant; can be weighted
(sum scores across multiple stakeholder-value criteria) to rank a longer list of options.

**10. Root-Cause Analysis (Fishbone / Ishikawa).** What: trace a problem back to root causes across
categories (4Ms: Machines, Methods, Materials, Manpower; or 4Ps: Policies, Procedures, People,
Plant/Equipment). When: decomposing causes down to primary vs. secondary drivers. Data: starts
qualitative/directional, then quantitative/empirical; causes must be MECE. Typical conclusion: focus
on one or a few root causes rather than treating all symptoms — reduces cost/effort. Process: (1)
agree on the problem, (2) brainstorm categories, (3) map the process where the problem occurs, (4)
brainstorm and link sub-causes (causes, not solutions — "lack of X" is not a valid cause), (5) get
more data (Pareto chart, control chart, histogram), (6) select the root cause.

---

## Decisions — structure choices and decide (#11–15)

**11. Cause-and-Effect Analysis (regression/correlation).** What: identify policy measures or
strategies likely to drive an outcome by testing how two (or more) variables move together —
correlation matrices, binary/linear regression, factor analysis. When: assessing the impact of
controllable drivers while controlling for other variables. Data: explanatory variables for the
system (population, investment, capital/interest rates, policy, etc.). Typical conclusion: focus on
the controllable, statistically significant variable(s), but watch for multicollinearity and keep
searching for mitigating variables (X2...Xn). Caveat this deck states explicitly: correlation is not
causation — more evidence is needed to confirm a causal (not just correlated) relationship.

**12. Elasticity / Sensitivity Analysis.** What: measure the percent responsiveness of a dependent
variable (demand, unit cost) to a percent change in an independent variable (price, input cost).
Related concepts: price sensitivity, experience curve, economies of scale, price-curve slope. When:
assessing a specific behavioral response (e.g., to a price change or new technology). Data:
industry or internal sales/production data. Typical conclusion: decide on price changes, hiring
changes, or pace of technology adoption — and characterize the market as elastic, unit-elastic, or
inelastic before setting policy.

**13. Cluster / Segmentation Analysis.** What: group entities (customers, competitors, regions,
voters) by co-occurring values across several dimensions to reveal segments or structure (e.g.,
K-means clustering, hypersegmentation, response/renewal/customer-value scoring). When: positioning
new features, pricing, or products; deciding where to concentrate limited resources. Data: discrete
attribute/feature data. Typical conclusion: select target segment(s), or surface a smaller-but-more-
lucrative segment the org was previously averaging away (e.g., a high-per-capita mid-market pocket).

**14. Marginal Utility / Pay-offs Analysis.** What: determine how the value of an outcome shifts as
an influencing variable is increased or decreased (ΔV/ΔQ, "S-curve" of value); often operationalized
as a decision tree with chance nodes, decision nodes, and expected NPV/payoff at each branch. When:
exploring changing quantity at a given price, or sequencing a go/no-go decision (e.g., field test →
commercialize → payoff) under probabilistic branches. Data: data similar to sensitivity analysis,
plus probability estimates for each branch. Typical conclusion: decide when to change quantity,
policy, or product availability — pick the branch/path with the best expected (probability-weighted)
payoff.

**15. Monte Carlo Simulation.** What: model risk, variability, and confidence levels for a complex,
uncertain outcome (investment NPV, project schedule, commodity price) by defining a probability
distribution for each input and repeatedly sampling from it (thousands of trials) rather than using
single-point estimates. When: uncertainty is too complex for a deterministic answer and you need a
statistical/probabilistic picture. Data: starting values, plausible ranges, and a distribution shape
(uniform, normal, etc.) for each input. Typical conclusion: invest in features/production based on
the likely (expected) return and its confidence interval — flag that the choice of distribution
shape materially changes the result (this deck's own example: switching from a uniform to a normal
distribution swung a sample NPV from +$429K to −$37K).

---

## Quick reference — matching an insight need to a tool

| If the question is about... | Reach for... |
|---|---|
| What's shaping this industry/market right now | Forces at Work (#1), Five Forces |
| How value/cost flows through the org or vs. competitors | Value Chain (#2) |
| Whether a pattern (S-curve, hockey stick) will continue | Trend Analysis (#3) |
| How we compare to a benchmark or competitor | Gap Analysis (#4) |
| Why a system oscillates, overshoots, or has feedback effects | System Dynamics (#5) |
| Which few causes drive most of the cost/impact | Pareto (#6) |
| Which variable to watch as an early signal | Leading/Lagging Indicators (#7) |
| Where two forces balance out / market-clearing price | Trade-offs/Equilibrium (#8) |
| Which of several options to prioritize on 2 dimensions | Portfolio Mapping (#9) |
| Why a problem is happening, structurally | Root-Cause/Fishbone (#10) |
| Whether X actually drives Y, and how strongly | Cause-Effect/Regression (#11) |
| How much Y responds to a % change in X | Elasticity/Sensitivity (#12) |
| How to group customers/competitors/regions meaningfully | Cluster/Segmentation (#13) |
| Sequencing a decision with probabilistic branches | Marginal Utility/Payoff, decision trees (#14) |
| Quantifying risk/uncertainty in a forecast | Monte Carlo (#15) |

## Presentation conventions worth reusing

- Slide pattern: insight-bearing title stating the conclusion → supporting chart/diagram → a short,
  bolded/italicized "quote" callout restating the so-what in plain language.
- Each tool's write-up follows What is it? / When do we use it? / What data do we need? / What's a
  typical conclusion? before showing the analysis.
- When multiple tools chain together (e.g., Forces at Work → Trend Analysis → System Dynamics for an
  industry outlook, or Segmentation → Portfolio Mapping → Decision Tree for a go-to-market decision),
  say so explicitly — that's the intended combinatorial use of this framework, not a limitation.
