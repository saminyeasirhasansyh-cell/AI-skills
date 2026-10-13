---
name: "resume-tailor"
description: "Build and tailor Samin Hasan's one-page resume for a specific job posting. Trigger this whenever Samin pastes or describes a job description, names a company/role he's applying to, asks for a resume, asks to \"tailor my resume for X,\" shares a new work experience/project/course to fold in, or asks about ATS optimization, cover-callback strength, or company-culture fit for his resume — even if he doesn't say the word \"skill.\" Always use this instead of improvising a generic resume, since it encodes his real work history, link URLs, and the JD-driven cutting rules he wants applied every time."
---

# Resume Tailor (Samin Hasan)

Produces a one-page, ATS-optimized resume tailored to a specific job description
(JD) and that company's working style — pulling only from Samin's real, verified
work history. Never invents metrics, tools, or claims not present in
`references/master-resume.md`.

## Source of truth
- `references/master-resume.md` — every role, project, cert, award, and real
  link URL (LinkedIn/GitHub/Portfolio/project pages). This is the only place
  content comes from. Read it in full before drafting.
- `references/coursework.md` — optional relevant-coursework content from EM 211
  (Lean Six Sigma) and ENP161 (Human Factors in Product Design), plus rules on
  when to include it and how to phrase in-progress items honestly.
- `references/culture-analysis.md` — how to read the JD + company signals to
  decide what to emphasize/cut (waterfall vs. matrix vs. in-between).
- `references/ats-checklist.md` — formatting and keyword-parseability checklist.
- `assets/style_reference_sample.docx` — a *formatting/layout* reference only
  (section order, one-page density, XYZ-style bullets). Its content belongs to
  someone else — never copy its wording or its specific numbers.

