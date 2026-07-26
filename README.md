# Antigen Brand Kit

Everything needed to build on-brand Antigen materials — landing pages, decks, one-pagers,
social, email. Hand this whole folder to a designer, or drop it into an AI coding tool
(Cursor, Claude Code, Windsurf, v0, etc.) and start building.

## Quick start

**Using an AI tool (Cursor / Claude Code / etc.):**
1. Open this folder as your project / workspace.
2. The tool auto-reads [`AGENTS.md`](AGENTS.md) — a router that points at the specs below.
3. Prompt it: *"Build me a [landing page / pitch deck / one-pager / email] for Antigen."*

**Working by hand:** open the file that owns the decision you're making (see the map below).

## Layout

```
antigen-brand-kit/
├── AGENTS.md               ← router for AI tools: which file owns what
├── README.md               ← you are here
├── CHANGELOG.md            ← history of changes to the kit
├── verbal/
│   ├── positioning.md      → who Antigen is, category, audience, contact
│   ├── messaging.md        → voice, tone, hero lines, CTA, writing rules
│   └── naming.md           → product & mark names, taglines, master line
├── visual/
│   ├── creative-direction.md → the visual system, its intent, + build recipes
│   ├── color.md            → color tokens, hex/RGB, pairings
│   ├── type.md             → typefaces, scale, type treatment
│   ├── logo.md             → logo variants, selection rules, clear space
│   └── assets/
│       ├── logos/svg/ + png/ → all lockups, marks, avatars
│       ├── imagery/        → brand guide + design-system PDFs
│       └── fonts/          → Clash Display, Clash Grotesk, Chivo Mono
├── examples/
│   ├── good/               → finished reference builds + exports
│   └── wrong/              → what to avoid
└── tests/
    └── prompts.md          → prompt tests
```

## The 30-second brand

- **Verbal:** technical, precise, adversarial-but-trusted. Sentence-case headlines; mono uppercase
  labels. *"Accelerating enterprise defense at agentspeed."* See [`verbal/`](verbal/).
- **Visual:** warm, earthy, editorial. Bark brown-black, one Scarlet spark, Sage/Greige secondaries;
  Clash Display + Clash Grotesk + Chivo Mono; black-and-white classical statuary, rice-paper texture,
  the burst mark, and the `02.16` number motif. See [`visual/`](visual/).

Full detail — and the *why* behind each rule — lives in the files above.

---
Contact: Antigen — antigen.sh
