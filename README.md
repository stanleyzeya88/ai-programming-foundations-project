# Modular Data Workflow for Wine Quality Analysis (Project #1)

## Project Overview
This repository contains a modular, reproducible Python data processing and exploratory analysis workflow analyzing the UCI Wine Quality dataset (`winequality-red.csv`). The project standardizes feature representations, discretizes numerical quality ratings into categorical tiers, aggregates physicochemical attributes, and generates publication-ready visualizations.

---

## Repository Structure
```text
ai-programming-foundations-project/
├── data_workflow.ipynb          # Main Jupyter Notebook with data processing, EDA, & plots
├── winequality-red.csv          # UCI Red Wine Quality dataset (semicolon delimited)
├── winequality-white.csv        # UCI White Wine Quality dataset
├── plot1_alcohol_vs_quality.png # Box plot: Alcohol distribution across quality ratings
├── plot2_correlation_heatmap.png# Heatmap: Physicochemical property correlation matrix
├── plot3_acidity_comparison.png # Scatter plot: Volatile acidity vs. citric acid by tier
├── module_summary.pdf           # Academic summary report (Methodology, EDA, Bias, References)
├── requirements.txt             # Python dependencies for reproducible environment
└── README.md                    # Project documentation and setup guide
