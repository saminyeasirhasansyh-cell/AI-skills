# Source prompts (verbatim)

The original prompts from Prof. Intriligator's design-thinking toolkit, preserved as supplied. The other reference files expand these into runnable procedures; when the two differ, the original intent here wins.

Related: example journey maps — https://www.smaply.com/blog/example-journey-maps

## Contents
1. SUN analysis (main prompt)
2. CLIMBER analysis
3. Persona Multiplication (PMM)
4. The funnel glide
5. The time glide
6. Failure ecology
7. Constraint collision
8. Turning a client's ask into research questions

---

## 1. SUN analysis (main prompt)

Here is a new skill I want to teach you: how to perform a detailed Stakeholders Users Needs (SUN) analysis for a project. When I ask you to perform a SUN, I will have already given you project details (if not, ask for a detailed description). Assuming you understand the project, follow these steps:

**Explore and Enrich the Project and the Project Space:** Deeply explore the project. Understand its goals, stakeholders, users, customers, and aspirations. Use related projects, brainstorming, clustering, and enrichment to gain more insight. Ensure this is done thoroughly before summarizing the project, goals, and challenges in a succinct description.

**Identify Key Stakeholders:** For each stakeholder, describe their role, goals, main tasks, pain points, dream features, and issues to explore. Be sure to cover key activities and responsibilities interacting with the system. Rank stakeholders by importance.

**Identify Key Users/Customers:** For each user, provide details of their role, goals, tasks, pain points, dream features, and issues. Clearly describe their interactions with the system and what they hope to achieve. Rank users by importance.

**Final Synthesis and Recommendations:** Summarize the top 5-7 areas for exploration, providing the most valuable insights for the project. Prioritize 3-5 stakeholders/users to interview, explaining their importance and proposing "interview themes" that can reveal key constraints and opportunities.

**Matrix and Visualization:** If applicable, create a visual matrix or chart mapping stakeholders and users against their roles, needs, and suggested features. Use this to visualize dependencies and relationships between system personas and features.

For context, here are some specific methods and approaches you should consider applying:

* Apply Multidimensional Task Analysis (MTA) to understand the physical, cognitive, emotional, decisional, informational, attentional dimensions. An MTA is like performing a traditional physical or cognitive task analysis, but it is applied across many more dimensions - e.g. emotional, decisional, informational, attentional, material, sustainability, profitability, risk, complexity, investment, etc etc dimensions. Use Teamwork Task Analysis (TTA) if the project involves multiple actors (humans, robots, machines, tools, subsystems, etc) interacting with the system.
* Use Intriligator's CLIMBER model of design thinking (Customer, Life, Insight, Mechanism, Build, Evaluate, Refine) to frame stakeholder and user needs. Each stage (C, L, I…) has sub-steps that should help guide your explorations, these include: C: FLATS—Fears, Loves, Aspirations, Traits, Skills; L: RAMPS—Relationships, Activities, Mappings, Problems, Stakeholders; I: BASE—Brainstorm, Analyze, Synthesize, Ecosystem (market-research, competitor research, lit-reviews); M: GEAR—Generate, Evaluate, Align, Refine; B: PATH—Prototype, Assess, Tweak, Hone; E: SCAN—Scrutinize, Confirm, Adjust, Navigate; R: SPIN—Scrutinize, Pivot, Integrate, Nurture.

---

## 2. CLIMBER analysis

Let me tell you about Professor Intriligator's CLIMBER model of design thinking. Just digest this -- and think about possible extensions or implications of the model -- but no need for an extensive reply -- just reply "I now know how to do a CLIMBER analysis - ask me anything! (the more specific the product/project, the better!)".

The CLIMBER model is a holistic approach to design thinking, consisting of 7 phases: Customer, Life, Insight, Mechanism, Build, Evaluate, and Refine. Each phase has a sub-acronym for a nuanced exploration.

1. **Customer**: Understand the customer's FLAT—Fears, Loves, Aspirations, Traits—to form a foundational understanding of the individual in question. Note: while called "Customer", of course this could also be a user, stakeholder, proto-customer, secondary customer (eg dogs are the consumer/"customer" of dog food, dog owners are the secondary customer… for toys: kids are the customers/users and parents are the secondary-customer, etc etc. When performing this analysis it might be good to ask the user for a detailed description of the customer (and, perhaps begin by offering ideas for possible customers they might want to consider - if you have enough info to do that).
2. **Life**: Dive into the RAMPS—Relationships, Activities, Mappings, Problems, Stakeholders—to contextualize the customer in their environment.
3. **Insight**: Reach the BASE—Brainstorm, Analyze, Synthesize, Ecosystem (market-research, competitor research, lit-reviews)—to generate solutions and hypotheses. The goal is to generate a set of "how might we?" insight statements…. To understand how you could make that customer, living that life, happier, safer, better off, more free, etc etc – generally increase the good and decrease the bad.
4. **Mechanism**: Use GEAR—Generate, Evaluate, Align, Refine—to develop the solution mechanisms, ensuring they're aligned with the insights gathered. In other words, this is the way or ways that you can realize/make/enact the insight(s).
5. **Build**: Follow the PATH—Prototype, Assess, Tweak, Hone—to bring the mechanism to life. Either DO or DESCRIBE how to build that mechanism – offering details and insights.
6. **Evaluate**: Implement a SCAN—Scrutinize, Confirm, Adjust, Navigate—to assess the build's effectiveness. In real life, this is where you take your prototype and show it to users/customers…. In LLM world, perhaps offer detailed descriptions of HOW you would evaluate it.
7. **Refine**: Engage in a SPIN—Scrutinize, Pivot, Integrate, Nurture—to continuously refine and adapt the solution.

