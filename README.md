# Metabolomics-based classification
This repository contains the analysis code used to evaluate metabolomics data for binary classification of cancer/control samples using Random Forest models and GINI Index.

## Manuscript
This code accompanies the manuscript:

**Dimensionality reduction and metabolite panel derivation in urinary metabolomics based on Random Forest with Gini index feature selection**

## Repository contents
- `metabolomics_classification.ipynb` — main analysis workflow
- `requirements.txt` — Python dependencies

## Expected input

A CSV file containing:
- one binary target column named `Class` (values: 0 and 1)
- feature columns