## Full MSEM coursework record (Tufts Gordon Institute, from official transcript)
Samin's complete, verified course list — use it to confirm GPA-supporting
coursework, term dates, and grades whenever a JD or Samin asks for accuracy beyond
the two "resume-worthy" methods courses in `coursework.md`. Only EM 211 and ENP161
normally earn their own resume bullet (per `coursework.md`'s rules) — the rest
support the "GPA 3.85" / "Coursework: ..." line under Education, not standalone bullets.

**Fall Term 2025**
- EM 0201 Essentials of Technology Strategy — A
- EM 0202 Leadership: Personal Development — A
- EM 0203 Building Financial Intelligence — B+
- EM 0204 Customer Discovery and Solution Design — A-
- EM 0206 Introduction to Data Analytics — A
- EM 0208 Program and Project Management — A
- EM 0272 Immersive Experience (Product Management) — A
- EM 0295 MSEM/MSTML Graduate Seminar (Career Impact) — A+

**Spring Term 2026**
- EM 0205 Milestone Project: New Product & Service Development — B+
- EM 0207 Solving Complex Problems through Systems Thinking — B+
- EM 0209 Essentials of Strategic Management — A-
- EM 0210 Practice of Ethical Leadership — A-
- TML 0193 Special Topics: Intro to Management Consulting — A-

**Fall Term 2026 (in progress, no grade yet)**
- EM 0211 Lean Six Sigma
- ENP 0161 Human Factor Product Design

If Samin's actual GPA or term dates ever conflict with what's in
`master-resume.md`'s Education section, this transcript-sourced list wins —
update `master-resume.md` to match and flag the correction to Samin.

## Workflow

### 1. Get the job description
If Samin hasn't pasted the JD or a link to it, ask for it — don't guess at a
target role. If he gives a company + role name only, web_search for the current
posting and read it with web_fetch before proceeding.

### 2. Analyze company culture and work style
Follow `references/culture-analysis.md`: mine the JD's own language first, then
do 2-3 targeted web searches (careers page, culture reviews, engineering/product
blog) to place the company on the waterfall ↔ matrix spectrum. State your one-line
read (e.g. "matrix-leaning consumer software PM role") before drafting — share it
with Samin inline as you present the draft, not as a separate approval gate,
unless the signal is genuinely ambiguous.

### 3. Select and cut content
Using `master-resume.md` as the pool:
- Pick the roles/projects/bullets that best answer the JD's top requirements,
  weighted per the culture read from Step 2.
- Cut ruthlessly to fit one page — prefer fewer, sharper bullets over cramming.
  Depth on 2-3 most-relevant roles beats shallow coverage of everything.
- Every bullet you keep should show initiative/curiosity (see the "Always true"
  section of culture-analysis.md) — reword passive bullets into active,
  problem-finding framing without changing the underlying facts or metrics.
- Decide whether a "Relevant Coursework" line earns its space per
  `coursework.md` — it's optional, not default-on.
- Confirm/attach the correct links (LinkedIn, GitHub, Portfolio, individual
  project links) from `master-resume.md` — never fabricate a URL, and if a
  project you want to feature has no link on file, ask Samin for it rather than
  guessing or omitting silently.

#### Fill the page
A one-page resume means using the full page, not just avoiding overflow. After
picking the strongest, most-relevant roles for this JD, check whether the draft
actually fills the page. If the most-relevant roles/bullets leave visible white
space at the bottom, don't just leave it empty or stretch margins/line-spacing to
pad it out — pull in additional real content from `master-resume.md`'s fuller
pool to fill it, in this order of preference:
1. Additional roles from master-resume.md not yet included, even if only loosely
   relevant (e.g. Brac, UTC Global Academy, Tufts Marketing Intern).
2. Applied academic/personal projects (EasyDry, Flowhabit, PM Insight Engine,
   New Venture Financial Modeling, SafeFolded, Smart Helmet Safety System, Ori-o,
   JailbreakEDU) — pick whichever reads as closest in spirit to the JD's domain
   or skills, even if the connection is more "adjacent/transferable" than a
   direct keyword match. Frame the bullet's opening clause to draw out the
   transferable angle (e.g. a hardware/IoT project for a technical-ops JD:
   emphasize the systems-thinking and cross-functional delivery, not just the
   hardware specifics).
3. Restore a cut bullet on an included role rather than leaving a role
   under-described.
Every add here still obeys the "never fabricate" rule — only real content from
master-resume.md, never a stretched or invented claim. If, after adding
everything relevant/adjacent, the page is still visibly short, say so to Samin
rather than silently leaving white space — that's a signal his master resume
needs more raw material, not a formatting problem to hide. If filling the page
this way would mean writing wordy or padded bullets, don't — concision (see
below) always wins over reaching a line-count target with filler.

### 4. Write for a callback, not just accuracy
- Lead the summary line with the exact job-family language the JD uses.
- Front-load metrics in bullets; use the JD's own keywords wherever Samin
  genuinely has the matching experience (don't force a keyword that isn't true).
- Keep tone active/confident, never boastful-without-evidence — every claim
  should be traceable to master-resume.md.

#### Bullet format: tight Google XYZ, not wordy
Every bullet follows Google's XYZ formula — "Accomplished [X], as measured by
[Y], by doing [Z]" — but written as tightly as the formula allows, never as a
full restatement of everything in master-resume.md's fullest version of that
bullet:
- Hard cap: one line at normal resume width, roughly 12-20 words. If a bullet
  wraps to a third line, cut it, don't shrink the font to fit it.
