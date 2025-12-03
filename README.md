NSCLC Differential Expression Analysis (GSE19188)

A reproducible Python pipeline to download, preprocess, and analyze the GSE19188 gene expression dataset from GEO, identifying tumor and normal differential expression signatures in early-stage NSCLC.

📌 What This Project Does

This pipeline performs:

Automatic download of the GSE19188 dataset directly from NCBI GEO

Cleaning & preprocessing of the expression matrix

Filtering low-variance probes

Log₂ transformation

Sample classification into tumor and normal groups using GEO metadata

Differential expression analysis using Welch’s t-test

Generation of intuitive visualizations, including:

Volcano plot

Heatmap (Top 50 DEGs)

PCA plot

MA plot

This project is designed to be easy to read, easy to run, and easy to extend, especially for students learning transcriptomics or bioinformatics.

🧬 Dataset Information

Dataset: GSE19188

Condition: Early-stage NSCLC with matched normal lung tissue

Source: NCBI Gene Expression Omnibus (GEO)

Storage: Data are downloaded automatically when you run the notebook (no need to store raw files in the repo).

📁 Project Layout
├── notebooks/                     # Main end-to-end analysis notebook
│   └── GSE19188_NSCLC_DE_analysis.ipynb
├── src/                           # Optional helper modules
├── figures/                       # Exported plots (Volcano, PCA, Heatmap, MA)
├── data/                          # Generated DEG tables and processed files
├── requirements.txt               # Python dependencies
└── README.md                      # Project documentation


You may customize or expand this structure for your own workflow.

🚀 Getting Started

1. Clone the repository

git clone https://github.com/NSCLC_GSE19188_DE_analysis.git

cd NSCLC_GSE19188_DE_analysis

2. Create and activate a virtual environment

Mac/Linux:

python -m venv venv

source venv/bin/activate


Windows:

venv\Scripts\activate

3. Install dependencies

pip install -r requirements.txt

4. Open the analysis notebook

You can use Jupyter Notebook, VS Code, or Google Colab:

notebooks/GSE19188_NSCLC_DE_analysis.ipynb

▶️ How to Run the Pipeline

Once the notebook is open, simply run all cells from top to bottom.

The notebook will:

Download and preprocess GSE19188

Define tumor vs. normal sample groups

Perform Welch’s t-test to identify DEGs

Save results into:

figures/ (plots)

data/ (DEG lists, normalized expression tables)

🧠 Methods (Plain Language)

Expression values are log₂-transformed for normalization.

Low-variance probes are removed to focus on informative genes.

GEO metadata is used to label samples as tumor or normal.

For each gene, the workflow computes:

Log₂ fold change

Welch’s t-test p-value

Plots such as volcano, heatmap, PCA, and MA help confirm:

Clear separation of tumor vs. normal groups

Proper normalization

Visualization of major gene expression changes

💡 Why This Project is Useful

A clean starting point for NSCLC or GEO-based gene expression projects

A teaching example for differential expression workflows in Python

A reusable template you can extend with:

Pathway enrichment

Survival analysis

Machine-learning models

Additional GEO datasets

🙏 Acknowledgements

Dataset:
GSE19188 – “Expression data for early-stage NSCLC” (NCBI GEO)

Tools Used:
Python, GEOparse, NumPy, Pandas, SciPy, scikit-learn, Matplotlib, Seaborn
