# Changelog — 20260624-1646

Remove Motivation downstream anchor link; show shared input image in HaMeR comparison rows.

## Summary

- Motivation paragraph no longer links to `#downstream-application`, so readers follow Method → Results → Qualitative → HaMeR in order.
- HaMeR comparison matrix rows now display the same input image as ScaleHP (samples 30 and 27).
- Removed unused `.comparison-panel.matrix-empty` CSS rule.

## Files Changed

| File | Lines (approx.) | Intent |
|------|-----------------|--------|
| `index.html` | 191 | Delete trailing sentence with `<a href="#downstream-application">` |
| `index.html` | 638–650, 679–691 | Replace `matrix-empty` with `compare_30/27_input.jpg` in HaMeR rows |
| `static/css/index.css` | 1043–1045 | Remove `.comparison-panel.matrix-empty` |
