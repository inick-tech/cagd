# Data-Driven Geometric Design for Marketing & Consumer Experience

**MAT516/4 · Curve and Surface Methods for CAGD · Assignment 1**
Universiti Sains Malaysia — School of Mathematical Sciences · June 2026

---

## Overview

This repository contains the submission for Assignment 1 of MAT516/4 (Curve and Surface Methods for CAGD), a coursework requirement at Universiti Sains Malaysia.

The work proposes a computational pipeline that connects unstructured customer language to parametric 3D product geometry. Using the Coca-Cola bottle as a benchmark, it demonstrates how natural language processing can drive continuous optimisation of B-spline control points — bridging the gap between consumer voice and surface design.

The pipeline runs end-to-end across six stages:

1. **Customer Review Corpus** — 50 synthetic reviews annotated along three perceptual axes: Sleekness, Roundness, and Compactness
2. **BERT Encoder** — each review is encoded into a 768-dimensional embedding; the corpus-level preference vector is the mean of all embeddings
3. **Design Dimension Scores** — the preference vector is projected to three scalar scores via a learned linear mapping and sigmoid activation
4. **MLP Decoder** — a semantic modulation matrix maps design scores to signed radial deltas on nine B-spline control points
5. **B-Spline Surface** — a cubic B-spline profile is evaluated and revolved to produce the full 3D CAGD surface
6. **Joint Loss Function** — training optimises simultaneously for preference alignment, surface fairness, and control net regularity

---

## Repository Contents

| File | Description |
|------|-------------|
| `index.html` | Full assignment write-up as a formatted web page |
| `*.ipynb` | Jupyter notebook with complete Python implementation (all six pipeline stages) |

---

## Live Preview

The assignment is viewable online at:

**[https://inick-tech.github.io/cagd/](https://inick-tech.github.io/cagd/)**

---

## Author

**Mohammad (Nick) Nikbakht**
Pusat Pengajian Sains Matematik · Universiti Sains Malaysia
