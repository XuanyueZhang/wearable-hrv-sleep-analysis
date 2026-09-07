# Wearable HRV and Sleep Efficiency Analysis

## Overview
This project investigates whether heart rate variability (HRV) features derived from wearable devices can be used to predict nightly sleep efficiency in real-world conditions.

The analysis compares pre-sleep and overnight HRV windows and evaluates both interpretable linear models and nonlinear machine-learning models.

## Objectives
- Predict nightly sleep efficiency using HRV-derived features
- Compare pre-sleep and overnight HRV windows
- Identify important HRV predictors of sleep efficiency
- Evaluate participant-level generalization using grouped cross-validation
- Explore participant symptom profiles using clustering

## Data
The project uses longitudinal wearable HRV and sleep diary data from a publicly available research dataset.

To avoid redistributing source data improperly, raw data are not included in this repository.

## Methods
- Data cleaning and quality control
- Night-level feature engineering
- Time-domain HRV features
- Frequency-domain HRV features
- Participant-wise GroupKFold cross-validation
- Elastic Net regression
- Gradient Boosting regression
- K-means clustering
- Model evaluation using MAE, RMSE, and R²

## Tools
- Python
- pandas
- NumPy
- scikit-learn
- Jupyter Notebook
- matplotlib

## Key Findings
- Overnight HRV provided more usable observations than the pre-sleep window
- Elastic Net showed more stable generalization than Gradient Boosting
- Participant-wise validation helped reduce leakage between training and test data
- Predictive performance suggested that HRV alone has limited ability to explain nightly sleep efficiency

## Repository Structure

```text
wearable-hrv-sleep-analysis/
├── notebooks/
├── scripts/
├── figures/
├── results/
├── README.md
└── requirements.txt

## Author
Xuanyue Zhang  
M.S. Biological Data Science  
Arizona State University
