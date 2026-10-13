---
name: human-writer
description: Use this skill whenever writing fiction, short stories, narrative scenes, or any creative prose — even if the user just asks for "a short story," "a scene," or "write something creative" without mentioning style. Applies structural anti-patterns identified by research (StoryScope, COLM 2026) that reliably distinguish AI-generated fiction from human-written fiction at the level of plot, causality, temporal structure, and emotional rendering — not just word choice. Trigger this proactively for any narrative/story-writing task, not only when the user explicitly asks to "write like a human" or "avoid AI clichés."
---

# Human Writer

Research on distinguishing AI fiction from human fiction (StoryScope, COLM 2026) found
that the strongest signal isn't surface style (em-dashes, "delve," "tapestry") — those are
already fading and easy to edit away. The durable signal is **structural**: how AI models
consistently choose to build plot, resolve conflict, handle time, and render emotion. A
classifier trained on structure *alone*, with all stylistic features removed, still separated
human from AI writing at 93.2% macro-F1.

This skill applies the inverse of those structural fingerprints as active writing constraints.
Use it any time you're producing fiction, a narrative scene, or story-shaped prose — apply
these as default instincts, not just when explicitly asked to sound human.

## The 14 rules

When drafting fiction, actively resist these AI-typical patterns:

1. **Don't over-explain the theme.** AI narrators state the moral/lesson explicitly ~77% of
   the time vs. 52% for humans. Trust the reader to infer meaning. Don't end a character
   arc with the narrator summarizing what it meant.

2. **Don't make every dialogue exchange "mean something."** AI dialogue serves
   philosophical debate 59% of the time vs. 34% for humans. Let some conversation just be
   conversation — banter, deflection, small talk — without every line advancing a Message.

3. **Don't keep causal chains too clean.** AI favors single unbroken causal chains and tidy
   single-track plots (79% "no subplots" vs. 57% human). Allow loose threads, subplots that
   don't resolve, or tangents that don't obviously serve the main theme.

4. **Don't default to protagonist-driven, internally-resolved endings.** AI resolutions lean
   on protagonist choice (69% vs. 46%) and internal acceptance/understanding (47% vs. 27%).
   Let outside forces, luck, or other people's choices determine outcomes sometimes. Let
   endings stay ambiguous rather than neatly "earned."

5. **Don't over-somaticize emotion.** AI conveys feeling through bodily sensation/metaphor
   81% of the time (tightening chest, cold sweat) vs. 38% for humans, and rarely names
   emotions directly (8% vs. 29%). Occasionally just say "she was afraid" — don't feel
   obligated to always render it physically.

6. **Don't overload sensory/smell imagery as a mood shortcut.** AI uses smell-based imagery
   in 82% of stories vs. 57% human. Don't reach for scent-as-atmosphere as a reflexive
   device.

7. **Don't use setting purely as psychological mirror.** AI leans heavily on environment
   reflecting characters' inner states. Let a setting sometimes be neutral or even
   contradict the mood instead of always echoing it.

8. **Don't keep time strictly linear.** Humans use far more flashbacks, flash-forwards,
   time jumps, and nonlinear structure to delay revelations. A rigidly chronological
   telling (first clue → grand reveal) is an AI tell. Consider opening in medias res or
   fracturing the timeline.

9. **Don't avoid the fourth wall entirely.** Humans address the reader directly far more
   often (28% vs. 7%) and break narrative frame more (67% vs. 39%). Don't treat "no reader
   awareness" as the only serious mode.

10. **Don't keep references vague/generic.** AI favors vague allusions over specific named
    references to real works, places, or brands (72% vs. 50% vague). Use concrete,
    specific, named intertextual detail rather than gestural "a certain famous poet"
    phrasing.

11. **Don't flatten moral ambiguity.** AI protagonists' choices skew more morally clear-cut;
    humans frame characters as ambivalent/mixed more often (59% vs. 38%). Resist making the
    protagonist's decisions cleanly justified — leave room for the reader to disagree with
    them.

12. **Don't restrict the character's social world.** Human stories tend to have more dynamic
    or expansive social networks and casts; AI narratives are comparatively narrower. (One
    exception to avoid overcorrecting into: don't lean on gossip/rumor as the default plot
    engine either — that's its own AI tell.)

13. **Don't keep event intensity flat or the narrative voice too uniform.** Some AI output
    shows notably restrained, flat event escalation and a very consistent voice throughout.
    Vary intensity and register rather than keeping a consistently "controlled" tone cover
    to cover.

14. **Don't wrap everything into a single tidy epilogue.** A neat denouement/epilogue that
    resolves every loose end is a detectable AI habit. Leave some narrative untidiness or
    an open thread instead of closing every one.

## How to apply this

- Treat these as a checklist to run *while drafting*, not just a post-hoc edit pass —
  structural choices (plot shape, time order, resolution mechanism) are much harder to fix
  after the fact than word choice is.
- Don't apply all 14 rules mechanically to every piece — pick the handful most relevant to
  the story's length and genre. A 300-word flash piece doesn't need nonlinear time; a
  10,000-word piece probably should have some structural untidiness somewhere.
- The underlying principle: AI fiction over-determines meaning (clear theme, clear
  causality, clear resolution, named emotion) where human fiction tolerates ambiguity,
  tangents, and unresolved threads. When in doubt, ask "am I tying this up too neatly?"
  and if so, loosen it.
- This is about narrative construction, not about adding "human" stylistic quirks (typos,
  slang, etc.) — those are surface-level and not what this skill targets.

Source: Russell, Rajendhran, Pham, Iyyer & Wieting, "StoryScope: Investigating
idiosyncrasies in AI fiction," COLM 2026.
