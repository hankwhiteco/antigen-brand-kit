# Creative direction

The system behind the brand. How to make judgment calls the spec files don't cover. Color, type, and logo define the raw elements. This file is how they get applied.

## Moves

The visual elements, motifs, and graphics the brand uses, and the consistent way it applies them, to create cohesion and recognition. Color, type, and logo define the raw elements; this is how they combine into something recognizable.

<!-- Each move: name it, describe the maneuver as an instruction that produces a recognizable result, and give the intent: why it exists, what it's meant to signal. Intent is what lets the machine extrapolate to a surface no one anticipated. Fill from the sprint. -->

**Classical statuary.** Use a black-and-white Greek/Roman marble bust as the hero image, cropped large and calm against a light ground. *Intent:* the timeless adversary — antiquity meets AI; gravitas and permanence under a technical, modern system. This is the brand's signature image; reach for it first on hero surfaces.

**The number motif.** Place an oversized `02.16` / `0216` in Chivo Mono, Scarlet (or reversed on Bark), as an edition/marker anchor — often rotated up a vertical edge panel. *Intent:* ordinal precision, a technical signature; it reads as a serial stamp, not literal data.

**Mark as graphic.** Deploy the burst icon at three scales — inline marker (small, in text), section marker (medium, opening a zone), or watermark/ghost (huge, cropped at the edge, low-opacity Greige or a bold Scarlet crop). *Intent:* brand presence as texture and structure without competing with the headline.

**Rice & pattern texture.** Lay the rice-paper crackle or organic leaf pattern over light grounds and Bark panels. *Intent:* warmth and tactility that offsets a cold security subject — keeps the system human.

**Edge panels + 1px zoning.** Anchor a layout with a full-height Bark panel on one edge and/or a Sage bar on the other, and split zones with 1px hairline dividers (Greige, Oxblood, or Scarlet). *Intent:* editorial rigor and an asymmetric grid; the structure of an audit report.

**Scarlet mono eyebrow.** Set the eyebrow (`SECURES YOUR ENTIRE ATTACK SURFACE`) in Chivo Mono, uppercase, tracked, Scarlet, near the top-left or under the headline. *Intent:* a consistent tag that flags the surface as Antigen at a glance.

**Collage / layered imagery.** Build image zones by overlapping, not by dropping one photo into a box. Stack two or more black-and-white duotone images (marble busts, a photographed portrait, stippled art) so they meet at hard seams, lay a Rice or Pattern texture semi-transparent over part of an image, and set the burst mark large across the seam where two images meet. Let ghost marks sit at more than one scale and bleed off the edge. Scarlet is the only color on the imagery, nothing else. *Intent:* the layered dossier, an adversary assembling the picture from fragments. This is the signature of the brand's richest surfaces and the thing that stops a hero from reading as a stock photo in a column. See `examples/good/` for the target.

## Composition & density

How elements are arranged and how much goes on a given area: layout, proportion, whitespace, type scale, how many elements per zone. Governs whether something feels composed or crammed.

<!-- The section that stops output from going generic. Everything can be right, correct color, type, moves, and the thing still looks templated because the spacing is default and every zone is equally full. Rules go here as testing surfaces them: copy limits per zone, one idea per zone, hard type-scale jumps, what breathes vs. what fills. -->

- **Full-height asymmetric zones.** The layout is full-bleed vertical zones of uneven width, not a centered container with even columns. Run a Rice or White field as the main ground, pin a Bark panel and a Sage bar to the far edges, and split zones with 1px vertical hairlines. Columns are deliberately unequal and content sits off-center inside the field. Anchor the asymmetry with a giant number or the logo rotated up a vertical edge. If every column is the same width and the composition is centered, it is wrong.
- **Light-ground dominant.** White / Rice fills ~60% of the surface; Bark and Sage are edge anchors, not the field. Scarlet stays ~10% — a spark.
- **One idea per zone.** A zone holds the headline, or the statue, or the big number — not all three fighting. Let the hero image breathe with real whitespace around it.
- **Hard type-scale jumps.** Go Display/H1 straight to Body — no safe mid-scale filler. The jump is the composition.
- **Asymmetric, left-aligned.** Columns are uneven and divided by 1px verticals; body copy is left-aligned, never centered.
- **0px radius, flat.** No rounded corners, no shadows, no elevation — edges are hard, color is flat (texture is the only surface treatment).

