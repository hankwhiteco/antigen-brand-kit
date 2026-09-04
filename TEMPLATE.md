# Template layer

Antigen is the worked example. This kit doubles as the **template** for future brand kits.
When Antigen is complete and tested, the brand layer is stripped and re-filled per brand.

Two layers live in this repo:

- **Layer A, Template (reusable):** structure, process, and craft rules that carry to every kit unchanged.
- **Layer B, Brand (Antigen):** tokens, assets, voice, and brand-specific moves. Stripped and re-filled per brand.

## Tagging convention

- Brand-specific rules and blocks are marked inline with `<!-- [B] -->`; reusable ones with `<!-- [A] -->` where a file is mixed.
- Defaults when untagged: token and asset files are Layer B wholesale; craft-rule prose is Layer A.
- This file is the source of truth. If an inline tag and the map below disagree, the map wins.
- Rule of thumb when writing a rule: state the craft, not the brand value. "The accent touches imagery, never type" is Layer A. "Scarlet touches imagery" is Layer B.

## Layer map

| File / section | Layer | On strip |
|---|---|---|
| `AGENTS.md` router structure | A | keep; swap the brand name and one-line pitch |
| `AGENTS.md` Antigen name / tagline | B | replace with placeholder |
| `verbal/positioning.md`, `messaging.md`, `naming.md` | B | blank to TODO templates |
| `visual/color.md` token table + CSS scaffold | A | keep the format |
| `visual/color.md` hex values, Rice/Pattern, spacing scale | B | replace with named placeholders (`--accent`, `--dark`, `--light`, `--neutral`) |
| `visual/type.md` roles + scale format | A | keep |
| `visual/type.md` Clash/Chivo families + sources | B | swap families, keep the scale |
| `visual/logo.md` | B | replace mark + variants; keep the selection-rule format |
| `creative-direction.md` → Default corrections, Copy, Interaction states | A | keep unchanged (shared Bolster asset) |
| `creative-direction.md` → Composition (framed grid, one-texture, column headings, contained collage, asymmetry) | A | keep (craft) |
| `creative-direction.md` → Restraint | A | keep (craft) |
| `creative-direction.md` → Moves (Classical statuary, number motif `0216`, Scarlet eyebrow, edge panels, textures, mark-as-graphic) | B | replace with the new brand's moves; keep the "name / maneuver / intent" format |
| `creative-direction.md` → Failure modes | B | reset (fills per brand as testing surfaces repeats) |
| `creative-direction.md` → Components (nav, buttons, forms, tags, spacing) | A format / B values | keep specs, swap values |
| `creative-direction.md` → Recipes | A surface list + density format / B which moves | keep skeletons, re-point the moves |
| `visual/assets/**` (fonts, logos, imagery, motion) | B | empty; keep a manifest of required slots |
| `examples/good/`, `examples/wrong/` | B | replace with the new brand's examples |
| `tests/prompts.md` | A | keep (the five surfaces are universal) |
| Built comps (`landing/`, `deck/`, ...) | A layout / B skin | keep the layouts as de-branded templates; rebuild the skin per brand |
| `TEMPLATE.md` (this file) | A | keep |

## Strip-to-clean-slate TODO

- [ ] Replace color hexes with named placeholders (`--accent`, `--dark`, `--light`, `--neutral`, `--ground`) in `color.md` and every build.
- [ ] Swap type families (Clash / Chivo) for placeholder font variables; keep the scale untouched.
- [ ] Remove logo/mark SVGs; leave a mark spec and an inline-symbol slot.
- [ ] Empty `visual/assets/{fonts,logos,imagery,motion}`; leave a manifest of required slots and sizes.
- [ ] Blank `verbal/*` to TODO templates (positioning, messaging, naming).
- [ ] Rewrite `creative-direction.md` → Moves for the new brand; keep the section and format.
- [ ] Reset `creative-direction.md` → Failure modes (empty, with the fill-as-you-test note).
- [ ] Repoint Recipes' lead moves; keep the surface list and density format.
- [ ] Swap component-spec values (colors, radii, weights); keep the specs.
- [ ] Replace `examples/good/` and `examples/wrong/`.
- [ ] De-brand the built comps or rebuild their skin; keep the layouts.
- [ ] Leave untouched: Default corrections, Copy reset, Interaction states, Composition + Restraint craft rules, `tests/prompts.md`, the `AGENTS.md` router, this file.

## Running notes

<!-- Log template-level decisions and anything discovered while building Antigen that should shape the template. -->

- The frame grid (light-grey lines + gutter), contained collage, one-texture-per-stretch, mono-or-not nav, and "column headings near body" are craft rules (Layer A). The *values* they reference (Greige, Scarlet, Chivo) are Layer B.
