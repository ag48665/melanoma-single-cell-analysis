# Melanoma Single-Cell RNA-seq Analysis

Single-cell transcriptomic analysis of the melanoma tumour microenvironment using **Python**, **Scanpy**, and unsupervised clustering.

This project investigates:

- T-cell exhaustion states
- Tumour heterogeneity
- Melanoma lineage programs
- Proliferative tumour subpopulations
- Stress / plasticity signatures

---

# Project Overview

Melanoma contains diverse tumour and immune cell states that influence progression and therapy response.  
Using publicly available single-cell RNA-seq data, I built an end-to-end analysis pipeline to identify biologically meaningful cell populations and transcriptional programs.

---

# Main Results

## 1. Tumour Microenvironment Mapping

Unsupervised clustering identified multiple cell populations:

- T cells
- B cells
- NK cells
- Macrophages
- Endothelial cells
- CAFs
- Tumour cells

Using UMAP visualization and marker-based annotation.

---

## 2. T-cell Exhaustion Analysis

A custom exhaustion score was computed using canonical checkpoint genes:

- PDCD1
- LAG3
- TOX
- TIGIT
- HAVCR2
- CTLA4

This revealed heterogeneous T-cell functional states, with subclusters showing elevated exhaustion signatures.

---

## 3. Tumour Heterogeneity Analysis

Tumour cells were refined using melanoma lineage markers:

- PMEL
- TYR
- DCT
- MITF

Distinct tumour programs were observed:

### Melanocytic State
High expression of:

- PMEL
- TYR
- DCT

### Proliferative State
Subset enriched for:

- PCNA

### Stress / Signaling State
Variable:

- FOS

### Plastic / Dedifferentiated Tendency
Partial expression of:

- VIM

---

# Tools & Libraries

- Python
- Scanpy
- Pandas
- NumPy
- Matplotlib
- Jupyter Lab

---

# Workflow

1. Load scRNA-seq matrix  
2. Create AnnData object  
3. Metadata annotation  
4. Normalization & log transform  
5. Highly variable genes  
6. PCA  
7. Nearest-neighbor graph  
8. UMAP embedding  
9. Leiden clustering  
10. Marker gene analysis  
11. Signature scoring  
12. Biological interpretation

---

# Repository Structure

```text
melanoma-single-cell-analysis/
│── notebooks/
│   ├── 01_start.ipynb
│   └── 02_melanoma_project.ipynb
│
│── figures/
│   ├── umap_celltypes.png
│   ├── tcell_exhaustion.png
│   ├── tumor_states.png
│
│── data/
│   └── metadata / processed input files
│
└── README.md

---


# Figures
Global UMAP

Cell populations across the melanoma microenvironment.

T-cell Exhaustion Score

Spatial distribution of exhausted T-cell states.

Tumour Programs

Differentiated vs proliferative vs plastic melanoma states.

# Skills Demonstrated
Single-cell RNA-seq analysis
Cancer bioinformatics
Transcriptomics
Data visualization
Biological interpretation
Reproducible research workflows
Python for life sciences
Future Extensions
Pseudotime trajectory analysis
Cell-cell communication (CellChat / CellPhoneDB)
Differential expression by patient
Survival-associated signatures
Multi-omics integration

# Author
Independent computational biology project developed to build research-ready skills in cancer genomics and single-cell analysis.
