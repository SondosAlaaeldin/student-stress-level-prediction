# Student Stress Level Prediction

## Overview
This group project predicts student stress levels using survey and physiological data.  
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

# Modeling (My Contribution)
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


## Result Analysis

Three machine learning models were trained and evaluated to predict stress levels: **SVC, Decision Tree, and KNN**. Each model was optimized using **GridSearchCV with cross-validation** and evaluated using **Accuracy, Weighted F1-score, and ROC-AUC**.

---

## Key Findings

## Decision Tree (Best Overall Model)
- Achieved the **highest test accuracy (95.74%)**
- Also delivered the **best Weighted F1-score (0.956)**
- Provides the most balanced performance across all stress classes
- Slightly lower ROC-AUC compared to SVC but more stable overall

---

## SVC (Best Class Separation)
- Achieved the **highest ROC-AUC (0.998)**, indicating excellent class separability
- Slightly lower accuracy and F1-score than Decision Tree
- Very strong performance in distinguishing stress levels

---

## KNN (Consistent Performer)
- Competitive results across all metrics
- Slightly below Decision Tree and SVC in overall ranking
- Shows that local similarity patterns in the dataset are meaningful

---

## Interpretation

- All models achieved **very high performance (>95% accuracy)**
- This indicates that the dataset contains **strong, learnable patterns for stress prediction**
- Proper preprocessing (scaling, encoding, and outlier handling) significantly improved model performance

---

## Conclusion

- **Best overall model:** Decision Tree  
- **Best for class separation:** SVC  
- **Balanced alternative:** KNN  

Overall, the models demonstrate that stress level prediction is highly feasible using the selected features and preprocessing pipeline.

## Tools
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

## How to Run
1. Install dependencies from `requirements.txt`
2. Open `stress_classification.ipynb`
3. Run all cells