# Code Change Log — 20260624-1528

## Summary
Implemented four webpage refinements: author affiliation superscripts, aligned-metrics results table, paper-style static qualitative/HaMeR grids (replacing carousels), and retargeting-first downstream narrative.

## Files Changed

| File | Lines (approx.) | Intent |
|------|-----------------|--------|
| `index.html` | 87–106, 122–141, 190, 311–360, 405–520, 548–610 | Author superscripts + affiliation list; JSON-LD all 6 authors; aligned SOTA table; static qualitative/HaMeR grids; downstream retargeting requirements first |
| `static/css/index.css` | 203–230, 830–980 | Affiliation styling; scrollable aligned table; qualitative/comparison grid layouts; downstream-needs block |
| `static/js/index.js` | 135 | Limit Bulma carousel to `#demo-carousel` only |
| `static/images/qualitative_{1-4}_{input,metric,front,top}.*` | — | Copied 16 in-the-wild multi-view assets from paper `visual7/` |
| `static/images/compare_{30,27}_{scalehp,hamer}_{metric,front,top}.png` | — | Copied 12 HaMeR comparison view assets from paper `Supple/` |

## Key Changes

1. **Authors**: Each author now has numbered affiliation superscripts matching `main.tex`; institutions listed as numbered lines below.
2. **Results**: Added full Table `tab:aligned` (20 methods × 5 metric columns) with horizontal scroll on narrow screens.
3. **Qualitative / HaMeR**: Removed `#qualitative-carousel` and `#comparison-carousel`; replaced with static 4-column and row×column grids mirroring paper figures.
4. **Downstream**: New `.downstream-needs` section describing retargeting requirements before ScaleHP benefit cards; reordered cards with Reliable Retargeting first.
