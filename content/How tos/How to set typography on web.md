---
Tags:
  - "#web"
  - design
  - "#development"
draft: false
Date:
---

## How to set typography on web

### Text
- Line length: CSS property - max-width: 66ch
- Line height: 1.4 - 1.6
    - line height units;  
        `p { margin-block: 1lh; }`
- Smoothing: `-webkit-font-smoothing: antialiased` and `-moz-osx-font-smoothing: grayscale`.
- Reduce font weights on dark mode
- Wrapping
    - Headings - Use `text-wrap: balance` for headlines to make them feel, well, more balanced.
    - Body - use `text-wrap: pretty`
    - `hanging-punctuation` property

### Numbers
- Tabular figures makes numerical figures all take up the same width.
- Old style figures (editorial type) with `font-feature-settings: "onum"` or `font-variant-numeric: oldstyle-nums`.
- Tables: right align + tabulise them for easy comparison

### Fitting type
- `clamp()` lets type [interpolate](https://www.interfacecraft.dev/library/interpolation-and-map-range) smoothly between a floor and a ceiling. In `clamp(1.375rem, 6cqi, 2.75rem)`
- deliberate clipping
    - A single line takes `text-overflow: ellipsis`
    - a longer description clamps to a fixed number of lines with `-webkit-line-clamp`
- [Open type features](https://pangrampangram.com/blogs/journal/opentype-features)
    - font-feature-settings and font-variantf


## References