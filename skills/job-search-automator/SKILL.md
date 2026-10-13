---
name: job-search-automator
description: Run Samin Hasan's daily co-op / new-grad job search — search Indeed, ZipRecruiter, and Dice for roles fitting his resume, shortlist the real fits, tailor a resume per JD via the resume-tailor skill, draft outreach, and get his explicit approval before anything is sent or applied to. Trigger this whenever Samin says "run my job search," "find me jobs," "job search automator," "today's job list," asks for his daily/weekly job shortlist, or references his recurring job hunt — even if he doesn't name the skill directly. Always use this instead of improvising a one-off job search, since it encodes his real target criteria, quality filters, and approval process.
---

# Job Search Automator (Samin Hasan)

Runs Samin's recurring job search: source postings → filter to genuine fits →
tailor resumes → draft outreach → get explicit approval before anything goes
out. This is a same-session workflow, not a background daemon — it runs each
time Samin invokes it (see "On scheduling" at the bottom for the recurring/
Cowork piece).

## Source of truth
- `/areas/job-search.md` (memory) — target criteria, connectors, and process
  Samin has already confirmed. Read it first; if it's missing or looks stale,
  ask him to re-confirm the fields below rather than guessing.
- `resume-tailor` skill + its `references/master-resume.md` — his real work
  history. Never build a resume without going through that skill.
- Google Calendar / Gmail connectors — for outreach and any scheduling that
  comes out of an application.

## Standing search profile (confirm against /areas/job-search.md, don't re-ask if already answered)
Capture these once and keep them current in memory rather than re-asking each
run — modeled on a config file, not a fresh interview every time:
- **Role stage:** both spring co-op and new-grad/early-career roles
- **Location:** Boston / Northeast only
- **Functions:** ops, strategy, PM-adjacent, data/analytics, sustainability —
  broader than a narrow keyword match; read the JD, not just the title
- **Work authorization:** ask Samin's current status if not already known this
  conversation (independent authorization vs. needs CPT/sponsorship vs.
  citizen/PR). If he needs sponsorship, exclude postings that explicitly say
  "not willing to sponsor" — don't surface them and then discover the problem
  after tailoring a resume.
- **Company blacklist:** companies Samin says never to surface (e.g. a past
  employer, a competitor of a company he's already deep in process with).
  Ask if one comes up, don't assume.
- **Title blacklist:** keywords he wants excluded outright (e.g. "Sales,"
  "Staffing," a title pattern that's wasted his time before).
- **Other preferences, if he states them:** remote/hybrid/onsite tolerance,
  relocation openness, salary floor. Only apply these if Samin has actually
  said them — don't invent defaults.
Do NOT capture demographic self-identification (gender, ethnicity, veteran/
disability status) as a standing autofill field. If a specific application
form asks for that, handle it on that application, in that moment, with
Samin's input — never pre-store it for reuse.

## Workflow

### 0. Check the tracking log first
Before searching, check whatever record exists of prior runs (memory area,
or a log Samin points you to). Don't re-surface a company/role already shown,
tailored, applied to, or explicitly skipped in a prior run — each day should
add new listings, not repeat old ones. If no log exists yet, start one (see
"Tracking" below) rather than starting a new one ad hoc each session.

### 1. Search
Query Indeed, ZipRecruiter, and Dice (all pre-connected) across several
keyword clusters to cover the target functions — e.g. "business operations
analyst," "associate product manager," "sustainability analyst," "data
analyst," "program manager co-op," "strategy analyst." One query per cluster
per platform; ZipRecruiter returns 5 per call, so multiple calls are normal.
Aim for ~30 genuine fits/day — if the real fit count is lower, say so rather
than padding with weak matches. If Samin only wants postings gathered (not
acted on) for a given run, say so up front — that's a valid "collect-only"
mode, distinct from the full pipeline below.

### 2. Filter before presenting
Drop, without asking:
- Anything on the company or title blacklist
- Seniority mismatches (director/senior/staff-level titles)
- Roles outside the confirmed location/function scope
- Sponsorship mismatches per the work-authorization rule above
- Staffing-spam: identical postings mass-copied across many cities from the
  same recruiting agency (a strong tell, not a hard-and-fast rule — use
  judgment)
- Pay-to-train / placement-fee outfits (a well-known pattern: "entry level"
  postings from firms that charge candidates for training/placement rather
  than being the actual employer)
- Already-seen postings per the tracking log (step 0) — one application per
  company per cycle by default, unless Samin explicitly wants to try again

### 3. Present the shortlist
Ranked list, grouped as "strong fits" and (if relevant) "skip, with reasons"
for anything borderline you excluded so Samin can override you. For each:
title, company, location, comp if available, apply link, one line on why it
fits. Then stop and wait — don't tailor anything yet.

### 4. Tailor on request
For whichever roles Samin flags, hand off to the `resume-tailor` skill in
full (culture read, JD-driven cuts, docx build). Don't shortcut it.

### 5. Outreach (drafted, never sent unprompted)
If Samin wants a recruiter/team touchpoint for a role:
- **LinkedIn:** draft the connection note / message for him to send himself —
  no LinkedIn connector exists, and automated LinkedIn messaging risks his
  account, so this is always self-send.
- **Email:** draft it, show him the draft, and only send via Gmail after he
  explicitly approves that specific message.

### 6. Applying — approval gate, every time
Never submit an application without Samin's explicit go-ahead on that
specific role. Two paths, per his call each time:
- **Self-submit:** hand him the tailored resume + apply link, he does the rest.
- **Email application:** draft the application email with resume attached,
  show it, send via Gmail only after he says go.
Don't assume last time's answer carries over to a new role — confirm per role
unless he's told you to default to one path for a batch.

## Tracking
Keep a running record across runs so the daily batch stays genuinely new:
- **Shown:** every posting surfaced, so it's never presented twice
- **Tailored:** roles a resume was built for
- **Applied:** roles actually submitted (self-submit confirmed by Samin, or
  email sent by Claude after approval)
- **Skipped:** roles filtered out or declined, with a one-line reason
If Samin hasn't set up a specific place for this (a sheet, a doc), keep it as
a simple dated log and ask him where he'd like it to live long-term rather
than silently accumulating it session-to-session.

## On scheduling / Cowork
This skill makes each run of the workflow reliable and repeatable, but it
doesn't make the workflow run unattended — a skill triggers when Samin (or
Cowork) invokes it in a session, not on a timer by itself. To get a genuine
daily unattended run (the way his text-to-calendar automation runs), Samin
needs to set this skill up as a **scheduled Cowork task** from within Cowork
itself: open Cowork, point it at this skill (or paste this SKILL.md), and set
a daily recurring schedule. From a plain Claude.ai chat there's no scheduling
mechanism to configure that — the most this skill can do here is run well
each time it's invoked.

## Keeping /areas/job-search.md current
When Samin changes a target criterion (fields, location, authorization
status, connectors), that should get captured in memory the normal way —
don't just apply the change in this session and let it lapse next time.
