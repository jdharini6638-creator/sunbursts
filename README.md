# Metabolite–ChEMBL sunburst charts

Interactive sunburst charts showing metabolite to ChEMBL compound relationships for two targets, HTR2A and SLC18A2.

**Live page:** https://jdharini6638-creator.github.io/sunbursts/

## What's in it

| Chart | Target | Descriptor space |
| --- | --- | --- |
| 1 | HTR2A | 2D |
| 2 | HTR2A | 3D |
| 3 | SLC18A2 | 2D and 3D together |

Each ring moves one level down the hierarchy: target, then metabolite, then the ChEMBL compounds mapped to it. Wedge size is the number of compounds.

## How to read it

- Click a wedge to zoom into that branch.
- Click the centre circle to step back out.
- Hover a wedge for its label, count, parent and ID.

## Data and Method

- **Metabolite source:** IMPPAT
- **Target prediction:** SwissTargetPrediction
- **Metabolites:** SMILES representations of the selected metabolites were submitted to SwissTargetPrediction.
- **Targets examined:** HTR2A and SLC18A2
- **Similarity data:** The structurally similar 2D and 3D compounds associated with these targets were explored through the SwissTargetPrediction results.
- **ChEMBL data:** The corresponding ChEMBL compound IDs were collected and used to construct the interactive sunburst charts.

## Files

- `index.html` — all three charts in one self-contained page. Plotly.js is embedded, so it opens offline with no dependencies. About 4 MB, give it a few seconds on a slow connection.
