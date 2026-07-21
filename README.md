# CS7643 Uplift Modeling

This repository is for a CS7643 deep learning group project on uplift modeling and individualized treatment effect estimation.

## Project Description

The project is centered on the MineThatData / Hillstrom Email Analytics dataset and may include:

- exploratory data analysis
- traditional baselines
- uplift modeling methods
- deep learning models
- evaluation and reporting

## Dataset Location

`data/raw/hillstrom_email.csv`

## Folder Structure

```text
cs7643-uplift-modeling/
├── README.md
├── requirements.txt
├── .gitignore
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_baselines.ipynb
│   ├── 03_deep_learning.ipynb
│   └── 04_evaluation.ipynb
├── results/
│   ├── figures/
│   ├── metrics/
│   └── outputs/
└── report/
    ├── figures/
    └── notes.md
```

## Folder Guide

- `data/raw/`: original source data, including the optional tracked Hillstrom CSV
- `data/processed/`: cleaned data, transformed tables, and feature sets
- `notebooks/`: primary workspace for analysis and model development
- `results/figures/`: generated plots for experiments and presentations
- `results/metrics/`: saved evaluation summaries and score tables
- `results/outputs/`: other generated artifacts from notebook runs
- `report/`: writeup notes and report figures

# Development Environment (macOS)

## Recommended: Micromamba

We recommend using Micromamba instead of an older Anaconda installation, as dependency resolution for `econml` is significantly faster and more reliable.

### Create the environment

```bash
micromamba create -n cs7643-project2 -c conda-forge \
  python=3.10 \
  numpy \
  pandas \
  scipy \
  scikit-learn=1.6 \
  matplotlib \
  jupyterlab \
  tqdm \
  econml=0.16 \
  -y
```

Activate it:

```bash
micromamba activate cs7643-project2
```

Install PyTorch:

```bash
pip install torch==2.2.2 tensorboard
```

Downgrade NumPy (required for PyTorch 2.2):

```bash
micromamba install -c conda-forge "numpy<2"
```

### Verify

```bash
python -c "import numpy, pandas, sklearn, torch, econml"
python -c "from econml.dml import CausalForestDML"
```

Expected versions:

```
Python 3.10
NumPy 1.26.4
scikit-learn 1.6.1
PyTorch 2.2.2
EconML 0.16.0
```


