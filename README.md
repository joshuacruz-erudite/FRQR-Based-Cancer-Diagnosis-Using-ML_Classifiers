# FRQR-Based Cancer Diagnosis Using Machine Learning Classifiers

## Overview

This repository contains the Python Jupyter notebooks accompanying the research study on Fuzzy-Rough QuickReduct (FRQR)-based feature selection and machine learning classification for breast cancer diagnosis.

The primary investigation uses the Wisconsin Diagnostic Breast Cancer (WDBC) dataset to evaluate FRQR-based feature reduction and its influence on classification performance and computational requirements.

A separate experiment using the Oxford Parkinson's Disease Detection Dataset is also included to examine the applicability of the workflow to a different classification problem.

## Repository Contents

| File | Description |
|---|---|
| `FRQR.ipynb` | FRQR feature-selection implementation and experiments. |
| `FRQR+ML.ipynb` | FRQR-based feature selection and machine learning classification experiments. |
| `Elastic Net.ipynb` | Feature-selection experiments using Elastic Net. |
| `Genetic algorithm.ipynb` | Feature-selection experiments using a Genetic Algorithm. |
| `LASSO.ipynb` | Feature-selection experiments using LASSO. |
| `Mutual Information.ipynb` | Feature-selection experiments using Mutual Information. |
| `ReliefF.ipynb` | Feature-selection experiments using ReliefF. |
| `Parkinson.ipynb` | Separate FRQR-based feature selection and classification experiment using the Parkinson's dataset for external validation. |
| `brca.csv` | CSV-formatted WDBC data used as input by the Genetic Algorithm notebook. |

## Datasets

### 1. Wisconsin Diagnostic Breast Cancer (WDBC)

- Source: UCI Machine Learning Repository
- Dataset ID: 17
- Instances: 569
- Input features: 30
- Classification: Benign and malignant
- Dataset URL: https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic
- DOI: https://doi.org/10.24432/C5DW2B

The WDBC dataset is accessed through scikit-learn's built-in dataset loader in the relevant notebooks. The `brca.csv` file is also included for the Genetic Algorithm experiments.

### 2. Oxford Parkinson's Disease Detection Dataset

- Source: UCI Machine Learning Repository
- Dataset ID: 174
- Recordings used: 195
- Acoustic features: 22
- Classification: Healthy and Parkinson's disease
- Dataset URL: https://archive.ics.uci.edu/dataset/174/parkinsons
- DOI: https://doi.org/10.24432/C59C74

The Parkinson's experiment is conducted independently and is not combined with the WDBC dataset.

## Software and Dependencies

The experiments were implemented using Python and Jupyter Notebook.

The notebooks use scientific computing and machine learning libraries, including:

- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- SciPy
- Scikit-rebate (skrebate)

Additional packages may be required depending on the notebook being executed. Refer to the individual notebook imports and installation cells.

## Running the Notebooks

1. Download or clone this repository.
2. Install the required Python packages.
3. Open the relevant notebook using Jupyter Notebook or JupyterLab.
4. Execute the notebook cells in the appropriate sequence.

For `Genetic algorithm.ipynb`, keep `brca.csv` in the repository's root directory, alongside the notebook. The notebook reads this file using the relative filename `brca.csv`.

The Parkinson's notebook downloads its dataset directly from the UCI repository and therefore requires an internet connection.

## Reproducibility

The notebooks are provided as the research code accompanying the manuscript. They contain the experimental implementations, parameter configurations and saved outputs associated with the study.

The code is provided for inspection, reproducibility and further academic research.

## Dataset Acknowledgement

The WDBC dataset is attributed to Wolberg, Mangasarian, Street and Street (1993), UCI Machine Learning Repository, DOI: 10.24432/C5DW2B.

The Parkinson's dataset is attributed to Little (2007), UCI Machine Learning Repository, DOI: 10.24432/C59C74.

## Citation

Please cite the associated research article when using this code in subsequent research. The original datasets should also be cited through their respective UCI Machine Learning Repository references.
