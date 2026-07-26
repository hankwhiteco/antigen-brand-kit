# Color

Four solid colors plus two texture treatments. The palette is warm and earthy — a brown-black stands in for black, Scarlet is the only bright, Sage and Greige are quiet secondaries.

| Token | Name | HEX | RGB | Role |
|---|---|---|---|---|
| `--bark` / `--oxblood` | Bark / Oxblood | `#291B14` | 41, 27, 20 | Primary dark — **in place of black.** "Bark" for large panels/blocks; "Oxblood" for text, UI default, and dividers. Same value, two role-names. |
| `--scarlet` | Scarlet | `#D23737` | 210, 55, 55 | The only accent — active states, big numbers, the eyebrow, one graphic mark. A spark, never a wash. |
| `--sage` | Sage / Pale Olive | `#D2D297` | 210, 210, 151 | Secondary — sage blocks, edge panels, "Pale Olive" button fill. |
| `--greige` | Warm Greige | `#D4D1D0` | 212, 209, 208 | Warm light neutral — greige blocks, hairline dividers, quiet surfaces. |
| `--white` | White | `#FFFFFF` | 255, 255, 255 | Clean ground and text on Bark. |

```css
:root {
  --bark:    #291B14; /* a.k.a. --oxblood */
  --oxblood: #291B14;
  --scarlet: #D23737;
  --sage:    #D2D297;
  --greige:  #D4D1D0;
  --white:   #FFFFFF;
}
```

**Rice & Pattern (textures, not colors).** *Rice* is a subtle rice-paper / crackle texture over a warm off-white ground; *Pattern* is an organic leaf motif in Greige. They dress light surfaces — see the texture move in [`creative-direction.md`](creative-direction.md). Treat them as surfaces, not palette tokens.

*Print (CMYK/Pantone) values are not defined in the brand guide — flag to the brand owner before any print run.*

## Usage & pairings
- **Grounds:** White or the Rice texture for content-heavy surfaces; **Bark** for anchor panels and dark sections.
- **Text on light** (White/Rice/Greige): Bark (Oxblood).
- **Text on dark** (Bark): White or Greige.
- **Accent:** Scarlet for the eyebrow, big numbers, active/hover states, and a single graphic mark per surface. Never a large Scarlet background wash.
- **Sage:** secondary blocks and edge panels; Pale Olive as a button fill.
- **Ratio guide:** ~60% White/Rice ground · ~30% Bark + Greige/Sage · ~10% Scarlet spark.
