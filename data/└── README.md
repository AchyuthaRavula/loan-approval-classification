## Data Directory

This directory follows standard data engineering practices.

### raw/
- Contains the original, untouched dataset
- Dataset source:
  🔗 https://www.kaggle.com/datasets/taweilo/loan-approval-classification-data
- Raw data is not committed to this repository to keep it lightweight and compliant

### processed/
- Intended for cleaned and feature-engineered datasets
- Includes encoded categorical variables and scaled numerical features
- Processed data is generated dynamically using PySpark pipelines in the notebook

### Dataset Summary
- Records: ~45,000
- Features: 14
- Target variable: `loan_status`
- Data type: Synthetic financial loan application data

