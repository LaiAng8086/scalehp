# Code Change Log — 20260624-1552

## Summary
Second-round webpage refinements: FreiHand multi-method qualitative comparisons upfront, horizontal HaMeR layout, ablation data tables, and compact spacing.

## Files Changed

| File | Lines (approx.) | Intent |
|------|-----------------|--------|
| `index.html` | 315–360, 407–620 | Ablation cards → HTML tables; FreiHand 3-sample block before in-the-wild; HaMeR 7-column horizontal rows without Sample IDs |
| `static/css/index.css` | 31–390, 820–1060 | Compact spacing; `.freihand-row`, `.comparison-horizontal-row`, `.ablation-table`, subsection styles |
| `static/images/freihand_{0008,0009,0010}_{input,metric,top}.png` | — | Copied 9 FreiHand baseline comparison images from `Comparison/pics/` |

## Key Changes

1. **Qualitative**: Added FreiHand subsection (samples 0010/0009/0008) with Input + multi-method metric/top plots (GT/ScaleHP/HandDGP/CMR legend); in-the-wild block moved below.
2. **HaMeR**: Replaced vertical row layout with horizontal 7-column grid per example; removed "Sample 30/27" headings.
3. **Ablation**: Two side-by-side tables matching paper `tab:Ablation` and `tab:scale_token`.
4. **Spacing**: Reduced body line-height, hero/section padding, grid gaps, and card padding site-wide.
