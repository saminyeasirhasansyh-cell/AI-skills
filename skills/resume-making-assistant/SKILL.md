---
name: "resume-making-assistant"
description: "Only when Samin explicitly invokes it by name (e.g. \"/resume-making-assistant\", \"use the resume assistant\", \"rank my experience for this\") together with a job link or JD — never on a bare pasted job link/JD alone, since resume-tailor already owns that. Fast, low-token ranking of which of Samin's real work experiences, projects, coursework, and skills to keep, cut, or hold as backup for a specific posting — no resume file, no drafting."
---

# Resume Making Assistant (Samin Hasan)

A decision tool, not a resume builder. Given a job posting, it tells Samin which
real experiences/projects to lead with, which coursework (if any) is worth
surfacing, which Skills-line items to keep (under what category titles) vs.
cut or collapse as redundant, and why — in one short reply. It never drafts
bullets, never opens docx/pdf/Artifact tools, and never produces a file.
That's `resume-tailor`'s job; this skill is upstream of it, for when Samin
just wants the ranking call fast.

## When this runs
Only on an explicit call — Samin invokes it by name, or clearly asks to
"rank," "decide," or "tell me what to keep/cut" for a specific posting.
A bare pasted job link or JD with no such ask belongs to `resume-tailor`
(which builds the actual resume) — don't hijack that trigger.

## Speed rules
- No web_fetch beyond ONE call to read the job link/JD if Samin only pasted a
  URL. If he pasted the JD text directly, skip fetching entirely.
- No reading of `resume-tailor`'s reference files. The pools below are the
  source of truth for this skill — condensed indexes of the same real
  history/skillset, kept current by Samin telling this skill directly when
  something changes. Don't re-derive them from scratch each run.
- No file/artifact tools of any kind. Output is a plain chat reply.
- Target under 240 words of output. This is a fast lookup, not a report.
- One reply per posting by default.

## Default vs. separate ranking
Default: experience and projects are ranked together as ONE pool of 14 items
and shown interleaved by relevance in a single Keep list — not grouped into
a "Work Experience" section and a separate "Projects" section.
Exception: if Samin explicitly asks to rank them separately (e.g. "rank
separately," "split experience and projects"), give two labeled lists
(Experience / Projects) for that reply only — don't change the default for
future postings unless he says to.
If Samin asks a short follow-up like "projects?" with no new posting, treat
it as wanting the existing ranking's project items pulled out, not a new pass.

## Samin's experience/project pool (condensed — keep this list current)
Work experience:
1. SuperDataScience — AI Fellow | May 2026–Aug 2026 — agentic AI/multi-agent systems, RAG, fine-tuning, LLM apps, eval/guardrails
2. Auster Center (Tufts Gordon Institute) — Research Assistant | May 2026–Aug 2026 — PRD auditing, sub-requirements, feasibility review, stress-testing, stability/risk diagnosis, $50K+ savings, patent doc translation
3. Tufts University — Program & Operations Associate | Jan 2026–Present — WBS/milestone tracking, 200+ participants, SOPs, Excel/VBA dashboards
4. Tufts University — Marketing Intern | Sep 2025–Present — social media strategy, content marketing, event attendance
5. Edu-Explorer (Founder/PM) | May 2023–Aug 2025 — 0-to-17K users, P&L ($150K+ rev, $100K grants), 12-person team, Agile sprints, CAC/engagement
6. Brac (107K-employee NGO) — Ops & Training Consultant | Dec 2023–Aug 2025 — field deployment, training workshops, donor funding, executive reporting
7. UTC Global Academy — Market Research Analyst | Jun 2021–Aug 2021 — VoC surveys, market sizing, competitor/pricing analysis

Projects:
8. Ori-o (Motor-Assisted Origami Smart Umbrella) — Personal — hardware/mechanical design, human factors, solenoid gear-shift engineering, cost/risk trade-offs
9. JailbreakEDU (Hackathon) — AI tool strategy, PRD standardization org-wide
10. PM Insight Engine — Personal — Python/Cloudflare AI telemetry, feature prioritization
11. EasyDry — Academic — hardware product concept, GTM budget, financial modeling
12. Flowhabit — Academic — customer interviews, UX iteration, subscription pricing MVP
13. SafeFolded — Academic — sustainable packaging, pro forma financial modeling, OKR dashboards
14. Smart Helmet Safety System — Academic — IoT accident detection, emergency response telemetry

If either pool ever looks stale next to what Samin describes, flag it in the
reply in one line and ask him to confirm the update — don't silently guess.

## Samin's coursework pool (condensed, MSEM at Tufts Gordon Institute)
Fall 2025:
- EM 0201 Essentials of Technology Strategy
- EM 0202 Leadership: Personal Development
- EM 0203 Building Financial Intelligence
- EM 0204 Customer Discovery and Solution Design
- EM 0206 Introduction to Data Analytics
- EM 0208 Program and Project Management
- EM 0272 Immersive Experience (Product Management)
- EM 0295 MSEM/MSTML Graduate Seminar (Career Impact)

Spring 2026:
- EM 0205 Milestone Project: New Product & Service Development
- EM 0207 Solving Complex Problems through Systems Thinking
- EM 0209 Essentials of Strategic Management
- EM 0210 Practice of Ethical Leadership
- TML 0193 Intro to Management Consulting

Fall 2026 (in progress, no grade — label as "in progress" if surfaced):
- EM 0211 Lean Six Sigma
- ENP 0161 Human Factor Product Design

Grades are deliberately NOT tracked in this pool — never state or guess a
grade in a reply. If Samin mentions a new term or course, update this list
and say so in one line.

## Samin's Skills-line pool (condensed, from master-resume.md)
- Product & Program Management: Customer Discovery, User Stories, Roadmapping, PRD Writing & Auditing, Product Lifecycle Management, Backlog Grooming & Prioritization, UX Research, Prototyping (Figma, Sketch), Go-to-Market Strategy, MVP Creation & Iteration, Product Launches, Agile Scrum, Sprint Planning, Work Breakdown Structures, Risk & Blocker Management, Release Readiness, Stakeholder Management & Alignment, Cross-Functional Collaboration, Negotiation, Systems Thinking
- Data & AI: Python, SQL, Excel (incl. VBA), Power BI, Dashboards, A/B Testing, Structured/User Data Analysis, Data Visualization, Cursor, Claude Code, RAG, LLMs, Agentic AI, Fine-Tuning, Prompt Engineering, Function Calling, Tool Use, Evaluation Frameworks & Guardrails
- Domain & Technical: Electronics & Telecommunications Engineering fundamentals, IoT telemetry, SCADA modeling (Python), carbon-accounting/emissions measurement systems, Human Factors & Usability Testing
- Tools & Collaboration: JIRA, Monday, Click, Slack, Zoom, PowerPoint

These four category names are a starting point, not fixed labels: when a JD's
own domain calls for a different grouping (e.g. a Business Analyst JD reads
better under "Business Analysis" than "Product & Program Management"), rename
or re-split the categories to match the JD's language, using only skills
already in this pool — never invent a skill to fill a category.

## Workflow
1. Get the JD: use pasted text as-is, or one web_fetch if only a link was given.
2. Pull the JD's top 4-6 real requirements/keywords (skip boilerplate).
3. Score the experience/project pool (14 items) against those requirements in
   a single pass — direct keyword/domain matches score highest,
   transferable/adjacent next, unrelated last.
4. Score every skill in the Skills-line pool into exactly one of three buckets
   — never leave a skill unclassified:
   - **Keep**: directly asked for or clearly relevant to the JD.
   - **Cut**: off-domain for this JD.
   - **Redundant**: a near-duplicate of another kept skill — keep the
     stronger/more specific phrasing, drop the repeat.
5. Decide category titles for the Keep list: reuse the four pool categories
   above when they fit the JD, or rename/re-split them to match the JD's own
   domain language (e.g. "Business Analysis," "Technical & Data," "Tools")
   when that reads stronger — say the titles you'd use, not just the skills.
6. Scan the coursework pool for any course whose title has a real, specific
   tie to the JD's own language (e.g. a technical-PM JD → Program and Project
   Management, Customer Discovery and Solution Design; a strategy JD →
   Essentials of Strategic Management, Intro to Management Consulting). Never
   pad with a generic course just to fill space, and never surface a grade.
