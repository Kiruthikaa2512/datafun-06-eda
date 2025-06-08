
# US Housing Market Analysis: Supply-Demand Dynamics - EDA  Project

**Author**: Kiruthikaa NS
**Repo Name**: datafun-06-eda  
**Date**: June 2025  
**GitHub Repo**: [View this project on GitHub](https://github.com/Kiruthikaa2512/datafun-06-eda)

## Project Introduction

This exploratory data analysis (EDA) project investigates the **supply-demand dynamics in the US housing market** using a structured dataset from Kaggle. The primary goal is to uncover how different features — such as property size, location, room count, and amenities — correlate with housing prices, and how these relationships may reflect underlying patterns in market supply and buyer demand.

By applying visualization and descriptive statistics in a Jupyter Notebook, we aim to present a data story that reveals:
- Which features most influence home prices
- Regional trends that suggest supply-demand imbalances
- Possible market signals for pricing behavior

## Dataset Overview
- **Source**: [Kaggle - Factors Influencing House Price in US](https://www.kaggle.com/datasets/utkarshx27/factors-influence-house-price-in-us)
- **File Format**: CSV
- **Attributes**: Includes sale price, lot size, number of bedrooms/bathrooms, zip code, garage size, year built, etc.
- **Use Case**: Analyzing the dataset to identify housing market pressures and price influencers.

## Project Setup Steps
### 1. Repository Creation

- Created a GitHub repository named `datafun-06-eda`.
- Initialized the repository with a default `README.md`.

### 2. Clone & Local Development Setup

git clone https://github.com/your-Kiruthikaa2512/datafun-06-eda.git

* Opened the repository folder in **VS Code**.

### 3. .gitignore Configuration

Added the following to `.gitignore` to exclude unneeded files:
.vscode/
.venv/
__pycache__/
*.pyc
.DS_Store

### 4. Python Virtual Environment Setup

# Create virtual environment
python -m venv .venv

# Activate environment
# Windows:
.venv\Scripts\activate
# Mac/Linux:
source .venv/bin/activate

# Install dependencies
pip install pandas seaborn matplotlib jupyterlab pyarrow

## Notebook Summary

The Jupyter notebook (`datafun-06-eda.ipynb`) includes:

* **Project introduction and goals**
* **Data loading** and preliminary inspection
* **Descriptive statistics** and summary metrics
* **Univariate and bivariate visualizations** using Seaborn and Matplotlib
* **Feature engineering**: Renaming, creating new features
* **Data storytelling**: Markdown-supported insights on price influencers and patterns

## GitHub Repository Link

[https://github.com/your-Kiruthikaa2512/datafun-06-eda](https://github.com/your-Kiruthikaa2512/datafun-06-eda)

## Next Steps

* Continue detailed visualization and statistical analysis
* Interpret results and finalize narrative
* Review notebook structure and formatting before final push


