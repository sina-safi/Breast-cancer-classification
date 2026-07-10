# Breast Cancer Classification using Machine Learning

## Overview

This project compares six machine learning algorithms for classifying breast cancer tumors as benign or malignant using the Wisconsin Breast Cancer Dataset.

The main goal was to build a complete machine learning workflow, including data preprocessing, model selection, hyperparameter tuning, and performance evaluation.

---

## Dataset

- **Dataset:** Wisconsin Breast Cancer Dataset
- **Samples:** 569
- **Features:** 30 numerical features
- **Target:** Diagnosis (Benign / Malignant)

---

## Project Workflow

1. Data loading and cleaning
2. Exploratory Data Analysis (EDA)
3. Correlation analysis
4. Train / Validation / Test split (70/15/15)
5. Outlier handling using a custom Winsorizer
6. Feature scaling with MinMaxScaler
7. Model training
8. Hyperparameter tuning using GridSearchCV
9. Model evaluation
10. ROC Curve and Confusion Matrix visualization

---

## Models

The following models were trained and compared:

- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- K-Nearest Neighbors
- Gaussian Naive Bayes

---

## Results

| Metric | Value |
|---------|------:|
| Accuracy | 97% |
| ROC-AUC | 0.998 |

The best model achieved:

- Accuracy: **97%**
- Precision: **97%**
- Recall: **94%**
- ROC-AUC: **0.998**

---

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Repository Structure

```
Breast-cancer-classification/
│
├── Breast-cancer-classification.ipynb
├── README.md
├── requirements.txt
└── images/
```

---

## Future Improvements

Some possible improvements include:

- Feature selection techniques
- XGBoost and LightGBM models
- SHAP feature importance
- Model deployment using Streamlit

---

## Notes

This project was created for learning and portfolio purposes. It is **not intended for medical diagnosis**.

---

## Author

**Sina Safi**

GitHub: https://github.com/sina-safi