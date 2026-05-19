# AI-physics Wind Forecast Figures

This folder contains Jupyter notebooks, data, and outputs used to generate figures for an AI-based wind forecast study. Notebooks are grouped by figure in the top-level folders (`Fig1`, `Fig2`, …) and use the corresponding `data/` subfolders.

**Overview**

- **What:** Notebooks and data for figures used in the manuscript and supplementary materials.
- **Where:** Figures are organized by folder: Fig1, Fig2, Fig3, Fig4, Fig5, Fig6, Supplementary.
- **Date:** Packaged May 19, 2026.

**Repository structure (high-level)**

- Fig1/ — notebooks and `data/` for Figure 1
- Fig2/ — notebooks and `data/` for Figure 2
- Fig3/ — notebooks and `data/` for Figure 3
- Fig4/ — notebooks and `data/` for Figure 4
- Fig5/ — notebooks and `data/` for Figure 5
- Fig6/ — notebooks and `data/` for Figure 6
- Supplementary/ — additional notebooks and resources

Each `FigX/data/` directory contains the raw or preprocessed files used by the notebooks in that figure folder.

**How to run the notebooks**

Create an environment

Conda (recommended)

```bash
conda env create -f environment.yml
conda activate ai-wind-figs
```

Run notebooks in order; they expect data files to be present in the `data/` subfolders of each figure folder.

**Notes & recommendations**

- Some notebooks read large NetCDF files (e.g., `uv10_d05_*.nc`). Ensure you have sufficient memory and disk space.
- An `environment.yml` and `requirements.txt` are included in this folder for convenience. For publication, pin exact package versions (e.g., `package==x.y.z`).
- If you plan to publish this repository, add a `LICENSE` and update this `README.md` with citation text.

**Files added**

- `requirements.txt` — minimal pip install list
- `environment.yml` — conda environment spec (uses `conda-forge` channel)

