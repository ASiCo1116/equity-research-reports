# equity-research-reports

GitHub Pages source for AI-generated equity research reports.

**This repo is generated** by `pixi run build-site` in the sibling
`equity-research-agent` repo. Do not edit files here by hand — re-run the
build script to refresh.

## Contents

- `index.html` — root landing page with per-ticker cards + disclaimer
- `assets/style.css` — shared styling
- `<TICKER>/index.html` — per-ticker report list
- `<TICKER>/<TICKER>-<DATE>.html` — individual self-contained reports

Each report's metadata (rating, target price, potential return) is parsed
from the embedded `<script id="report-metadata">` JSON block.

## Disclaimer

All reports are AI-generated and **do not constitute investment advice**.
See the disclaimer at the top of `index.html` and the bottom of each report
for full details.

## Rebuild

In the sibling repo:

```
pixi run build-site
```

That writes everything under this directory (overwriting in place).
