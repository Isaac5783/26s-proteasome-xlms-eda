# 26S Proteasome XL-MS EDA

Exploratory data analysis of a cross-linking mass spectrometry (XL-MS) dataset from the Rappsilber Lab.

The project uses a CSM-level xiFDR result from a 26S proteasome dataset and focuses on understanding the structure and characteristics of XL-MS identification data before applying further analysis.

## Dataset

The analysis currently focuses on one CSM-level xiFDR result file from the dataset:

* **1,035 CSMs**
* **59 columns**
* Crosslinker: **BS3**
* Charge states: **3–8**

The dataset contains information about:

* Experimental MS/MS spectra
* Precursor mass and charge
* Crosslinked peptide pairs
* Protein identifiers
* Crosslink positions
* Fragment evidence
* Match scores
* Target/decoy classification
* FDR estimates
* Peptide-pair, link, and protein-interaction identifiers

## Current Analysis

The notebook currently covers:

* Dataset structure and terminology
* Column inspection and data types
* Missing-value investigation
* Target/decoy composition
* Charge-state distribution
* Peptide-length statistics
* Fragment-evidence statistics
* Initial visualizations

Some metadata fields, particularly `Name1`, contain substantial missing or incomplete values. These fields are being documented rather than modified during the initial analysis.

## Project Structure

```text
eda_on_26s_proteasome/
├── data/
│   └── 26S/
├── .venv/
├── README.md
└── Untitled.ipynb
```

The raw dataset is kept separate from the analysis notebook.

## Tools

* Python
* pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

## Status

**Work in progress**

The analysis will be expanded with additional EDA of peptide pairs, fragment evidence, scores, FDR measures, crosslink information, and other XL-MS characteristics.

## Goal

The goal is to build practical familiarity with proteomics and XL-MS data structures while developing a reproducible exploratory analysis workflow.
