# AI Design Tells Catalog

Organized by category. Each entry: the detection signal, why it reads as AI-generated, and a fix
for plain HTML/CSS and for React + Tailwind + shadcn. Severity tags follow the tiers in SKILL.md
(P0 = screams AI, P1 = obvious smell, P2 = cosmetic).

---

## Typography

**[P0] Inter / Roboto / system-font stack, no pairing, no display face.**
Why: these are the un-opinionated defaults every framework ships with, so unprompted output
reaches for them by default rather than by choice.
- HTML/CSS fix: pick a real pairing — a display/serif or distinctive sans for headings, a
  readable, different-feeling face for body (e.g., a slab serif heading + a humanist sans body).
  Load via `@font-face` or a font-hosting `<link>`, set explicit `font-family` stacks, never leave
  the browser default.
- React/Tailwind fix: replace the default `font-sans` token in `tailwind.config` with a real pair;
  don't just add a class to one element — set it at the design-token level so it's consistent.

**[P1] The overused "safe" pick treated as a non-choice (e.g., Space Grotesk everywhere).**
Why: it's become the *second* default — the thing people reach for specifically to avoid Inter,
which makes it just as recognizable as a tell once you've seen enough AI output.
- Fix (both stacks): treat font choice as intentional to the specific brand/content, not a
  category of "not-Inter" fonts. Justify the pick against the direction chosen in step 3.

---

## Color

**[P0] Purple-to-blue gradient on white or near-black background.**
Why: statistically the single most common "AI startup" palette; recognizable within a second.
- HTML/CSS fix: replace with a dominant, deliberate color (60–70% of visual weight), one or two
  supporting tones, and a single sharp accent — not a gradient blend of two hues chosen for
  "looking techy."
- React/Tailwind fix: delete any `bg-gradient-to-r from-purple-* to-blue-*` (or equivalent) as a
  background or `bg-clip-text` headline treatment; replace with a solid dominant color from a
  content-informed palette.

**[P0] Untouched shadcn `zinc`/`slate` default theme.**
Why: shadcn ships with `zinc` as the default base color; leaving it as-is is visibly "I didn't
theme this."
- Fix: change the base color in `components.json` / CSS variables to something that matches the
  chosen direction — even a different neutral (stone, warm gray) reads as an intentional choice.

**[P1] Timid, evenly-distributed palette; default Tailwind `blue-600` buttons.**
Why: no color is doing the work of drawing the eye; every hue gets equal weight, so nothing feels
designed.
- Fix (both stacks): pick one dominant color and let it actually dominate; use the accent
  sparingly and only on the single most important action or data point per screen.

---

## Layout

**[P0] Centered hero + subhead + two buttons + three-card feature grid.**
Why: this is the single most-repeated page shape across AI-generated marketing sites — the
"safe" answer to "build a landing page" regardless of what the product actually is.
- Fix (both stacks): break the symmetry deliberately — an asymmetric hero (text left, real
  product screenshot or illustration right, not centered), a feature section that isn't three
  identical cards (a numbered list, a comparison, a single large illustrated point), diagonal or
  overlapping elements instead of a strict centered grid.

**[P1] The default page shell; three-tier pricing rings; four-column footer; zero asymmetry.**
Why: these are template-level defaults that ship with every scaffold and rarely get questioned.
- Fix (both stacks): vary section-to-section — not every section needs the same grid; deliberate
  negative space or deliberate density, chosen per section rather than applied uniformly.

---

## Components

**[P1] `rounded-2xl shadow-lg` on every surface; reflexive glassmorphism; icon-in-a-rounded-square.**
Why: this is the shadcn/Tailwind starter-kit look, applied without any decision about which
surfaces actually need elevation or a rounded treatment.
- Fix (both stacks): vary corner radius and elevation intentionally — flat surfaces where flat
  serves the content, elevation reserved for genuinely floating/interactive elements. Use
  glassmorphism only where it serves a real layering purpose (a nav over scrolling content), not
  as a default card treatment.

**[P1] Default shadcn `Card`/`Button` with no custom styling.**
Why: shipped components used exactly as scaffolded are the fastest way to look unstyled.
- Fix: override the component's variant/styling to match the chosen direction — border treatment,
  padding, typography inside the component — don't ship the library default as the final UI.

---

## Spacing

**[P2] Uniform `gap-4` / `p-6` everywhere, no spatial hierarchy.**
Why: real designed layouts vary spacing to signal relationships (tight spacing = related items,
generous spacing = a section break); uniform spacing signals nothing.
- Fix (both stacks): establish a spacing scale and use different steps deliberately — tighter
  within a card, looser between sections, extra generous around the single most important element
  on a page.

---

## Motion

**[P2] No motion at all, or the same `fade-in-up` copy-pasted on every element.**
Why: either extreme (nothing, or one animation reused everywhere) signals no thought was given to
which moments actually deserve emphasis.
- Fix (both stacks): pick one or two high-impact moments (a staggered hero reveal on load, a
  meaningful hover/interaction state) rather than animating everything uniformly or nothing at
  all.

---

## Icons

**[P1] The worn `lucide` set used reflexively (Sparkles for "AI", ArrowRight for every CTA, Zap
for "fast"); emoji used as feature bullets.**
Why: these are the first icons every `lucide-react` autocomplete suggests, so they show up
identically across unrelated projects.
- Fix (both stacks): pick icons that represent the *specific* content next to them, not a generic
  stand-in; keep one consistent icon style/weight throughout rather than mixing sets; drop emoji
  bullets in favor of numbered points, a consistent icon, or plain text.

---

## Copy

**[P1] "Elevate / Seamless / Powerful"; generic CTAs; filler microcopy.**
Why: this is marketing-copy convergence, the same phenomenon as design convergence, applied to
words — see the companion `avoid-ai-writing` skill for the full pattern catalog if the copy itself
(not just the visual design) needs a pass.
- Fix: replace vague superlatives with a specific, concrete claim about what the product actually
  does; replace "Get Started" with a CTA specific to the actual next action.

---

## Imagery

**[P2] Gradient placeholders; DiceBear-style generated avatars; generic stock-photo energy.**
Why: placeholder-grade imagery signals nothing was sourced or created specifically for this
product.
- Fix: use a real product screenshot, a purpose-made illustration, or — if no real asset exists —
  a deliberately-styled placeholder that matches the chosen direction rather than a default
  gradient block.