## Restraint: when to do less

When to hold back. Which moves to drop when a piece is doing too much, and when a plain treatment is the right answer.

<!-- Fill as testing surfaces the over-reaches. -->

- **One hero move per surface.** Statue *or* the giant number *or* the oversized ghost mark — not all at once.
- **Drop the texture** when a zone is type-dense; Rice/Pattern is for open grounds, not behind body copy.
- A plain, correct default is strong: Bark headline on a White ground, one Scarlet mono eyebrow, generous margins. If in doubt, ship that.

## Default corrections

The machine ships with a house style. Left unguided, it reaches for these on its own. None of them are in the brand's designs. Think of this as a CSS reset: clear the defaults before applying the brand, then re-enable any line the brand actually uses.

**Color & surface**

- No gradients the brand didn't define
- No glassmorphism, frosted panels, or blur
- No drop shadows, glows, or soft elevation
- No dark-mode assumption unless specified

**Shape & form**

- No rounded corners unless specified
- No pill-shaped buttons by default
- No circular icon badges

**Layout**

- No centered body text
- No three-column icon-topped feature grids
- No card-ifying every block. Not every block needs a container
- No forced symmetry when the brand is asymmetric

**Type**

- No shrinking to safe mid-scale sizes, respect the brand's scale jumps
- No unspecified font weights
- No all-caps unless the brand uses it

**Decoration**

- No emoji or decorative icons as bullet substitutes
- No filler illustration or stock-y spot graphics
- No divider between every section
- No standalone dashes as content, headings, or placeholders. A big dash set as a number, a label, or a section divider is not a design element. If a value is missing, omit it or flag it as placeholder, never fill the space with a dash.

<!-- This block carries over to every kit unchanged. Add to it as you catch new AI tells across projects. It's a shared Bolster asset, not brand-specific. -->

**Antigen re-enables:** flat color with **Rice/Pattern texture** on light grounds; **0px radius** on all buttons/inputs; **UPPERCASE tracked mono** for eyebrows, CTAs, and labels; the **burst mark as an oversized graphic**. These are brand-sanctioned — everything else in the reset stands.

## Failure modes (brand-specific)

What wrong looks like for this brand in particular. The mistakes this brand's own system invites. Empty at the start; fills in as testing surfaces repeat offenders.

<!-- A rule enters when the same mistake shows up twice. Once is a bad prompt. Twice is a missing rule. Name the failure concretely enough to catch on sight. -->

**Filled box in the nav.** The Get a demo CTA in the header is text: Chivo Mono, uppercase, tracked, no fill and no border. If it renders as a solid Oxblood or Scarlet box, that is wrong. Filled buttons are for in-page actions, not the header. Nav links are Clash Grotesk 16px, not mono.

---

# Components

Component specs transcribed from the design system (`visual/assets/imagery/antigen design system.pdf`). That file is authoritative: where a recipe or spec here disagrees with it, the design system wins. All controls are 0px radius.

## Navigation

Header layout: logo left, nav links and the Get a demo CTA on the right.

| Element | Spec |
|---|---|
| Nav links | Clash Grotesk Variable, 16px, Oxblood. |
| Link hover | 1px underline, Oxblood. |
| Link active | Scarlet. |
| CTA | `Get a demo`. Chivo Mono, uppercase, tracked. Plain text, no fill and no border. |

Nav links are Grotesk, not mono. Only the CTA is mono, and it stays text, never a filled button.

## Buttons

Three button types. Filled and outline buttons are 44px tall with 0px radius. Labels are Chivo Mono, uppercase, tracked (the CTA type style).

**Text CTA.** Label only, no fill and no border. States: default, hover (1px underline), disabled (greyed). This is the header CTA and inline text actions.

