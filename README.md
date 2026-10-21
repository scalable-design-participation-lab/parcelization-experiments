# parcelization-experiments

Experiments on segmenting city blocks from building footprint data.

Each experiment is one folder or file set named `YYYY_MM_DD_topic`, dated by the day the
experiment ran. The `.qmd` is the source. The `.html` next to it is the rendered report.

| Experiment | Report | What it does |
|---|---|---|
| `2026_09_22_block_marching_squares_raw` | [Read it](https://scalable-design-participation-lab.github.io/parcelization-experiments/2026_09_22_block_marching_squares_raw.html) | Compares marching squares over building footprints against momepy's enclosed tessellation, for Boston, Charlotte, Pittsburgh and Manhattan. Scores the two with average IoU, panoptic quality and boundary F-score. |

## Running the notebooks

The notebooks read building footprints from the *Million Neighborhoods* shared drive and import
three modules that are not in this repository yet: `footprint_rasterize`, `marching_squares` and
`footprint_metrics`. Paths are absolute, so the notebooks render only on the author's machine
for now.

## Published reports

`docs/` is the GitHub Pages root. It holds the rendered reports and their figures, and nothing else.
The `.qmd` sources stay in `notebooks/` and are not served.

Site: https://scalable-design-participation-lab.github.io/parcelization-experiments/
