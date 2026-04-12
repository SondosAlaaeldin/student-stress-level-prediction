# Student Stress Level Prediction

## Overview
This project predicts student stress levels using survey and physiological data.  
It combines data preprocessing, exploratory data analysis, and machine learning to identify factors associated with stress.

## Dataset
- Source: [Kaggle Student Stress Monitoring Dataset]([text](https://www.kaggle.com/datasets/mdsultanulislamovi/student-stress-monitoring-datasets))
- Features: Psychological, Physiological, Environmental, Academic, and Social factors
- Target: `stress_level` (multiclass classification)

## Exploratory Data Analysis
- Outlier detection and removal
- Distribution analysis for demographic and stress-related variables
- Correlation heatmaps
- Category-wise factor analysis

## Modeling (My Contribution)
I led the modeling and evaluation phase, including:

- Data preprocessing (encoding, scaling, imputation)
- Built classification models:
  - Support Vector Classifier (SVC)
  - Decision Tree
  - K-Nearest Neighbors (KNN)
- Hyperparameter tuning using GridSearchCV
- Performance evaluation using:
  - Accuracy
  - Weighted F1-score
  - ROC-AUC
  - Confusion Matrix
  - Classification Report
- Saved trained models using Pickle

## Results

| Model | Test Accuracy | Weighted F1 | ROC-AUC |
|------|---------------|------------|--------|
| SVC | 95.11% | 0.943 | 0.998 |
| Decision Tree | 95.74% | 0.956 | 0.984 |
| KNN | 95.27% | 0.950 | 0.990 |

## Tools
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

## How to Run
1. Install dependencies from `requirements.txt`
2. Open `stress_classification.ipynb`
3. Run all cells