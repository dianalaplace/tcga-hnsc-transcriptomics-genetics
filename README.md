# tcga-hnsc-transcriptomics-genetics

> Bulk RNA-seq transcriptomics and somatic variant analysis of TCGA-HNSC (Head and Neck Squamous Cell Carcinoma).

## Overview

This project performs integrated transcriptomic and genetic analysis on the TCGA-HNSC cohort using data from UCSC Xena. The analysis covers dimensionality reduction, unsupervised clustering, differential expression, and VCF variant filtering to characterize tumor heterogeneity and the somatic genetic landscape in head and neck squamous cell carcinoma.

## Dataset

| Source | Data type |
|--------|-----------|
| [UCSC Xena / TCGA-HNSC](https://xenabrowser.net/) | Bulk RNA-seq gene expression |
| TCGA-HNSC VCF | Somatic variant calls |

## Analysis

Transcriptomics:
- PCA and UMAP dimensionality reduction
- Hierarchical clustering (silhouette score optimization)
- Differential expression analysis (t-test + Benjamini-Hochberg correction)

Genetics:
- VCF filtering: chromosome 6, PASS variants, ALT = T

## Requirements

pip install numpy pandas matplotlib seaborn scikit-learn scipy statsmodels umap-learn

## Repository Structure

tcga-hnsc-transcriptomics-genetics/
├── data/              Input expression and VCF data
├── figures/           Output plots and visualizations
├── notebooks/
│   └── 01_setup.ipynb Main analysis notebook
└── 01_setup.ipynb

## Status

Analysis complete (January 2026).