**Filled.** 44px tall, 0px radius. Three fills, each with a darker hover:

| Fill | Label |
|---|---|
| Oxblood | White |
| Scarlet | White |
| Pale Olive (Sage) | Oxblood |

**Outline.** 44px tall, 0px radius, 1px border. Default is an Oxblood border with an Oxblood label. Hover fills Oxblood with a white label. A ghost variant uses a light Greige border for low emphasis.

All three fills are sanctioned. Pick one primary action per surface and choose the fill by context; do not fall back to the Oxblood fill on reflex.

## Form elements

Inputs, checkboxes, and radios. 0px radius throughout. Field labels sit above the control in Chivo Mono, uppercase, tracked (for example `EMAIL ADDRESS`). Value text is Clash Grotesk.

**Text input.** 1px border, 0px radius.

| State | Treatment |
|---|---|
| Default | Light Greige border, grey placeholder. |
| Focus | Oxblood border, visible cursor. |
| Filled | Oxblood value text. |
| Error | Scarlet border with a helper line below in Scarlet (for example "This field is required"). |
| Disabled | Greyed border and fill. |

**Checkbox.** Square, 0px radius. Unchecked is a light Greige border. Checked is an Oxblood fill with a white check. Error is a Scarlet border. Disabled is a Greige fill.

**Radio.** Circle. Unchecked is a light Greige border. Checked is an Oxblood dot. Error is a Scarlet border. Disabled is a Greige fill.

## Tags & badges

Severity tags for findings. Chivo Mono, uppercase, small, 0px radius. Two styles: filled and outline.

| Level | Color |
|---|---|
| Critical | Scarlet |
| High | Oxblood |
| Medium | Sage (Pale Olive) |
| Low | Greige |

Filled uses the color as the fill: white label on Scarlet and Oxblood, Oxblood label on Sage and Greige. Outline uses the color as a 1px border with a matching label.

## Interaction states

Every interactive element ships its states. They are not optional polish, and a build that only has a default state is not finished. Pull the states from the component specs above.

| Element | States |
|---|---|
| Nav links | Hover is a 1px underline. The active link is Scarlet. |
| Filled buttons | Darken on hover. |
| Outline button | Fills Oxblood with a white label on hover. |
| Text CTA | Underlines on hover. Disabled is greyed. |
| Inputs | Focus is an Oxblood border. Error is a Scarlet border with a message. |

If nothing changes on hover or focus, it is not done.

---

# Recipes

Per-surface builds. Each names the lead move and the density for that piece. These match the test prompts in tests/prompts.md. Document what you test, test what you document.

## Full landing page
**Lead move:** classical statuary hero + Scarlet mono eyebrow. **Density:** hero breathes (statue, headline in Clash Display, one-line lead, `Get a demo`); nav is Clash Grotesk top-right (Solutions · Industries · Research · Company), with `Get a demo` as a mono text CTA, not a filled button (see Components > Navigation). Down-scroll: alternate White/Rice grounds with a Bark section; big-number motif marks one section; footer on Bark with reversed logo. One hero move per section.

## 4-page deck
**Lead move:** the number motif as running marker (`02.16`…). **Density:** cover = statue + Display headline + logo, sparse; three content pages hold one idea each — a Bark divider page, a stat page using Big Numbers in Scarlet, a body page in Clash Grotesk. Consistent 1px zoning cover-to-content.

## LinkedIn banner
**Lead move:** mark-as-graphic (cropped burst) + wordmark. **Density:** near-empty. Bark or White ground, the eyebrow or the number motif small, logo in the safe area. Carry the brand in a sliver — no paragraph.

## Social post
**Lead move:** one hero statement or the statue. **Density:** near-zero copy — a single Clash Display line or the bust, the mark, and Scarlet as the only accent. Thumb-stop recognition, not information.

## Bus-stop / OOH poster
**Lead move:** statue or oversized ghost mark, one idea. **Density:** minimal — one headline read at distance, the eyebrow, logo, and a Scarlet spark. Bark or White field, huge type, nothing that needs a second read.
