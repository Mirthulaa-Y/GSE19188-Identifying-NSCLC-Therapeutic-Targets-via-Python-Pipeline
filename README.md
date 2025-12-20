Gene-Level Differential Expression Analysis of NSCLC (GSE19188)

This repository contains a Python-based bioinformatics workflow for gene-level differential expression and pathway analysis of non-small cell lung cancer (NSCLC) using the public GEO microarray dataset GSE19188.

The project focuses on identifying transcriptomic differences between NSCLC tumor samples and normal lung tissues through statistically rigorous analysis and biological interpretation.

📌 Background

Non-small cell lung cancer accounts for the majority of lung cancer cases and is characterized by extensive molecular heterogeneity. Transcriptomic profiling enables systematic identification of genes and pathways associated with tumor development and progression.

Public repositories such as the NCBI Gene Expression Omnibus (GEO) provide access to large-scale expression datasets that can be reanalyzed to extract biologically meaningful insights using reproducible computational workflows.

🎯 Objectives

Perform gene-level differential expression analysis between NSCLC tumor and normal lung tissues

Identify significantly upregulated and downregulated genes with false discovery rate (FDR) correction

Explore global transcriptomic patterns using dimensionality reduction and clustering

Interpret results through functional pathway enrichment analysis

🧪 Dataset

Source: NCBI Gene Expression Omnibus (GEO)

Accession: GSE19188

Platform: Affymetrix microarray

Data type: Pre-normalized gene expression data

All data used in this project are publicly available.

🔬 Analysis Workflow

The analysis pipeline includes the following steps:

Retrieval of expression data using GEOparse

Probe-to-gene mapping using platform annotations

Construction of gene-level expression matrices

Low-variance gene filtering to reduce noise

Differential expression analysis using Welch’s t-test

Multiple testing correction using Benjamini–Hochberg FDR

Exploratory data analysis (PCA, heatmap, volcano plot, MA plot)

Functional pathway enrichment analysis (KEGG)

📊 Key Results

Identification of 159 significantly differentially expressed genes

Clear transcriptomic separation between tumor and normal samples observed in PCA

Consistent expression patterns across top DEGs in hierarchical clustering

Enrichment of cancer-associated pathways, particularly those related to cell cycle regulation

🛠 Tools & Libraries

Python

Pandas, NumPy

GEOparse

gseapy

Matplotlib / Seaborn

📁 Repository Structure
.
├── analysis_script.py
├── README.md
└── results/
    └── figures/


(File names may vary depending on implementation)

📚 Purpose & Scope

This project was conducted as an academic learning and research exercise to strengthen skills in:

transcriptomic data analysis

statistical evaluation of high-dimensional biological data

reproducible bioinformatics workflows

The findings are intended for educational and research purposes and do not represent clinical or therapeutic validation.



