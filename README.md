# Metabolomics-based classification of invasive ductal breast cancer

This repository contains the analysis code used to evaluate metabolomics data for binary classification of invasive ductal breast cancer using repeated stratified train/test splits and Random Forest models.

## Manuscript
This code accompanies the manuscript:

**Blood and urine biomarkers in invasive ductal breast cancer: Mass spectrometry applied to identify metabolic alterations**

## Repository contents
- `metabolomics_classification.ipynb` — main analysis workflow
- `requirements.txt` — Python dependencies

## Expected input

A CSV file containing:
- one binary target column named `Class` (values: 0 and 1)
- feature columns (e.g. metabolite intensities)

## Method overview

The workflow:
1. loads the dataset
2. performs repeated stratified 80/20 train/test splits
3. applies train-only normalization
4. optionally selects top-k features using training-set Gini importance
5. trains a Random Forest classifier
6. evaluates:
   - Accuracy
   - Recall
   - F1 score
   - ROC-AUC
   - PR-AUC
   - Confusion matrices
   - Mean ROC and PR curves

## Reproducibility

All results are based on fixed random seeds and train-only preprocessing to avoid data leakage.

## Contact

For questions, please contact: [your email]