This multidimensional approach is more than a linear progression; it's an iterative and layered framework, offering multiple angles for problem-solving and innovation.

If it is not already clear from the context or the prompt, then please ask me for a product and any other details. If (based on context) this is very early in the research, then please just run C and L only, and give me a response in under 500 words.

---

## 3. Persona Multiplication (PMM)

Here is a method I want you to learn and then run for me: Persona Multiplication.

The problem it solves: when a team writes three or four personas, they nearly always describe the same person wearing different jobs. Age and occupation change; the body, the budget, the language, the bandwidth and the household stay the same as the designers'. Everyone the product will fail is missing, and the team cannot see who is missing, because the personas look varied.

The method: instead of inventing a handful of people, first name the DIMENSIONS along which your users actually vary, then multiply along them.

- For this product, list 8 to 12 dimensions of real variation. Go past age and gender: body size and strength, dexterity, vision and hearing, language and literacy, cognitive load and attention, money, time, housing, transport, care responsibilities, documentation status, digital access and data cost, trust in institutions, and whatever else this product touches.
- For each dimension, name the ends and the awkward middle, not just the average.
- Generate 10 to 14 personas by combining ends of different dimensions, including combinations that are uncomfortable or inconvenient for the design.
- For each persona: one line on who they are, one on what they need from this product, and one on how the current design fails them.
- Now sort them. Which three are we designing to win for? Which are we knowingly not serving, and what is the consequence for them?
- Finally, list the three personas we would MISS entirely if we had written only four personas the ordinary way, and say what they would have told us.

Ask me for the product and any constraints before you start. When you report back, keep each persona to three lines, and put the uncomfortable ones first.

Why we do it: the method comes from Pearl and Intriligator, *Persona Multiplication: A Method to Avoid Designed Injustice* (Week 3 readings).

---

## 4. The funnel glide

Use this when the space is too big to think about at once.

Act as my transversal gliding copilot. The goal: [ONE SENTENCE]. First, give me 6 to 8 broad areas I would have to understand before designing anything here. Keep them as short labels, and put them in the order you would explore them, with one line on why that order. Then stop and ask me which area to enter. When I name one, explore it widely across dimensions (physical, cognitive, emotional, social, economic, technical, regulatory, environmental), then compress what you found into exactly five clusters. For each cluster: a short name, two sentences, and one design implication. End every round with three things we should verify with real people, and wait for me.

---

## 5. The time glide

Use this before any futurecasting. It is what makes a forecast specific rather than vague.

Describe [product or service] at four moments: ten years ago, five years ago, two years ago, and today. For each moment, describe it along the same dimensions: materials, safety or regulatory standards, who used it, what it cost, where it was bought, what happened when it broke, and how it was disposed of. Then tell me which dimensions changed fastest, and which have not moved at all. Then project each fast-moving dimension two to five years out, and for each projection say what would have to be true for it to happen. Finally, say which of those futures our client's project is sitting inside, and what that means for what we design now.

---

## 6. Failure ecology

Ask this early, and it will change what you design.

List 25 ways [product] fails in the real world rather than in a lab: misuse, disuse, abandonment, discomfort, embarrassment, cost, theft, repair friction, and the failures that only show up after months of use. Group them into 5 to 7 families. For each family, name the design lever that would reduce it, and say what that lever would cost us elsewhere. Then tell me which failure a user would never report to us, and why.

---

## 7. Constraint collision

Use this to kill concepts before a client does it for you.

Here are our [3 to 5] candidate concepts: [list]. Collide each one with these constraints: certification or regulation, manufacturing, unit cost, weight or size, cleaning and maintenance, repairability, accessibility, supply chain, and the client's own capacity to maintain it after we leave. Score each collision as survives, wounded, or dead, with one line of reasoning. Then recommend one hero concept and one wildcard, and tell me what evidence would change your mind.

---

## 8. Turning a client's ask into research questions

For the first weeks of a client project.

Our client said: "[paste what they actually said]". Turn that into (a) the decision they are really trying to make, (b) five questions we would have to answer to inform that decision, and (c) for each question, the cheapest method that would answer it in two weeks with student resources. Flag any question that cannot be answered ethically or in the time we have, and say so directly.
