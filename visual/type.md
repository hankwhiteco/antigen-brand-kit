# Typography

Three families. Clash Display is the headline voice, Clash Grotesk carries body and UI, Chivo Mono handles numbers, eyebrows, labels, and CTAs.

| Role | Typeface | Source | Use for |
|---|---|---|---|
| Display / Headlines | **Clash Display** | Fontshare (licensed, incl. in kit) | Display and H1–H3. **Regular (400)**, **sentence case**, tight. |
| Body / UI | **Clash Grotesk Variable** | Fontshare (licensed, incl. in kit) | Lead, body copy, subheads, navigation, form text. |
| Numbers / Labels | **Chivo Mono** | Google Fonts (OFL) | Big/medium numbers, eyebrows, CTAs, tags, technical labels, usually uppercase, tracked. |

Font files live in [`assets/fonts/`](assets/fonts/): `ClashDisplay_Complete/`, `ClashGrotesk_Complete/`, and `ChivoMono[wght].ttf` (+ italic). Web builds should prefer the `.woff2` files.

```css
--font-display: "Clash Display", system-ui, sans-serif;      /* Regular 400, sentence case, tight */
--font-body:    "Clash Grotesk Variable", system-ui, sans-serif;
--font-mono:    "Chivo Mono", ui-monospace, monospace;        /* uppercase labels, tracked */
```

## Type scale (from the web spec)

| Style | Family | Size / Line-height / Tracking |
|---|---|---|
| Display | Clash Display | 64 / 72 / −1 |
| H1 | Clash Display | 56 / 64 / −0.5 |
| H2 | Clash Display | 40 / 48 / 0 |
| H3 | Clash Display | 32 / 40 / 0 |
| Lead | Clash Grotesk Variable | 24 / 32 / 0 |
| Body Large | Clash Grotesk Variable | 20 / 28 / 0 |
| Body | Clash Grotesk Variable | 16 / 24 / 0 |
| Body Small | Clash Grotesk Variable | 14 / 22 / 0 |
| Big Number | Chivo Mono | 96 / 100 / 0 |
| Medium Number | Chivo Mono | 48 / 56 / 0 |
| Eyebrow | Chivo Mono ExtraLight | 11 / 16 / 0.14em · UPPERCASE |
| CTA | Chivo Mono Regular | 13 / 20 / 0.1em · UPPERCASE |

**Type treatment**
- Headlines: Clash Display **Regular (400)**, **sentence case** (not all-caps), tight tracking, hard scale jumps between Display/H1 and body, don't drift to safe mid-scale sizes.
- Eyebrows & CTAs: Chivo Mono, UPPERCASE, tracked (0.1–0.14em), small; Scarlet for eyebrows.
- Numbers: Chivo Mono, oversized as a device (`02.16` / `0216`).
- Body: Clash Grotesk Variable, generous line-height (~1.5), left-aligned, never centered.