- Lead with the result/metric, not the setup. Cut throat-clearing openers
  ("Successfully...", "Was responsible for...", "Worked on...", "In order
  to...") entirely.
- One idea per bullet. If master-resume.md's version of a bullet chains two
  achievements with "and"/"while"/"then," split it or drop the weaker half
  rather than keeping both at full length.
- Cut filler and hedging words on sight: "successfully," "various,"
  "responsible for," "in order to," "a variety of," "utilized" (say "used"),
  "leveraged" (say what was actually done), double adjectives, and any clause
  that restates the job title instead of adding new information.
- Keep every number, named tool, and concrete mechanism — concision cuts
  words, never facts, metrics, or the specific method that makes the claim
  credible. When forced to choose between a word-count target and losing a
  real metric, keep the metric and cut somewhere else instead.
- This applies to every bullet on the page — Experience and Projects alike —
  not just the ones Samin flags as wordy. Re-read the full draft once for this
  before presenting it.

### 5. Run the ATS pass
Check the draft against `references/ats-checklist.md` line by line before
presenting it as final. Also re-check the bullet-concision rule above as its
own pass — flag anything you had to compromise on (e.g. "kept this at 10.5pt
margins to fit one page — want me to cut one more bullet instead?").

### 6. Build the file
Use the **docx skill** (`/mnt/skills/public/docx/SKILL.md`) to produce the actual
resume file — read it before generating. Section order: Education → Experience
→ Projects → Leadership/Awards → Skills. The earlier sections may be reordered
if the JD calls for leading with a different one (e.g. Projects before
Experience for a portfolio-heavy JD) — but **Skills always goes last, full
stop, never reordered ahead of any other section**, regardless of what the JD
emphasizes. Match the one-page density of `assets/style_reference_sample.docx`,
but write 100% original content from master-resume.md. Save to
`/mnt/user-data/outputs/`, then use `present_files` so Samin can open and
download it.

#### Formatting: Projects match Work Experience
Every entry in Hackathons & Applied Projects (and any other projects section)
must use the exact same layout as a Work Experience entry: a bold title on the
left with a right-aligned tag on the same line (dates for a timed engagement,
or "Personal Project"/location when there's no date range), then bullets
underneath. Never fold a project's title or link into the leading text of a
bullet — give it its own header row first, the way JailbreakEDU and Ori-o are
structured, so projects read with the same visual weight and scan pattern as
real roles.

#### Wording: Lean Six Sigma Black Belt credential
When this in-progress credential appears anywhere on the resume (Certifications
section or elsewhere), phrase it as just "Lean Six Sigma Black Belt — in
progress via EM 211 course project, contingent on documented
process-improvement results (expected Aug 2027)" or equivalent honest
in-progress phrasing per `coursework.md`. **Never prefix it with "Tufts Gordon
Institute"** — that affiliation is already established by the Education
section and repeating it here is redundant; state the credential name and
progress status only.

### 7. Keep the master resume current
Whenever this conversation surfaces something new — a new job, a new project, a
completed course deliverable, a new certification, a corrected metric — update
`references/master-resume.md` directly (don't just mention it and move on), per
the "Keeping this file current" section at the bottom of that file. This is what
makes future tailoring fast: the next JD doesn't require re-asking Samin for his
whole work history.

## Things to never do
- Never fabricate a metric, tool, employer, or link not present in
  master-resume.md.
- Never claim the Lean Six Sigma Black Belt (or any in-progress credential) as
  already held — see coursework.md for exact phrasing.
- Never prefix the Lean Six Sigma Black Belt credential with "Tufts Gordon
  Institute" — see "Wording: Lean Six Sigma Black Belt credential" in Step 6.
- Never place the Skills section anywhere but last — see Step 6's section-order
  rule. This holds even when reordering other sections for a JD.
- Never exceed one page.
- Never leave the page visibly under-filled when relevant/adjacent real content
  in master-resume.md could fill it — see "Fill the page" in Step 3.
- Never write a wordy, throat-clearing, or filler-laden bullet — see "Bullet
  format: tight Google XYZ" in Step 4. Concise and high-impact beats
  comprehensive.
- Never cut a real metric or concrete mechanism to hit a word-count target —
  trim filler words instead.
- Never copy wording or numbers from `assets/style_reference_sample.docx` — it's
  a stranger's resume kept only for layout/format reference.