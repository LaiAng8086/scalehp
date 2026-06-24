# Changelog — 20260624-1721

Fix GitHub push rejection caused by 150 MB `supplementary.pdf` in git history.

## Summary

- GitHub rejected push: `static/pdfs/supplementary.pdf` (149.85 MB) exceeds 100 MB limit.
- Rebuilt local history on top of `origin/main` as a single clean commit without any PDF under `static/pdfs/`.
- Fixed malformed `.gitignore` (`static/pdfs/*static/pdfs/` → `static/pdfs/`).
- PDFs remain on disk locally for deployment but are not tracked by git.

## Files Changed

| File | Intent |
|------|--------|
| `.gitignore` | Ignore entire `static/pdfs/` directory |
| Git history | Squashed 5 local commits into `b02ae31` without large blobs |

## User action required

Run push locally (credentials required):

```bash
cd /comp_robot/jingruitao/display_webpages/scalehp
git push origin main
```

Optional: host `supplementary.pdf` on arXiv/Google Drive and link from the webpage if needed.
