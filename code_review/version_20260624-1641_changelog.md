# Changelog — 20260624-1641

Fix layout uniformity, author superscript visibility, and HaMeR comparison matrix.

## Summary

- Restored visible author affiliation superscripts via merged `author-meta` tags and stronger CSS styling.
- Unified qualitative/comparison image sizing with `panel-img-wrap` (1:1 aspect ratio, `object-fit: contain`).
- Rebuilt HaMeR section as 4-column × 2-row matrix (views as columns, methods as rows); widened container to full `container`.
- Replaced 768px vertical stack with horizontal scroll on narrow screens.

## Files Changed

| File | Lines (approx.) | Intent |
|------|-----------------|--------|
| `index.html` | 126–131 | Author block: single merged `<sup class="author-meta">` per author |
| `index.html` | 446–600 | FreiHand + in-the-wild: `panel-img-wrap`, `qualitative-scroll` wrappers |
| `index.html` | 601–695 | HaMeR: `comparison-matrix` (header + ScaleHP/HaMeR rows), `container` width |
| `static/css/index.css` | 208–218 | `.author-meta` superscript styling (primary color, larger, vertical-align) |
| `static/css/index.css` | 890–970 | `.panel-img-wrap`, `.qualitative-scroll`, compact qualitative grid |
| `static/css/index.css` | 960–1054 | `.comparison-matrix`, matrix header/row/method labels |
| `static/css/index.css` | 1068–1076 | Removed 768px 2-column stack for qualitative/comparison rows |

## Functions / Selectors

- **CSS**: `.author-meta`, `.panel-img-wrap`, `.qualitative-scroll`, `.comparison-matrix`, `.comparison-matrix-header`, `.comparison-matrix-row`, `.matrix-method`, `.matrix-label`
- **Removed usage**: `.affiliation-mark`, `.comparison-horizontal-row`, `.comparison-horizontal-panel`
