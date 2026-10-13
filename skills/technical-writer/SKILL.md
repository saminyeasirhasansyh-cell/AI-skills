---
name: technical-writer
description: Write, improve, or restructure technical documentation — API references, SDK docs, developer guides, admin manuals, integration guides, troubleshooting docs, and getting-started guides. Use this whenever the user asks to draft, edit, or review a README, API reference, user guide, tutorial, changelog, or any developer-facing documentation, or asks to make existing docs clearer, more complete, more scannable, or more consistent in style. Also use when the user asks for a documentation audit, a content gap analysis for docs, or help planning an information architecture for a docs site.
---

# Technical Writer

Write documentation that helps users succeed with a product with the least possible friction — clear enough that support tickets go down, complete enough that nothing has to be guessed, and structured so people find the one paragraph they need without reading the rest.

## Before writing

Get oriented before producing content:

1. **Identify the audience.** A developer integrating an API needs different depth than an end user clicking through a UI. If it's ambiguous, ask or infer from context (file names, existing docs, the product itself) rather than defaulting to one style.
2. **Survey what exists.** If there's a docs folder, README, or prior version of the page, read it first (`Glob`/`Grep`/`Read`). Match its terminology and structure unless the user asked for a rewrite — inconsistent terminology across a doc set is one of the fastest ways to erode trust.
3. **Confirm the format.** Markdown page, docstring, README section, full guide? Check for an existing style guide or docs template in the repo and follow it.
4. **Scope the task.** "Document this API" could mean one endpoint or forty. Check the actual surface area (read the code/spec) before estimating or starting.

## Document types and what each needs

- **API reference** — every endpoint: method, path, auth requirements, parameters (with types and whether required), a request example, a response example, and the error responses that can come back. Don't document the happy path only.
- **Getting-started guide** — the shortest path from zero to a working result. One clear prerequisite list, then numbered steps, then a "what you just did / what's next" close. Cut anything not needed for that first success.
- **User guide / feature doc** — task-oriented, not feature-oriented. Organize around what the reader is trying to accomplish ("Export your data") rather than the UI's menu structure ("The Export Button").
- **Troubleshooting guide** — organize by symptom the user is experiencing, not by internal cause. Each entry: symptom → likely cause → fix, with a copyable command or setting where relevant.
- **SDK / integration guide** — an install step, an authentication step, one minimal working example, then a link out to the full API reference rather than re-documenting every parameter inline.
- **Changelog / release notes** — group by user impact (Breaking changes / New features / Fixes), not by internal ticket number. Lead each entry with what changed for the user, not the implementation detail.

## Writing principles

- **Task-based, not feature-based.** Structure around what the reader is trying to do.
- **Progressive disclosure.** Put the common case first and plainly; push edge cases, advanced options, and internals lower on the page or into a separate reference doc. A reader should be able to stop reading once they've solved their problem.
- **Show, then explain.** Lead with a working code example or concrete step, then explain what it does — not the reverse. Most technical readers scan for the example first anyway.
- **Active voice, present tense, second person.** "Click Save," not "The Save button should be clicked by the user."
- **One idea per sentence; short paragraphs.** Long paragraphs of prose are where developer docs go to be skipped.
- **Consistent terminology.** Pick one term per concept and use it everywhere (don't alternate "field," "property," and "parameter" for the same thing). If the product/codebase already has a term, use theirs.
- **Every code example must be runnable as written.** No pseudocode dressed up as a real example — placeholder values should be clearly marked as placeholders (e.g. `YOUR_API_KEY`).
- **Document errors, not just success.** For anything with failure modes (API calls, CLI commands, config), include what a failure looks like and how to resolve it.
- **Write the heading a reader would search for.** Headings are the units people actually scan; make each one answer a specific question ("Authenticate with an API key," not "Authentication Overview").

## Structure defaults

Unless the user or an existing style guide specifies otherwise:

```markdown
# [Product/Feature Name]

[One or two sentences: what this is and why someone would use it.]

## Prerequisites
[Only if there are any — don't include an empty section.]

## Quickstart / Getting started
[Shortest path to a first working result, numbered steps.]

## [Task-based sections]
[One section per thing a reader wants to accomplish.]

## Reference
[Exhaustive parameter/config/endpoint details, for lookup rather than reading start-to-end.]

## Troubleshooting
[Only if there are known common failure modes.]
```

Drop sections that don't apply rather than leaving stub headers.

## Review checklist

Before treating a doc as done, check it against:

- [ ] Every code example is accurate and would actually run
- [ ] No unexplained jargon or unlinked acronyms on first use
- [ ] Headings are specific enough to scan and jump to
- [ ] Terminology is consistent with the rest of the docs / codebase
- [ ] Error cases and edge cases are covered, not just the happy path
- [ ] A reader with the stated prerequisites and no other context could actually follow it
- [ ] Nothing states something as fact that wasn't verified against the code, spec, or source the user provided

## When editing existing docs

State briefly what was unclear, incomplete, or inconsistent before rewriting — this helps the user judge whether the edit fixed the right thing. Preserve any voice/style choices that are clearly intentional house style rather than accidental inconsistency. Don't restructure a whole doc when the user asked for a targeted fix; scope the edit to what was asked unless the surrounding structure is actively broken.
