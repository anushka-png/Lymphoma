# Lymphoma Research Project

## Overview

This repository contains code and resources for two main research projects focused on lymphoma data analysis:

1. **Custom Model for Lymphoma Image Classification**  
   Implements deep learning and machine learning approaches for classifying lymphoma subtypes using histopathology images.

2. **Gene Expression Data Statistical Analysis**  
   Provides statistical and machine learning analysis of gene expression data for lymphoma patient samples.

---

## Repository Structure

- `Lymphoma_Data_Custom_Model.ipynb`  
  Jupyter notebook for image-based custom model development and evaluation.

- `Lymphoma_Gene_Expression_Data_Statistical_Analysis.ipynb`  
  Jupyter notebook for gene expression data analysis and feature selection.

- `README.md`  
  Project documentation.

---

## Requirements

Install all required packages using:

```sh
pip install tensorflow numpy matplotlib scikit-learn opencv-python
```

---

## Dataset Summary

### 1. Lymphoma Gene Expression Dataset
*Referenced in [Lymphoma_Gene_Expression_Data_Statistical_Analysis.ipynb](Lymphoma_Gene_Expression_Data_Statistical_Analysis.ipynb)*


# Table1: Dataset Summary (Gene expression data)

| Category          | Details                                                                 |
|-------------------|-------------------------------------------------------------------------|
| Number of Samples | 77                                                                      |
| Number of Features| 7,131 (Gene expression values: V1 to V7129)                             |
| Feature Type      | Quantitative (Continuous numerical values per gene)                     |
| Label Columns     | TYPE (Lymphoma subtype), DTH (Patient status)                           |
| Class Labels (TYPE)| 2 classes – DLBCL, FL                                                  |
| Class Labels (DTH)| 2 classes – CURED, FATAL                                                |
| Missing Values    | None reported (assumed clean)                                           |
| Encoding          | Labels encoded as DTH_ENC and TYPE_ENC for classification models        |

---


### 2. Lymphoma Image Dataset
*Referenced in [Lymphoma_Data_Custom_Model.ipynb](Lymphoma_Data_Custom_Model.ipynb)*


# Table2: Dataset Structure and Feature Breakdown (Image dataset)

| Category             | Samples  | Features | Details                                |
|----------------------|----------|----------|----------------------------------------|
| Total Images         | 15,000   | -        | 5,000 per class                         |
| Training Data        | 12,000   | -        | 80% split with augmentation             |
| Validation/Test Data | 3,000    | -        | 20% holdout                             |
| Quantitative Data    | 15,000   | Numeric  | Mean, StdDev, Texture, Edges, Histogram |
| Qualitative Labels   | 3        | Categorical | MCL, CLL, FL                          |
| Independent Variables| -        | -        | RGB Pixels / Engineered Features        |
| Dependent Variables  | -        | -        | Class Labels                            |

---

## Usage

### 1. Image Classification

- Run `Lymphoma_Data_Custom_Model.ipynb` to train and evaluate hybrid deep learning and classical ML models on lymphoma images.
- Models are saved as `.h5` or `.pkl` files for future inference.

### 2. Gene Expression Analysis

- Run `Lymphoma_Gene_Expression_Data_Statistical_Analysis.ipynb` for preprocessing, feature selection, and statistical analysis of gene expression data.

---

## Data Sources

- **Image Dataset:**  
  Obuli Sai Naren. (2022). Multi Cancer Dataset [Data set]. Kaggle.  
  [https://doi.org/10.34740/KAGGLE/DSV/3415848](https://doi.org/10.34740/KAGGLE/DSV/3415848)

- **Gene Expression Dataset:**  
  Deepthimahanthi, R. (2020, April 8). Non-Hodgkin lymphoma cell detection and patient’s status by gene expression profiling (Using supervised-learning) [Data set]. GitHub.  
  [https://github.com/Roopesh-DMahanthi/lymphoma-cell-detection/blob/master/Lymphoma-Dataset.csv](https://github.com/Roopesh-DMahanthi/lymphoma-cell-detection/blob/master/Lymphoma-Dataset.csv)

---

## Citation

If you use this repository for your research, please cite appropriately.

---

## Contact

For questions or collaboration, please contact the repository owner.
