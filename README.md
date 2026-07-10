# 🧬 Breast Cancer Detection - Machine Learning Classification

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0+-orange.svg)](https://scikit-learn.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📌 Project Overview

Machine learning pipeline for breast cancer diagnosis using the Wisconsin Breast Cancer Dataset. Compares 6 classification algorithms with comprehensive preprocessing and hyperparameter optimization.

### 🎯 Results (Test Set)

| Metric | Score |
|--------|-------|
| **Accuracy** | **97%** |
| **ROC-AUC** | **0.998** |

---

## 📊 Model Performance

### Cross-Validation Results (5-Fold, Recall)

| Model | Best Parameters | CV Recall |
|-------|-----------------|-----------|
| **Logistic Regression** | C=100, penalty=l2 | 0.939 |
| **Decision Tree** | max_depth=5, criterion=gini, min_samples_leaf=4 | 0.925 |
| **Random Forest** | n_estimators=200, max_features='log2' | 0.939 |
| **SVM** | C=10, kernel=rbf, gamma=scale | 0.938 |
| **K-Nearest Neighbors** | n_neighbors=5, p=1, weights=uniform | 0.932 |
| **Naive Bayes** | var_smoothing=0.038 | 0.898 |

### Validation Set Performance

| Model | Accuracy | Precision | Recall | F1 | AUC |
|-------|----------|-----------|--------|-----|-----|
| **Logistic Regression** | 0.976 | 1.000 | 0.938 | 0.968 | 0.997 |
| **Decision Tree** | 0.941 | 1.000 | 0.844 | 0.915 | 0.933 |
| **Random Forest** | 0.965 | 1.000 | 0.906 | 0.951 | 0.992 |
| **SVM** | 0.976 | 1.000 | 0.938 | 0.968 | 0.995 |
| **Naive Bayes** | 0.929 | 0.933 | 0.875 | 0.903 | 0.987 |
| **K-Nearest Neighbors** | 0.965 | 1.000 | 0.906 | 0.951 | 0.995 |

### Test Set Classification Report

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| Benign | 0.96 | 0.98 | 0.97 | 54 |
| Malignant | 0.97 | 0.94 | 0.95 | 32 |
| **Accuracy** | | | **0.97** | **86** |

**Confusion Matrix:**
Predicted
Benign Malignant
Actual Benign 53 1
Actual Malignant 2 30

---

## 🛠️ Pipeline Features

- **Outlier Handling:** Custom Winsorizer (1st-99th percentile)
- **Feature Scaling:** MinMaxScaler
- **Validation Strategy:** Stratified 70/15/15 split
- **Hyperparameter Tuning:** GridSearchCV with 5-fold CV
- **Primary Metric:** Recall

## 🚀 Quick Start

```bash
# Clone
git clone https://github.com/yourusername/breast-cancer-classification.git
cd breast-cancer-classification

# Install
pip install -r requirements.txt

# Run
python breast_cancer_analysis.py
