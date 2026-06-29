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