7. Reply once, in this shape, nothing extra:
   - One line: culture/role read (e.g. "matrix-leaning technical PM role").
   - **Keep (ranked):** 4-6 experience/project items interleaved by rank in
     one list (or two labeled lists if Samin asked for separate ranking),
     each as `Name — why (≤8 words)`.
   - **Cut:** the rest of the experience/project pool, one line, grouped.
   - **Backup if page needs filling:** 1-2 next-best items not in Keep.
   - **Relevant coursework:** 0-4 courses tied to the JD, comma-separated by
     name only, no grades. Omit this line entirely if nothing in the pool has
     a real tie to the JD — don't force it.
   - **Skills — keep:** one line per suggested category title, e.g.
     `Business Analysis: Customer Discovery, Stakeholder Management...` —
     always name the title, not just a bare skill list.
   - **Skills — cut:** off-domain skills to drop, comma-separated.
   - **Skills — redundant:** near-duplicate pairs, naming which to keep.
8. Stop there. Don't ask if Samin wants a resume built — if he wants one,
   he'll say so, and that's `resume-tailor`'s job (which also owns the
   "fill the page" rule and one-page-density work, so don't duplicate that
   logic here beyond naming backups).

## Things to never do
- Never build, draft, or write actual resume bullets/content.
- Never open the docx/pdf/Artifact tools.
- Never fabricate an experience, project, course, or skill not in the pools above.
- Never state or guess a course grade.
- Never invent a category title's contents — every skill named under a Keep
  category must come from the Skills-line pool.
- Never trigger on a bare pasted job link/JD without an explicit ask to rank/decide — that's resume-tailor's trigger, not this skill's.
- Never split experience and projects into separate lists by default — only when Samin explicitly asks for that in a given reply.
- Never skip the Skills — keep/cut/redundant lines — all three are now a standard part of every ranking reply, and every pool skill must land in exactly one of the three.
- Never force a Relevant coursework line when nothing in the pool genuinely ties to the JD.