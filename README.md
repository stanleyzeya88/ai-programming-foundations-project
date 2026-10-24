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
```
---

## Key Workflow Modules

### 1. Custom Cleaning Functions
- **`clean_column_names(dataframe)`**: Standardizes column headers by stripping whitespace, converting text to lowercase, and replacing spaces with underscores (`snake_case`).
- **`add_quality_tier(dataframe)`**: Discretizes numerical quality ratings (3–8) into three ordinal tiers: **Low** (3–4), **Medium** (5–6), and **High** (7–8).

### 2. Exploratory Data Analysis (EDA)
- **`compute_wine_summary(dataframe)`**: Computes aggregated summary statistics (**mean**, **standard deviation**, and **median**) across key chemical properties (`alcohol`, `volatile_acidity`, `citric_acid`, `sulphates`, `ph`) grouped by `quality_tier`.

### 3. Visualizations
1. **Plot 1:** Box plot illustrating alcohol content trends across numerical quality scores.
2. **Plot 2:** Correlation matrix heatmap evaluating linear relationships among chemical properties.
3. **Plot 3:** Scatter plot displaying the inverse relationship between volatile acidity and citric acid colored by quality tier.

---

## Environment Setup & Installation

### Prerequisites
- Python 3.10+
- Anaconda / Miniconda or `venv`

### Step-by-Step Instructions

1. **Clone the repository:**
   ```text
   ```bash
   git clone https://github.com/stanleyzeya88/ai-programming-foundations-project.git
   cd ai-programming-foundations-project
   ```

3. **Create and activate a Conda environment:**
   ```text
   ```bash
   conda create -n capstone-proj1 python=3.10 -y
   conda activate capstone-proj1
   ```
Install dependencies:
   ```text
   pip install -r requirements.txt
   ```
Launch Jupyter Notebook:
   ```text
   jupyter notebook data_workflow.ipynb
   ```

### Citation & Dataset Source
- Dataset: UCI Machine Learning Repository 
- Wine Quality Dataset (Cortez et al., 2009).
- License: Open Academic / Research Use.
