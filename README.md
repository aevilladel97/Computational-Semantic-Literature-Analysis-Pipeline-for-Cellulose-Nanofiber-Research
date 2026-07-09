# Computational Semantic Literature Analysis Pipeline for Cellulose Nanofiber Research

[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](LICENSE)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.xxxxxxx.svg)](https://doi.org/10.5281/zenodo.xxxxxxx)

---

## Overview

This repository contains the complete computational workflow developed for the semantic analysis of scientific literature on cellulose nanofibers (CNFs).

The pipeline retrieves bibliographic records directly from a Zotero library using the Zotero Web API and performs Natural Language Processing (NLP), semantic embedding generation, topic modeling, clustering, sentiment analysis, computational methodological rigor assessment, and publication-quality visualization.

The workflow was developed as part of the doctoral research conducted at the LEPAMAP–PRODIS Research Group, Universitat de Girona.

---

## Main Features

The workflow includes:

- Automated literature retrieval from Zotero using the Web API
- Duplicate detection and metadata preprocessing
- Benchmarking of multiple sentence embedding models
- BERTopic topic modeling
- UMAP dimensionality reduction
- HDBSCAN clustering
- Semantic topic labeling
- DistilBERT multilingual sentiment analysis
- Computational methodological rigor assessment using rule-based indicators
- Publication-quality figures
- Automatic export of tables, figures and summary metrics

---

## Computational Workflow

The pipeline follows the sequence below:

1. Connect to a Zotero library through the Zotero Web API.
2. Retrieve all bibliographic records.
3. Clean and preprocess metadata.
4. Remove duplicated records.
5. Generate semantic embeddings.
6. Benchmark embedding models.
7. Reduce dimensionality using UMAP.
8. Cluster documents using HDBSCAN.
9. Generate semantic topics with BERTopic.
10. Perform multilingual sentiment analysis.
11. Compute methodological rigor scores.
12. Produce publication-ready figures.
13. Export all outputs as CSV files, publication figures and a ZIP archive.

---

## Execution Environment

This notebook is designed **exclusively for Google Colab**.

No local installation is required.

All Python dependencies are automatically installed during the first execution cells of the notebook.

Although a `requirements.txt` file is provided for documentation and reproducibility, it is **not required** when running the notebook in Google Colab.

---

## Requirements

Google Colab

Python 3.12+

Internet connection

A Zotero account with:

- User ID
- Private API Key

---

## Repository Structure

```text
.
├── Review_CNF_PhD.ipynb
├── README.md
├── LICENSE
├── NOTICE
├── CITATION.cff
├── requirements.txt
├── .gitignore
└── outputs/
```

---

## Running the Notebook

1. Open the notebook in Google Colab.

2. Execute the installation cells.

3. When prompted, provide:

- Zotero User ID
- Zotero API Key

4. Execute all remaining cells.

The pipeline automatically retrieves the literature, performs the complete analysis and exports all results.

---

## Outputs

The notebook automatically generates:

### Topic Modeling

- BERTopic model
- Topic labels
- Topic coherence metrics
- Topic diversity

### Semantic Analysis

- UMAP projections
- Inter-topic similarity
- Hierarchical topic clustering

### Sentiment Analysis

- Positive / Neutral / Negative classification
- Class-level statistics
- Topic-level sentiment summaries

### Computational Rigor Assessment

- Rigor scores
- Topic-level rigor
- Rigor heatmaps
- Class comparisons

### Exported Files

CSV tables

Publication-quality PNG figures

Summary metrics

ZIP archive containing all generated outputs

---

## Input Data

The pipeline retrieves bibliographic records directly from a Zotero library through the Zotero Web API.

No RIS or BibTeX files are required.

The notebook expects valid Zotero credentials provided by the user during execution.

---

## Software Components

Main libraries include:

- BERTopic
- Sentence Transformers
- Transformers
- PyTorch
- UMAP-learn
- HDBSCAN
- Scikit-learn
- Plotly
- Matplotlib
- pandas
- NumPy
- pyzotero

Complete dependency versions are listed in `requirements.txt`.

---

## Reproducibility

The repository contains:

- Complete source code
- Exact dependency versions
- License information
- Citation metadata

The notebook is intended to provide a fully reproducible computational workflow when executed under Google Colab.

Because external machine learning models and the Zotero Web API may evolve over time, minor differences in numerical results may occur.

---

## License

This software is distributed under the GNU Affero General Public License v3.0 (AGPL-3.0-or-later).

See the `LICENSE` file for details.

---

## Citation

If you use this software in academic work, please cite the corresponding Zenodo software release.

Example:

Villadiego del Villar, A. E.

Computational Semantic Literature Analysis Pipeline for Cellulose Nanofiber Research.

Version 1.0.0.

Zenodo.

https://doi.org/10.5281/zenodo.xxxxxxx

---

## Author

**Alfredo Enrique Villadiego del Villar**

PhD Candidate (2025 IFUdG Doctoral Programme)

LEPAMAP–PRODIS Research Group

Universitat de Girona

Campus Montilivi

17003 Girona

Spain

Email:

alfredo.villadiego@udg.edu

---

## Repository

GitHub:
https://github.com/aevilladel97/Computational-Semantic-Literature-Analysis-Pipeline-for-Cellulose-Nanofiber-Research

Zenodo:

https://doi.org/10.5281/zenodo.xxxxxxx
