# Code Change Log — 20260621-1600

## Summary
Implemented ScaleHP project webpage by replacing Academic Project Page template placeholders with paper content, figures, and PDFs sourced from the ECCV LaTeX repository.

## Files Changed

| File | Lines (approx.) | Intent |
|------|-----------------|--------|
| `index.html` | 1–520 | Full page rewrite: hero metadata, abstract, motivation, contributions, method, results, qualitative/comparison carousels, summary, BibTeX |
| `static/css/index.css` | 735–850 | Added styles for teaser image, contribution/method/ablation cards, stat cards, results table, comparison grid |
| `static/images/*` | — | Copied/converted teaser, pipeline, qualitative, FreiHand, and HaMeR comparison images |
| `static/pdfs/paper.pdf` | — | Copied from `main_compressed.pdf` |
| `static/pdfs/supplementary.pdf` | — | Copied from `Supple/main.pdf` |

## Asset Sources
- Paper root: `/comp_robot/jingruitao/eccv2026/_arxiv_ScaleHP_Estimating_Hand_Pose_in_Metric_Space/`
- Key figures: `teaser.pdf`, `pipeline2.png`, `visual7/`, `Comparison/pics/`, `Supple/output_scalehp3/`, `Supple/output_hamer/`

## Removed Template Sections
- More Works dropdown, YouTube embed, video carousel, poster iframe, placeholder Code/arXiv links
